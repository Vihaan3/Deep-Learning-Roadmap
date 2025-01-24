# Grokking the Fundamentals

<details>

<summary>Get familiar w/ any plotting library</summary>

* I would recommend Plotly
  * If you're interested in Plotly, see [this](https://www.perfectlynormal.co.uk/blog-plotly-widgets) and play around for an hour or so while using Anki to memorize all the basics

</details>

<details>

<summary>Neural Networks Basics</summary>

* Videos
  * Watch up to (but not including) “backpropagation calculus” from 3Blue1Brown's Neural Networks [playlist](https://www.3blue1brown.com/topics/neural-networks)&#x20;
* Revisit and complete the [coding page](coding.md) until the second stop.
* Practice
  * [How Does a Neural Network Really Work](https://www.kaggle.com/code/jhoward/how-does-a-neural-net-really-work)
  * [Linear Model and Neural Net From Scratch](https://www.kaggle.com/code/jhoward/linear-model-and-neural-net-from-scratch)
  * **How to practice** (relevant for all future Andrej Karpathy videos as well)
    * Run each cell and understand why it works. If you don't get it, ask GPT until you do. **Don't let your eyes glaze over and start skimming.**
      * Create a new cell that describes what the original cell does in comments. Include the basic functionality and hints for any particularly thorny implementation details as well as _why_.
      * Re-implement in your new cell&#x20;
    * Once you feel like you understand each cell, condense cells until each one represents a significant "chunk".&#x20;
      * Do the same process as above
    * Remove all hints and try to do the whole thing by yourself. At most, keep a bulleted list of all the high-level logical "chunks". &#x20;
    * Ideally, you want to now do the whole thing with new specifications (new dataset, slightly different architecture, etc).
  * (Recommended Bonus): go through the [fastbook version ](https://github.com/fastai/fastbook/blob/master/04_mnist_basics.ipynb)of this lesson. If you've already practiced extensively with the previous 2 notebooks, you can go through this relatively quickly and just understand each cell.&#x20;
* Revisit and complete the [last section of the coding page](coding.md#getting-better-with-tensors).
* Progress check:
  * Be able to answer the questions at the end of the fastbook.&#x20;
  * Understand weights as encoding transformations of space.
  * Build the intuition that a neural network is essentially the same thing as the line of best fit in a linear regression, except just bigger and more complex.&#x20;

</details>

<details>

<summary>Backprop</summary>

* Watch both of Artem Kirsanov's [lovely explainer](https://youtu.be/SmZmBKc7Lrs) on backprop and 3B1B's [backpropagation calculus](https://www.3blue1brown.com/lessons/backpropagation-calculus) (definitely read through the text after watching the video; it helps a lot with clarification)
* Watch Andrej Karpathy's lecture on [neural networks](https://youtu.be/VMj-3S1tku0) (it's okay if some of the exact backprop stuff doesn't make complete sense quite yet)
  * For all Andrej Karpathy videos, make sure you read the descriptions. They usually have Colab notebooks to follow along in and questions + exercises.&#x20;
    * I would recommend either following along in the Colab notebook provided but pausing every so often to re-implement yourself or just following along and implementing in a separate Colab notebook. Also, always try to work on at least one of the exercises.&#x20;
* Progress check
  * Really, truly, genuinely, understand that a neural net is just a function that is trying to fit some points in a space in a way that allows it to predict future points with as much accuracy as possible. Artem Kirsanov's video builds some good intuition for that.&#x20;
    * If you've taken a statistics class or followed along the statistics page, and remember looking at least-squares regression lines, just think of a neural network as a more complicated form of that.&#x20;
      * Now, if you'll recall things like underfitting/overfitting, being wary of extrapolation, using metrics and other graphs to evaluate fit, and the impact that outliers can have on the line, things will feel very familiar as you continue to watch Andrej Karpathy videos in future sections.
  * Understand that backpropagation is just the chain rule on multivariate functions.
  * More on "neurons that fire together, wire together": Hopefully this is another helpful way to understand _why_ neural nets learn if the linear regression analogy didn't help. At the very first layer, you have a pure representation of the input. At the very last layer, you have the output and the loss. From there, as you go back and make the connections with the brightest neurons higher, it "wires together" the brightest neurons. Then, at the last layer, the representation of the image will be fused with that overall chain. Neurons that fire when "seeing" a 2, will wire with those while "thinking" about a 2, and those will wire at the end with the neuron that outpus a 2. This is also why there's so much randomness. Which neurons get wired together is pretty heavily dependent on the initial random values that you set the weights to, so different neurons (at least in such a small model) won't necessarily pick up on the patterns that you might expect in the way you might expect. &#x20;

- [Become a backprop ninja part 1](https://arena3-chapter0-fundamentals.streamlit.app/\[0.4]_Backprop) :)
  * A lot might feel repetitive so skim if necessary. The last section is definitely worthwhile in it's entirety.&#x20;
  * Note: When I first went through ARENA, I didn't notice the colab notebooks at the top and was doing everything in my own Jupyter notebook. Definitely use the colab notebook provided for exercises to check your answers.&#x20;

</details>

<details>

<summary>Language Modeling (Mostly) w/ Andrej Karpathy </summary>

* **Meta-note**: for each video that has exercises in the description, try to answer all the questions and do at least one of the coding exercises. I didn't think to check the description until I looked at the videos again while linking them here. I have answers to some of the exercises [here](https://github.com/Vihaan3/Karpathy-Exercises/tree/main). &#x20;
* [Language Modeling Part 1: Makemore](https://www.youtube.com/watch?v=PaCmpygFfXo)
  * Make sure you understand all of the Pytorch operations
  * Explain broadcasting
  * What is negative log-likelihood?
  * What is softmax?
  * What were the two different models trained in the video? What are the key differences? Why might you prefer the second over the first (even if they have near-identical results as of now)?
* [Language Modeling Part 2: MLP](https://youtu.be/TCH_1BHY58I)
  * Why do you split into train/dev/test splits? Roughly what proportions are standard?
  * Why do you use minibatches? This video builds good intuition to what 3b1b mentions here: [https://youtu.be/Ilg3gGewQ5U?t=613](https://youtu.be/Ilg3gGewQ5U?t=613).
  * How do you find a good initial learning rate?
* [Language Modeling Part 3: MLP Internals](https://youtu.be/P6sfmUTpUmc)
  * Explain Kaiming init.&#x20;
    * Why do you even want to use it?&#x20;
    * How do you do it?
    * Why was it a breakthrough?
  * Repeat the above for batchnorm.
  * Take note of the different visualizations. What is each of them supposed to tell you? What do they look like when things are good? What do they look like when things are broken?
    * Make sure you can reproduce the visualizations using whatever plotting library you've learned.&#x20;
* [Become a backprop ninja part 2](https://youtu.be/q8SA3rM6ckI) :).
  * Do your best. I think it really helps build intuition for how gradients "flow" through a neural net.
* [Language Modeling Part 4: Wavenet](https://youtu.be/t3YJ5hKiMQ0)
* You'll notice that there are still a couple of videos left in Andrej's course. That's not a mistake! We'll get back them later.

</details>

<details>

<summary>Going a little deeper w/ Arena</summary>

* [Ray Tracing](https://arena3-chapter0-fundamentals.streamlit.app/\[0.1]_Ray_Tracing): I didn't do this during my first pass through the ARENA material, and I found that it was actually really helpful for upskilling w/ Pytorch.&#x20;
* [CNNs and ResNets](https://arena3-chapter0-fundamentals.streamlit.app/\[0.2]_CNNs_&_ResNets): This will probably feel somewhat familiar to the later Karpathy videos, and you can skip around a bit but I think it's good practice w/ Pytorch modules.
* [Optimization](https://arena3-chapter0-fundamentals.streamlit.app/\[0.3]_Optimization): This is a really important chapter.&#x20;
  * What is the advantage of the Adam Optimizer?
    * It combines two techniques:&#x20;
      * using the sum of the gradient: for speed and to escape local minima&#x20;
      * using the sum of gradient squared: allows you to move in sparse directions because you are dividing the learning rate by the square of the gradients (parameters that have had large gradients and therefore large updates in the past will have lower learning rates while parameters that have had smaller gradients and therefore smaller updates will have higher learning rates.)
* [GANs and VAEs](https://arena3-chapter0-fundamentals.streamlit.app/\[0.5]_VAEs_&_GANs): Don't feel like there's that much conceptually new covered (besides the intro to VAEs and GANs) but I thought it was a nice way to tie everything in this section together.&#x20;

</details>

<details>

<summary>Exercises/Mini-Projects</summary>

You should stop here and really work on some exercises/mini-projects that can help you actually understand what you've learnt. One of the issues with really good educators is that good lessons can make it easy to feel like you know far more than you actually do.&#x20;

* If you haven't already, really do try some of the Karpathy exercises. I have answers to some of what I considered the harder ones [here](https://github.com/Vihaan3/Karpathy-Exercises/blob/main/Karpathy_Exercises.ipynb).
* [Autodiff](https://github.com/UlisseMini/light) for another language that you know (basically replicate the basics of Pytorch but in another language).&#x20;
* Write a [neural network class](https://github.com/Elijah-Bodden/Numpy-NN) purely in numpy.

</details>
