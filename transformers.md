# Transformers

* Get a non-technical introduction to attention with 3B1B with these two videos: [https://www.3blue1brown.com/lessons/gpt](https://www.3blue1brown.com/lessons/gpt), [https://www.3blue1brown.com/lessons/attention](https://www.3blue1brown.com/lessons/attention). &#x20;
* [Andrej Karpathy Transformers](https://www.youtube.com/watch?v=kCc8FmEb1nY)
  * Be able to answer all of [these questions](https://jacobgw.com/blog/tft/2024/05/12/srs-intuit.html)
  * Understand the differences between:
    * encoder and decoder, self-attention vs cross attention, layernorm and batchnorm
  * Search up more about residual connections to get more intuition for why they actually work. You might get this right away, but for me it felt kind of unintuitive but really satisfying when I gained a mental model for it.
    * Ans: Because of the way that gradients flow (recall that + is a "distributor"), the network will learn to have the new layer as edits to the last layer rather than creating an entirely new representation.&#x20;
  * Explain attention from the perspective of two concurrent tokens _a_ and _b_ where a = "The", b = "dog", and _b_ is attending to _a_.
    * Answer: There will be a high affinity score for the "look one position behind" query for token b. After matrix multiplication with the value matrix, token b ("dog") will have the added context that can be thought of as "I follow 'The' " (because the part of V that points to "I am one position after..." will match up with the query that says "look one position behind..."). So token b will now have the added context that it follows token a. In other words, "dog" will have the added context that it follows "The".
* [https://arena3-chapter1-transformer-interp.streamlit.app/%5B1.1%5D\_Transformer\_from\_Scratch](https://arena3-chapter1-transformer-interp.streamlit.app/\[1.1]\_Transformer\_from\_Scratch)&#x20;
  * **TODO:** redo this&#x20;
  * To the people doing this AI roadmap: Do the rest of mech interp as well if you find it interesting (which is really is) but it's not strictly necessary.&#x20;
