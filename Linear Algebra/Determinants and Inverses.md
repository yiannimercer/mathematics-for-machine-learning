|    Course Name     |          Topic          |   Date    | Tags |
| :----------------: | :---------------------: | :-------: | :--: |
| **Linear Algebra** | Determinants & Inverses | 7/14/2025 |      |
[Class Video Link](https://www.coursera.org/learn/linear-algebra-machine-learning/lecture/nK1Eb/determinants-and-inverses)

# Summary
While matrices can be described as something that transforms space, we can also use determinant and inverses of matrices through the lens of linearly independence to describe the scale transformations

# Key Takeaways
1. When the matrix scales the original unit matrix linearly and there's no volume enclosed in the new form, then the determinant would be 0

# Definitions
- Determinants: a scalar value calculated from the elements of a square matrix. It provides information about the matrix's properties, such as its invertibility and its effect on geometric transformations like scaling and orientation
	- You can think of it as measure how much the matrix has transformed when scaling it 


# Additional Resources
- Name the hyperlink in brackets then outside the brackets put the URL in parens

# Notes
## Determinants
### Area = Determinants
- When you have a general matrix, and  it turns the original unit square into a parallelogram like below 
$$
\begin{bmatrix}
a & b \\
c & d \\
\end{bmatrix}
$$

<p align="center">
  <img src="images/image1.png" width="200">
</p>
* The **area of this parallelogram** is **ad - bc**, which would be `|A| = ad - bc`, which is the **determinant of A** 
* With...
$$
A = \begin{bmatrix}
a & b \\
c & d \\
\end{bmatrix}
$$
* The determinant of A can be calculated as 
$$
\begin{bmatrix}
a & b \\
c & d \\
\end{bmatrix} *
\begin{bmatrix}
d & -b \\
-c & a \\
\end{bmatrix} 
$$
* Which equals out to...
$$
\begin{bmatrix}
ad - bc & 0 \\
0 & ad-bc \\
\end{bmatrix}
$$
### No Area = No Determinant
* When you have a matrix like below
$$
\begin{bmatrix}
1 & 2 \\
1 & 2 \\
\end{bmatrix}
$$
this transforms the line in the spaces linearly, and creates no volume, meaning no determinant, `|A| = 0`
<p align="center">
  <img src="images/image2.png" width="200">
</p>
## Inverses
* Inverse matrix let's you undo your transformations, where you can go from the new transformation to the original transformation
* Determinant = how much we grow space
* When determinant = 0, inverse does not exist, basis vectors are not linearly independent  