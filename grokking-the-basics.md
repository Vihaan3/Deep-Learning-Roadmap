# Grokking the Basics

<details>

<summary>Get familiar w/ any plotting library</summary>

* I would recommend Plotly
  * If you're interested in Plotly, see [this](https://www.perfectlynormal.co.uk/blog-plotly-widgets) and play around for an hour or so while using Anki to memorize all the basics

</details>

<details>

<summary>Neural Networks</summary>

* Videos
  * Watch up to (but not including) “backpropagation calculus” from 3Blue1Brown's Neural Networks [playlist](https://www.3blue1brown.com/topics/neural-networks)
  * Watch fast.ai's [lesson on neural networks](https://course.fast.ai/Lessons/lesson5.html):  (try your best to understand everything other than backpropagation. It’s fine if that’s still fuzzy for you by the time you’re done.)
    * search up/use GPT for things you don’t understand but just passively watch the video for now
  * **TODO:** add questions from Anki for both of the above
* Practice
  * [How Does a Neural Network Really Work](https://www.kaggle.com/code/jhoward/how-does-a-neural-net-really-work)
  * [Linear Model and Neural Net From Scratch](https://www.kaggle.com/code/jhoward/linear-model-and-neural-net-from-scratch)
  * **How to practice** (relevant for future sections in this page as well)
    * First, run each cell and understand why it works. If you don't get it, ask&#x20;

</details>

<details>

<summary></summary>



</details>





* [ ] Run each cell and understand why it works.
  * [ ] Create a new cell that describes in plain English what the cell does
  * [ ] Delete the old cell and re-implement that functionality in your new cell
* [ ] Once you feel like you understand each cell, condense cells until each one represents a significant portion of the training pipeline
  * [ ] Do the same process as the above
* [ ] Bonus: read and play with [https://github.com/fastai/fastbook/blob/master/04\_mnist\_basics.ipynb](https://github.com/fastai/fastbook/blob/master/04\_mnist\_basics.ipynb)
* [ ] Watch [https://youtu.be/VMj-3S1tku0](https://youtu.be/VMj-3S1tku0) and follow along in a Jupyter notebook.
* [ ] Watch “backpropogation calculus” from 3b1b
* [ ] By now you should have a solid grok on backprop. Find other resources if you don’t.
* [ ] Neel Nanda: The intuition for what backprop is - in particular, grokking the idea that backprop is just the chain rule on multivariate functions
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
