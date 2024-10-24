# Transformers

How to study: preferably batches of 2+ hours at a time rather than distributed.&#x20;

Get a non-technical introduction to attention with this: [https://www.3blue1brown.com/lessons/gpt](https://www.3blue1brown.com/lessons/gpt) and this: [https://www.3blue1brown.com/lessons/attention](https://www.3blue1brown.com/lessons/attention). &#x20;

https://www.youtube.com/watch?v=kCc8FmEb1nY

* [ ] Do the standard playing around for this
* [ ] Understand the difference between encoder and decoder, self-attention vs cross attention, layernorm and batchnorm
* [ ] Search up more about residual connections to get more intuition for why they actually work. You might get this right away, but for me it felt kind of unintuitive but really satisfying when I gained a mental model for it.

Intuition question: Explain attention from the perspective of two concurrent tokens _a_ and _b_ where a = "The", b = "dog", and _b_ is attending to _a_.

Answer: There will be a high affinity score for the "look one position behind" query for token b. After matrix multiplication with the value matrix, token b ("dog") will have the added context that can be thought of as "I follow 'The' " (because the part of V that points to "I am one position after..." will match up with the query that says "look one position behind..."). So token b will now have the added context that it follows token a. Aka "dog" will have the added context that it follows "The".

[https://arena3-chapter1-transformer-interp.streamlit.app/%5B1.1%5D\_Transformer\_from\_Scratch](https://arena3-chapter1-transformer-interp.streamlit.app/\[1.1]\_Transformer\_from\_Scratch)\
\- speedrun through this again and add some comments on what exercises to do and what not to do if you've done the first. Add intuition questions. \
\
To the people doing this AI roadmap: Do the rest of mech interp as well if you find it interesting (which is really is) but it's not strictly necessary.&#x20;
