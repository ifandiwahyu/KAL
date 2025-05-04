## Bukti Transformasi Linear Rotasi Bidang

**Soal:**  
Tunjukkan bahwa transformasi linear \( T: \mathbb{R}^2 \rightarrow \mathbb{R}^2 \) yang dinyatakan oleh matriks:

\[
A = \begin{bmatrix}
\cos \theta & -\sin \theta \\
\sin \theta & \cos \theta
\end{bmatrix}
\]

merupakan rotasi terhadap asal koordinat sebesar sudut \( \theta \) berlawanan arah jarum jam.

---

### Solusi:

Misalkan sebuah vektor \( \vec{v} = (x, y) \) dinyatakan dalam koordinat polar:

\[
\vec{v} = (x, y) = (r \cos \alpha, r \sin \alpha)
\]

dengan:
- \( r = \|\vec{v}\| \) adalah panjang vektor,
- \( \alpha \) adalah sudut antara vektor dengan sumbu-x positif.

Transformasi \( T \) adalah:

\[
T(\vec{v}) = A \cdot \vec{v} = \begin{bmatrix}
\cos \theta & -\sin \theta \\
\sin \theta & \cos \theta
\end{bmatrix} \cdot \begin{bmatrix}
r \cos \alpha \\
r \sin \alpha
\end{bmatrix}
\]

Hitung hasil kali matriks:

\[
T(\vec{v}) =
\begin{bmatrix}
r (\cos \theta \cos \alpha - \sin \theta \sin \alpha) \\
r (\sin \theta \cos \alpha + \cos \theta \sin \alpha)
\end{bmatrix}
\]

Gunakan identitas trigonometri:

- \( \cos(\alpha + \theta) = \cos \alpha \cos \theta - \sin \alpha \sin \theta \)
- \( \sin(\alpha + \theta) = \sin \alpha \cos \theta + \cos \alpha \sin \theta \)

Maka:

\[
T(\vec{v}) =
\begin{bmatrix}
r \cos(\alpha + \theta) \\
r \sin(\alpha + \theta)
\end{bmatrix}
\]

Ini adalah koordinat polar dari vektor dengan panjang tetap \( r \), tetapi sudutnya berubah menjadi \( \alpha + \theta \), yaitu diputar sebesar \( \theta \) berlawanan arah jarum jam.

---

### Kesimpulan:

Transformasi linear yang dinyatakan oleh matriks:

\[
\begin{bmatrix}
\cos \theta & -\sin \theta \\
\sin \theta & \cos \theta
\end{bmatrix}
\]

merupakan rotasi bidang \( \mathbb{R}^2 \) terhadap titik asal sejauh sudut \( \theta \), berlawanan arah jarum jam.
