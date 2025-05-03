---
title: Penyelesaian Sistem Persamaan Linear dengan Eliminasi Baris Elementer

---

# Matriks Baris Elementer
## Penyelesaian Sistem Persamaan Linear dengan Eliminasi Baris Elementer

#### Diketahui sistem persamaan:
$$
\begin{array}
-7x_1 - 6x_2 - 12x_3 = -33 \\
5x_1 + 5x_2 + 7x_3 = 24 \\
x_1 + 4x_3 = 5
\end{array}
$$

Matriks yang sesuai:
$$
A = \begin{bmatrix} -7 & -6 & -12 \\ 5 & 5 & 7 \\ 1 & 0 & 4 \end{bmatrix}, \quad
b = \begin{bmatrix} -33 \\ 24 \\ 5 \end{bmatrix}
\
$$

Matriks augmented:
$$
\left[
\begin{array}{ccc|c}
-7 & -6 & -12 & -33 \\
5 & 5 & 7 & 24 \\
1 & 0 & 4 & 5
\end{array}
\right]
$$
$$
\textbf{Langkah 1: Tukar} R_1 \leftrightarrow R_3$$
$$
\left[
\begin{array}{ccc|c}
1 & 0 & 4 & 5 \\
5 & 5 & 7 & 24 \\
-7 & -6 & -12 & -33
\end{array}
\right]
$$

$$
\textbf{Langkah 2: Eliminasi elemen di bawah pivot pertama}$$
$$
R_2 \to R_2 - 5R_1, \quad R_3 \to R_3 + 7R_1
$$
$$
\left[
\begin{array}{ccc|c}
1 & 0 & 4 & 5 \\
0 & 5 & -13 & -1 \\
0 & -6 & 16 & 2
\end{array}
\right]
$$

$$\textbf{Langkah 3: Buat elemen (2,2) menjadi 1}$$
$$
R_2 \to \frac{1}{5} R_2
$$
$$
\left[
\begin{array}{ccc|c}
1 & 0 & 4 & 5 \\
0 & 1 & -\frac{13}{5} & -\frac{1}{5} \\
0 & -6 & 16 & 2
\end{array}
\right]
$$

$$\textbf{Langkah 4: Eliminasi elemen di bawah (3,2)}$$
$$
R_3 \to R_3 + 6R_2
$$
$$
\left[
\begin{array}{ccc|c}
1 & 0 & 4 & 5 \\
0 & 1 & -\frac{13}{5} & -\frac{1}{5} \\
0 & 0 & \frac{18}{5} & \frac{4}{5}
\end{array}
\right]
$$

$$\textbf{Langkah 5: Buat elemen (3,3) menjadi 1}$$
$$
R_3 \to \frac{5}{18} R_3
$$
$$
\left[
\begin{array}{ccc|c}
1 & 0 & 4 & 5 \\
0 & 1 & -\frac{13}{5} & -\frac{1}{5} \\
0 & 0 & 1 & \frac{2}{9}
\end{array}
\right]
$$

$$\textbf{Langkah 6: Eliminasi elemen di atas (3,3)}$$
$$
R_2 \to R_2 + \frac{13}{5} R_3, \quad R_1 \to R_1 - 4R_3
$$
$$
\left[
\begin{array}{ccc|c}
1 & 0 & 0 & \frac{41}{9} \\
0 & 1 & 0 & -\frac{11}{9} \\
0 & 0 & 1 & \frac{2}{9}
\end{array}
\right]
$$

$$\textbf{Hasil solusi:}$$
$$
x_1 = \frac{41}{9}, \quad x_2 = -\frac{11}{9}, \quad x_3 = \frac{2}{9}
$$