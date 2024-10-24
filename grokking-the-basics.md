# Grokking the Basics

<details>

<summary>Get familiar w/ any plotting library</summary>

* I would recommend Plotly
  * If you're interested in Plotly, see [this](https://www.perfectlynormal.co.uk/blog-plotly-widgets) and play around for an hour or so while using Anki to memorize all the basics

</details>

<details>

<summary>Neural Networks Basics</summary>

* Videos
  * Watch up to (but not including) “backpropagation calculus” from 3Blue1Brown's Neural Networks [playlist](https://www.3blue1brown.com/topics/neural-networks)
  * Watch Andrej Karpathy's lecture on [neural networks](https://youtu.be/VMj-3S1tku0) (it's okay if some of the exact backprop stuff doesn't make complete sense quite yet)
  * **TODO:** add questions from Anki on basic neural net concepts&#x20;
* Practice
  * [How Does a Neural Network Really Work](https://www.kaggle.com/code/jhoward/how-does-a-neural-net-really-work)
  * [Linear Model and Neural Net From Scratch](https://www.kaggle.com/code/jhoward/linear-model-and-neural-net-from-scratch)
  * **How to practice** (relevant for future sections in this page as well)
    * Run each cell and understand why it works. If you don't get it, ask GPT until you do. **Don't let your eyes glaze over and start skimming.**
      * Create a new cell that describes what the original cell does in comments. Include the basic functionality and hints for any particularly thorny implementation details as well as _why_.
      * Re-implement in your new cell&#x20;
    * Once you feel like you understand each cell, condense cells until each one represents a significant "chunk".&#x20;
      * Do the same process as above
    * Remove all hints and try to do the whole thing by yourself. At most, keep a bulleted list of all the high-level logical "chunks". &#x20;
    * Ideally, you want to now do the whole thing with new specifications (new dataset, slightly different architecture, etc).
  * (Recommended Bonus): go through the [fastbook version ](https://github.com/fastai/fastbook/blob/master/04\_mnist\_basics.ipynb)of this lesson. If you've already practiced extensively with the previous 2 notebooks, you can go through this relatively quickly and just understand each cell.&#x20;

</details>

<details>

<summary>Backprop</summary>

* Watch 3B1B's [backpropagation calculus](https://www.3blue1brown.com/lessons/backpropagation-calculus) (definitely read through the text after watching the video; it helps a lot with clarification)
  * Understand this (from Neel Nanda): backprop is just the chain rule on multivariate functions.
  * By now you should have a solid grok on backprop. Find other resources if you don't.&#x20;
* [Become a backprop ninja](https://www.youtube.com/watch?v=q8SA3rM6ckI) :).
  * You won't be able to do many of these yourself but try your best. Don't skip this because I think it really helps build intuition for how gradients "flow" through a neural net.

</details>

* [ ] **Go back to the** [**coding page**](coding.md) **and complete the rest of it.**&#x20;
* [ ] The Rest of Andrej Karpathy’s course: **add the best questions and exercises from Karpathy's lectures**&#x20;
  * [ ] https://www.youtube.com/watch?v=PaCmpygFfXo
    * [ ] Make sure you understand all of the Pytorch operations
    * [ ] Explain broadcasting
    * [ ] What is negative log-likelihood?
    * [ ] What is softmax?
    * [ ] What were the two different models trained in the video? What are the key differences? Why might you prefer the second over the first (even if they have near-identical results as of now)?
  * [ ] https://www.youtube.com/watch?v=TCH\_1BHY58I
    * [ ] Why do you split into train/dev/test splits? Roughly what proportions are standard?
    * [ ] Why do you use minibatches? This video builds good intuition to what 3b1b mentions here: [https://youtu.be/Ilg3gGewQ5U?t=613](https://youtu.be/Ilg3gGewQ5U?t=613).
    * [ ] How do you find a good learning rate?
  * [ ] https://youtu.be/P6sfmUTpUmc
    * [ ] Kaiming init
    * [ ] Batchnorm
      * [ ] Why do you even want to use batchnorm?
      * [ ] What is the batchnorm equation?
      * [ ] Why was batchnorm a breakthrough?
    * [ ] Why do you want to do something like layer.weight \*= 5/3?
    * [ ] Take note of the different visualizations. What is each of them supposed to tell you? What do they look like when things are good? What do they look like when things are broken?
      * [ ] Make sure you can reproduce the visualizations using whatever plotting library you've learned
  * [ ] https://youtu.be/q8SA3rM6ckI
    * [ ] Just go through this and make sure you understand all of it. Do all the exercises you can (if you’ve only been learning calc for the first time, you probably won’t be able to do the last two exercises yet, but that’s ok.)
  * [ ] https://youtu.be/t3YJ5hKiMQ0
    * [ ] Watch this, play around with the code. There’s nothing conceptually special, but it helps to watch.
