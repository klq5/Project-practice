# Least-squares Estimation Formulas

\[
\overrightarrow{x_i} = \begin{bmatrix} 1 & x_1^i & x_2^i & \cdots & x_m^i \end{bmatrix}
\]


\[
y_i \approx \vec{\beta}^\top \overrightarrow{x_i} = \beta_0 + \sum_{j=1}^m \beta_j x_j^i
\]

---

\[
y_i \approx \sum_{j = 0}^{n} \beta_j\times x_j^i=\vec{\beta}\cdot\vec{x}^i
\]


\[
\vec{\hat{\beta}} = \underset{\vec{\beta}}{\arg\min} L(D, \vec{\beta}) = \underset{\vec{\beta}}{\arg\min} \sum_{i = 1}^{n} (\vec{\beta}\cdot\vec{x}_i - y_i)^2
\]


\[
\begin{align}
L(D, \vec{\beta}) &= \lVert X\vec{\beta}-Y\rVert^2 \\
&= (X\vec{\beta}-Y)^{\mathrm{T}}(X\vec{\beta}-Y) \\
&= Y^{\mathrm{T}}Y - Y^{\mathrm{T}}X\vec{\beta}-\vec{\beta}^{\mathrm{T}}X^{\mathrm{T}}Y+\vec{\beta}^{\mathrm{T}}X^{\mathrm{T}}X\vec{\beta}
\end{align}
\]

---


\[
\begin{align}
\frac{\partial L(D, \vec{\beta})}{\partial \vec{\beta}} &= \frac{\partial (Y^{\mathrm{T}}Y - Y^{\mathrm{T}}X\vec{\beta}-\vec{\beta}^{\mathrm{T}}X^{\mathrm{T}}Y + \vec{\beta}^{\mathrm{T}}X^{\mathrm{T}}X\vec{\beta})}{\partial \vec{\beta}} \\
&= -2X^{\mathrm{T}}Y + 2X^{\mathrm{T}}X\vec{\beta}
\end{align}
\]

