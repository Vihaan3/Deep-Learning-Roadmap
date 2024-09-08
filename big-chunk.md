# Big chunk

**Made this as a curriculum for school club. Get a lot more questions from what you have in Anki. Go through the programming deck and drop good questions here. Also, speedrun through all this content and make more questions. Create it in gitbook and put it up on your github.**

*   Coding

    In this order:

    * [ ] Get familiar w/ Python: https://exercism.org/tracks/python
    * [ ] Get familiar w/ Numpy: https://cs231n.github.io/python-numpy-tutorial/
    * [ ] Get familiar w/ Pytorch:
      * [ ] https://pytorch.org/tutorials/
      * [ ] https://pytorch.org/tutorials/beginner/blitz/neural\_networks\_tutorial.html
      * [ ] https://pytorch.org/tutorials/beginner/nn\_tutorial.html#refactor-using-nn-module
      * [ ] https://pytorch.org/tutorials/beginner/basics/intro.html
    * [ ] Getting better with tensors
      * [ ] Learn einops and einsum with this: https://arena3-chapter0-fundamentals.streamlit.app/\[0.0]\_Prerequisites
      * [ ] https://arena3-chapter0-fundamentals.streamlit.app/\[0.1]\_Ray\_Tracing
*   Basic Math

    **Note: These are all incredibly interesting on their own, and I generally did the full course for all of them, but if you just want to get through the prerequisites, (as far as I’ve seen) you usually need less than you think, and you can probably get other things when you need it.**

    * Linear Algebra (link all the specific videos and tutorials you would recommend + some practice problems and questions from Anki to see how well they grok it)
      * [ ] Basis
      * [ ] Change of basis
      * [ ] That a vector space is a geometric object that doesn’t necessarily have a canonical basis
      * [ ] That a matrix is a linear map between two vector spaces (or from a vector space to itself)
      * [ ] What’s singular value decomposition? Why is it useful?
        * [ ] \*\*\*\*https://www.youtube.com/watch?v=nbBvuuNVfco
      * [ ] What are orthogonal/orthonormal matrices, and how is changing to an orthonormal basis importantly different from just any change of basis?
      * [ ] What are eigenvalues and eigenvectors, and what do these tell you about a linear map?
      * [ ] Find matrix multiplication practice worksheets online and practice until it feels really easy
    *   Probability

        https://seeing-theory.brown.edu/basic-probability/index.html

        Make sure you somewhat grok most of this.
    *   Calculus

        Watch at least the first 7 chapters of [https://www.3blue1brown.com/topics/calculus](https://www.3blue1brown.com/topics/calculus)
*   Grokking the basics

    _**Add intuition questions.**_

    * [ ] Watch up to “backpropagation calculus” from [https://www.3blue1brown.com/topics/neural-networks](https://www.3blue1brown.com/topics/neural-networks)
    * [ ] Use this [fast.ai](http://fast.ai) lesson: [https://course.fast.ai/Lessons/lesson5.html](https://course.fast.ai/Lessons/lesson5.html) (try your best to understand everything other than backpropagation. It’s fine if that’s still fuzzy for you by the time you’re done. )
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
    * [ ] The Rest of Andrej Karpathy’s course
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
      * [ ] https://www.youtube.com/watch?v=kCc8FmEb1nY
        * [ ] Do the standard playing around for this
        * [ ] Understand the difference between encoder and decoder, self-attention vs cross attention, layernorm and batchnorm
        * [ ] Search up more about residual connections to get more intuition for why they actually work. You might get this right away, but for me it felt kind of unintuitive but really satisfying when I gained a mental model for it.
* Basic Tooling
  * [ ] Data Visualization
    * [ ] Get familiar with any plotting library
    * [ ] Find some online tutorials and play around for an hour or so
    * [ ] If you haven’t already done so, go back to Andrej Karpathy’s makemore 3 video, and do the visualizations from scratch.
* Beyond the Basics?
  * [ ] https://arena3-chapter0-fundamentals.streamlit.app/\[0.3]\_Optimization
  * [ ] https://arena3-chapter0-fundamentals.streamlit.app/\[0.2]_CNNs_&\_ResNets
  * [ ] https://arena3-chapter0-fundamentals.streamlit.app/\[0.5]_GANs_&\_VAEs
  * [ ] Explain attention from the perspective of two concurrent tokens _a_ and _b_ where a = "D" and b = "urs" and _b_ is attending to _a_.
