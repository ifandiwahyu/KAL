---
title: Transformasi Linier

---

# Transformasi Linier
## Buktikan bahwa transformasi linier
$$
\textbf{Soal}
$$

$$
\textbf{Tunjukkan bahwa transformasi linier} 
$$

$$
T : \mathbb{R}^2 \to \mathbb{R}^2
$$

$$
\textbf{yang didefinisikan oleh:}
$$

$$
A = \begin{bmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{bmatrix}
$$

$$
\textbf{adalah rotasi berlawanan arah jarum jam sebesar sudut \( \theta \).}
$$

$$
\textbf{Penyelesaian}
$$

$$
\textbf{Misalkan sebuah vektor \( \vec{v} \in \mathbb{R}^2 \) dapat dituliskan dalam koordinat polar sebagai:}
$$

$$
\vec{v} = (x, y) = (r\cos\alpha, r\sin\alpha)
$$

$$
\textbf{dengan:}
$$

$$
\textbf{$r = \|\vec{v}\| = \sqrt{x^2 + y^2}$ adalah panjang vektor}
$$

$$
\textbf{$\alpha$ adalah sudut antara vektor $\vec{v}$ dan sumbu-$x$ positif}
$$

$$
\textbf{Terapkan transformasi \( T \) terhadap \( \vec{v} \):}
$$
$$
\textbf{T($\vec{v}) = A \vec{v} $=}
$$

$$
\begin{bmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{bmatrix}
\begin{bmatrix}
r\cos\alpha \\
r\sin\alpha
\end{bmatrix}
$$

$$
= r \begin{bmatrix}
\cos\theta \cos\alpha - \sin\theta \sin\alpha \\
\sin\theta \cos\alpha + \cos\theta \sin\alpha
\end{bmatrix}
$$

$$
\textbf{Gunakan identitas trigonometri:}
$$

$$
\cos(\alpha + \theta) = \cos\alpha \cos\theta - \sin\alpha \sin\theta
$$

$$
\sin(\alpha + \theta) = \sin\alpha \cos\theta + \cos\alpha \sin\theta
$$

$$
\Rightarrow T(\vec{v}) = r \begin{bmatrix}
\cos(\alpha + \theta) \\
\sin(\alpha + \theta)
\end{bmatrix}
$$

$$
= (r \cos(\alpha + \theta), r \sin(\alpha + \theta))
$$

$$
\textbf{Transformasi linier \( T \) memutar vektor \( \vec{v} \) sebesar \( \theta \) berlawanan arah jarum jam terhadap titik asal. Oleh karena itu, matriks }
$$

$$
A = \begin{bmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{bmatrix}
$$

$$
\textbf{merepresentasikan transformasi rotasi dalam bidang \( \mathbb{R}^2 \).}
$$

$$
\textbf{Terbuki}
$$

