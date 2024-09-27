# Grokking the Basics

How to study: preferably batches of 2+ hours at a time rather than distributed but it's fine if distributed.

_**Add intuition questions. Potentially cop some from fastbook -> for each topic below: find the relevant section in the website -> find the relevant sections in the fastbook -> add here**_

* [ ] Watch up to “backpropagation calculus” from [https://www.3blue1brown.com/topics/neural-networks](https://www.3blue1brown.com/topics/neural-networks)
* [ ] Use this [fast.ai](http://fast.ai) lesson: [https://course.fast.ai/Lessons/lesson5.html](https://course.fast.ai/Lessons/lesson5.html) (try your best to understand everything other than backpropagation. It’s fine if that’s still fuzzy for you by the time you’re done.)
  * [ ] first watch the video without doing anything, and search up/use GPT for things you don’t understand.
  * [ ] Make copies of [https://www.kaggle.com/code/jhoward/how-does-a-neural-net-really-work](https://www.kaggle.com/code/jhoward/how-does-a-neural-net-really-work) and [https://www.kaggle.com/code/jhoward/linear-model-and-neural-net-from-scratch](https://www.kaggle.com/code/jhoward/linear-model-and-neural-net-from-scratch) and play around with them.
    * [ ] Run each cell and understand why it works.
      * [ ] Create a new cell that describes in plain English what the cell does
      * [ ] Delete the old cell and re-implement that functionality in your new cell
    * [ ] Once you feel like you understand each cell, condense cells until each one represents a significant portion of the training pipeline
      * [ ] Do the same process as the above
  * [ ] Bonus: read and play with [https://github.com/fastai/fastbook/blob/master/04\_mnist\_basics.ipynb](https://github.com/fastai/fastbook/blob/master/04\_mnist\_basics.ipynb)
* [ ] Watch [https://youtu.be/VMj-3S1tku0](https://youtu.be/VMj-3S1tku0) and follow along in a Jupyter notebook.
* [ ] Watch “backpropogation calculus” from 3b1b
* [ ] By now you should have a solid grok on backprop. Find other resources if you don’t.
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
      * [ ] Don’t worry about understanding the visualizations now. We’ll come back later
  * [ ] https://youtu.be/q8SA3rM6ckI
    * [ ] Just go through this and make sure you understand all of it. Do all the exercises you can (if you’ve only been learning calc for the first time, you probably won’t be able to do the last two exercises yet, but that’s ok.)
  * [ ] https://youtu.be/t3YJ5hKiMQ0
    * [ ] Watch this, play around with the code. There’s nothing conceptually special, but it helps to watch.
