# Reinforcement Learning

* [Intro to RL](https://arena3-chapter2-rl.streamlit.app/\[2.1]\_Intro\_to\_RL)&#x20;
  * Use this link for Sutton and Barto instead: [https://web.stanford.edu/class/psych209/Readings/SuttonBartoIPRLBook2ndEd.pdf](https://web.stanford.edu/class/psych209/Readings/SuttonBartoIPRLBook2ndEd.pdf)&#x20;
  * For Tabular RL & Policy Improvement: I would definitely recommend doing the suggested readings before you get started.
  * Once you're done, read up to (but not including) the section titled "Common Approaches" from [Lilian Weng's great RL overview](https://lilianweng.github.io/posts/2018-02-19-rl-overview/) once done with this chapter. Also check out [Spinning Up's intro to RL](https://spinningup.openai.com/en/latest/spinningup/rl\_intro.html). Keep referencing these resources as need be.
* [Q-Learning and DQN](https://arena3-chapter2-rl.streamlit.app/\[2.2]\_Q-Learning\_and\_DQN)
  * In DQN, really understand that the target networks are predicting the q-value for the next state while the q-networks are predicting the q-value for the current state! This is probably very obvious, but I didn't quite register it at first pass. I ended up spending a day banging my head against the wall and trying to figure out how the hell DQN works if both networks were predicting the q-value for the same state and the target was almost guaranteed to be worse.  &#x20;
* [PPO](https://arena3-chapter2-rl.streamlit.app/\[2.3]\_PPO)
  * For me, PPO felt like it came out of left field, and it took spending more time learning about policy gradients to really grok things.
    * Before you get started, read the rest of Lilian Weng's post and read up on [policy gradients from Spinning Up](https://spinningup.openai.com/en/latest/spinningup/rl\_intro3.html) if you want to go deeper in the math. &#x20;
      * Look for other resources if things don't quite make sense yet. Once you feel a little confident, move on to the Arena lesson.
* [RLHF](https://arena3-chapter2-rl.streamlit.app/\[2.4]\_RLHF)
  * I think this week was the most straightforward out of all of them. It logically follows the PPO lesson fairly smoothly.&#x20;
