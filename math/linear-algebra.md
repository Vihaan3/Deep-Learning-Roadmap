# Linear Algebra

<details>

<summary>Learn</summary>

I love 3Blue1Brown's [introduction to linear algebra](https://www.3blue1brown.com/topics/linear-algebra). Since it's relatively short, I'd recommend just watching the whole thing through.&#x20;

By the end, make sure you can answer the following questions.

* From Neel Nanda
  * What is a basis?
  * Does a vector space necessarily have a canonical basis?
  * Understand that a matrix is a linear map between two vector spaces (or from a vector space to itself)
  * What are orthogonal/orthonormal matrices, and how is changing to an orthonormal basis importantly different from just any change of basis?
  * What are eigenvalues and eigenvectors, and what do these tell you about a linear map?
* From me
  * When is a transformation linear?
  * What is the idea of duality in vectors in linear algebra?
  * How can the change of basis be described?
  * Use what you know about linear combinations to explain why matrix multiplication works.
  * If a matrix is encoding a transformation, what does it mean to multiply it by a vector?
  * How would you represent a transformation in an alternative coordinate system, in the "language" of the alternative coordinate system?

</details>

<details>

<summary>Practice</summary>

[https://www.madasmaths.com/archive\_maths\_booklets\_further\_topics\_linear\_algebra.html](https://www.madasmaths.com/archive_maths_booklets_further_topics_linear_algebra.html)

Answers to the questions in the last section:

* Lines stay straight + origin doesn't move
* The coordinates of a vector encode a transformation from whatever dimension it's in to 1 dimension on the line of its arrow if you "tip" the vector on its side to form a matrix. This means that the transformation is equal to the dot product with that vector.
* As a linear transformation, where the matrix is the coordinates of the new basis vectors.
* Vectors are always linear combinations (scale and add) of the basis vectors. When you do a transformation, you're changing the basis vectors, so the coordinates of the vector are instructions for how to scale the basis vectors. Just like before, the x value should scale by the x basis vector and the y value should scale by the y basis vector. That's why the "flip" happens.
* You are applying the transformation to that vector.
* Matrix multiply the basis vectors of the other system in our "language" by the transformation in our "language". This will give you the transformation in our "language". Then, matrix multiply by the inverse of the basis vector matrix. This will translate the transformation to the other system.

</details>

Optional (but **highly** recommended): Go back and read through [this wonderful introduction](https://quantum.country/) to quantum computing. It's been designed with spaced repetition at its core. While learning about quantum computing, you will also understand how experts use spaced repetition to learn technical topics effectively.&#x20;
