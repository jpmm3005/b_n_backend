---
title: Review of Calculus skills and Linear Algebra
date: 2025-08-18
---

# Overview: A peek under the hood

## Motivation: Why Matrices?

Matrix (Linear) Algebra is a powerful tool in Data Science because it is the underlying foundation for techniques such as...

## PCA (Principle Component Analysis)
 
As covered in lecture last week, PCA is a method to reduce the dimensionality of data while preserving its structure.


Condsider the following data frame

|GPA (UW)      | SAT Score | # of Submitted Applications | Acceptances|
| -------- | -------   | ----------|---------|
| 3.9  | 1510      |6         |5       |
| 4.0  | 1340      |10        |7       |
| 3.2  | 1590      |2         |2       |
| 2.0  | 1220       |1         |1       |


If we let $A$ be a $4 \times 4$ matrix composed of the Data listed above

$A = \begin{bmatrix}
3.9 & 1510 & 6 & 5\\ 
4.0 & 1340 & 10 & 7\\
3.2 & 1590 & 2 & 2\\
2.0 & 1220 & 1 & 1\\
\end{bmatrix}$

then, If we have some projection matrix $P$ 


$ P = \begin{bmatrix}
-0.001 & −0.0001\\
0.999 & −0.004\\
0.003 & 0.987\\
0.002 & 0.159
\end{bmatrix}$
 
<small>If you want to read m</small>.


Then, the multiplication $A \times P$ yields a new  $4 \times 2 $ matrix $X$ which can be visualized in lower dimensional space.

$X = \begin{bmatrix}
1508.5 & 0.67661\\
1338.7 & 5.6226\\
1588.4 & -4.0683\\
1218.8 & -3.7342
\end{bmatrix}$

[]()

