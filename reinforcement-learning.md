# Reinforcement Learning

<details>

<summary>Intro to RL</summary>

Core Lesson: [Intro to RL](https://arena3-chapter2-rl.streamlit.app/\[2.1]_Intro_to_RL)

* Use this link for Sutton and Barto instead: [https://web.stanford.edu/class/psych209/Readings/SuttonBartoIPRLBook2ndEd.pdf](https://web.stanford.edu/class/psych209/Readings/SuttonBartoIPRLBook2ndEd.pdf)&#x20;
* For Tabular RL & Policy Improvement: I would definitely recommend doing the suggested readings before you get started.
* Once you're done, read up to (but not including) the section titled "Common Approaches" from [Lilian Weng's great RL overview](https://lilianweng.github.io/posts/2018-02-19-rl-overview/) once done with this chapter. Also check out [Spinning Up's intro to RL](https://spinningup.openai.com/en/latest/spinningup/rl_intro.html) and [Berkeley's Deep RL Bootcamp](https://sites.google.com/view/deep-rl-bootcamp/lectures) from 2017. Keep referencing these resources as need be.

</details>

<details>

<summary>Q-Learning and DQN</summary>

Core Lesson: [Q-Learning and DQN](https://arena3-chapter2-rl.streamlit.app/\[2.2]_Q-Learning_and_DQN) &#x20;

* In DQN, really understand that the target networks are predicting the q-value for the next state while the q-networks are predicting the q-value for the current state! This is probably very obvious, but I didn't quite register it at first pass. I ended up spending a day banging my head against the wall and trying to figure out how in the world DQN worked if both networks were predicting the q-value for the same state, and the target was almost guaranteed to be worse.&#x20;
* Progress Check
  * Understand that DQN is just an extension of Q-learning to deep learning. Instead of using a table to store all the Q-values for each state-action pair, we train a neural network to learn this function for us.
  * Give a conceptual overview of the steps of DQN.
    * use some kind of policy (usually epsilon-greedy)
    * store these experiences in the _replay buffer_
    * use the values from the replay buffer to calculate a TD error (temporal difference error) between a target network and the Q-network (where the Q-network provides the prediction for the current Q-value and the target network provides the prediction for the Q-value after the next step)
    * update the Q-network via gradient descent
    * every so often, copy the Q-network weights over to the target network
  * Why do you even need a target network?
    * Ans: Remember how in SARSA you were learning from the next action? This is the same thing (and in the first paper there actually wasn't even a target network). It was noticed that learning was very unstable because the Q-network was always changing, so the labels it was chasing after were always changing. Having a lagged copy of the Q-network helps provide it a consistent thing to optimize towards while updating the targets often enough that they improve as well and don't get left behind by the Q-network.
  * Is DQN suited for continuous action spaces?
    * No, because the Q function takes in states and returns Q-values (estimated future reward) for each discrete action. It's not even great for large action spaces.

</details>

<details>

<summary>PPO</summary>

Core Lesson: [PPO](https://arena3-chapter2-rl.streamlit.app/\[2.3]_PPO)

* For me, PPO felt like it came out of left field, and I was incredibly confused when I first went through the PPO lesson. It took spending more time learning about policy gradients upfront to really grok things.
  * Before you get started, read the rest of Lilian Weng's post and read up on [policy gradients from Spinning Up](https://spinningup.openai.com/en/latest/spinningup/rl_intro3.html) if you want to go deeper in the math.
    * Other good resources if the two above don't make much sense:
      * A different Lilian Weng's [post](https://lilianweng.github.io/posts/2018-04-08-policy-gradient/) specifically on policy gradients&#x20;
      * [Nathan Lambert](https://rlhfbook.com/c/11-policy-gradients.html)
    * Even though learning the same information from different lenses can often help (and I usually recommend it), you should also be wary of taking this to the extreme. Once you have a solid mental model, move into the lesson.&#x20;
* Progress Check
  * Describe the interplay between the actor and critic networks.
    * The actor network needs the critic network to estimate the gradient and perform gradient ascent, and the critic is learning the value function of the actor's current policy. Basically, the actor network learns the policy and the critic network learns the values function V(s).
  * What is the major innovation of PPO over TRPO?&#x20;
    * PPO has a simpler optimization process because of the clipped surrogate objective.&#x20;
  * Why did you do a shared network for actor and critic only for Atari (and not for Cartpole or Mujoco)?
    * Ans: Atari games have massive observation spaces while Cartpole and Mujoco have much smaller ones (4 and 11 respectively). The shared network generates high-level representations of the state, and the diverging branches for actor and critic at the end can use the same representation at the start.
  * What is the difference between on-policy and off-policy RL? What is the difference in how they update?
    * Ans: On-policy: The agent learns the value of the policy it is currently following. Basically, the agent learns directly from the actions it is actually taking. Off-policy: The agent learns the value of the optimal policy independent of the actions taken by the current policy. The agent learns about a policy different than the one currently being followed.
    * Update ans: On-policy: Updates are based on the difference between expected rewards from one step to the next. Off-policy: Updates are based on the difference between action selected by current policy and optimal action.
  * What is the difference between model-based and model-free RL?
    * Model-based algorithms have access to the transition probability distribution and the reward function while model-free algorithms help the agent learn about the world via interaction.

</details>

<details>

<summary>RLHF</summary>

Core Lesson: [RLHF](https://arena3-chapter2-rl.streamlit.app/\[2.4]_RLHF)

I think that this week was the most straightforward out of all of them; it logically follows the PPO lesson fairly smoothly. If you're having trouble, most of the same resources from the PPO section should still help. &#x20;

</details>

<details>

<summary>Exercises/Mini-Projects</summary>

* The Bonus tabs in the lessons are gems for mini-project ideas
* The ones that stood out to me in terms of "coolness" were:
  * RLHF
    * learning a human preference reward model
    * the suggested paper replications
    * differential learning rates
  * PPO
    * Wordle&#x20;
    * Other discrete environments

</details>
