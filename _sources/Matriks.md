---
title: Matriks

---

# Matriks
## Determinan Matriks

Determinan matriks adalah suatu nilai skalar yang dapat dihitung dari elemen-elemen sebuah matriks persegi (matriks dengan jumlah baris dan kolom yang sama). Determinan memiliki banyak aplikasi dalam aljabar linear, termasuk dalam mencari invers matriks, menyelesaikan sistem persamaan linear, dan menentukan apakah suatu matriks memiliki solusi unik.
### Minor matriks
Minor suatu elemen dalam matriks adalah determinan dari submatriks yang diperoleh dengan menghapus satu baris dan satu kolom tempat elemen tersebut berada.

Minor ini digunakan dalam berbagai perhitungan dalam aljabar linear, termasuk dalam kofaktor, determinan, dan invers matriks.
### Cofaktor Matriks
kofaktor matriks adalah matriks yang memiliki elemen-elemen yang di dalamnya juga disebut kofaktor.
### Mencari determinan dengan konsep minor dan cofactor matriks. 
* Contoh matriks 3x3
Misalkan kita memiliki matriks $A$ sebagai berikut:
$$
A =
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{bmatrix}
$$
Kita akan menghitung determinan menggunakan ekspansi kofaktor berdasarkan baris pertama:
$$
\det(A) = a_{11}C_{11} + a_{12}C_{12} + a_{13}C_{13}
$$
di mana $C_{ij} = (-1)^{i+j} M_{ij}$ adalah kofaktor dari elemen $a_{ij}$, dan $M_{ij}$ adalah minor dari elemen tersebut.
$$
\textbf{Menghitung Minor dan Kofaktor}
$$
$$
\textbf{Minor dan Kofaktor untuk $a_{11} = 1$}
$$
$$
M_{11} =
\begin{vmatrix}
5 & 6 \\
8 & 9
\end{vmatrix}
= (5 \times 9 - 6 \times 8) = 45 - 48 = -3
$$
$$
C_{11} = (-1)^{1+1} M_{11} = (-1)^2 (-3) = -3
$$
$$
\textbf{Minor dan Kofaktor untuk $a_{12} = 2$}
$$
$$
M_{12} =
\begin{vmatrix}
4 & 6 \\
7 & 9
\end{vmatrix}
= (4 \times 9 - 6 \times 7) = 36 - 42 = -6
$$
$$
C_{12} = (-1)^{1+2} M_{12} = (-1)^3 (-6) = 6
$$
$$
\textbf{Minor dan Kofaktor untuk $a_{13} = 3$}
$$
$$
M_{13} =
\begin{vmatrix}
4 & 5 \\
7 & 8
\end{vmatrix}
= (4 \times 8 - 5 \times 7) = 32 - 35 = -3
$$
$$
C_{13} = (-1)^{1+3} M_{13} = (-1)^4 (-3) = -3
$$
$$
\textbf{Menghitung Determinan}
$$
$$
\det(A) = (1 \times -3) + (2 \times 6) + (3 \times -3)
$$
$$
= -3 + 12 - 9 = 0
$$
Jadi, determinan dari matriks $A$ adalah:
$$
\det(A) = 0
$$
Karena determinan nol, matriks ini $\textbf{singular}$ dan tidak memiliki invers.

* Contoh matriks 4x4 
Misalkan kita memiliki matriks $A$ sebagai berikut:
$$
A =
\begin{bmatrix}
1 & 2 & 3 & 4 \\
5 & 6 & 7 & 8 \\
9 & 10 & 11 & 12 \\
13 & 14 & 15 & 16
\end{bmatrix}
$$
Kita akan menghitung determinan menggunakan ekspansi kofaktor berdasarkan baris pertama:
$$
\det(A) = a_{11}C_{11} + a_{12}C_{12} + a_{13}C_{13} + a_{14}C_{14}
$$
di mana $C_{ij} = (-1)^{i+j} M_{ij}$ adalah kofaktor dari elemen $a_{ij}$, dan $M_{ij}$ adalah minor dari elemen tersebut.
$$
\textbf{Menghitung Minor dan Kofaktor}
$$
$$
\textbf{Minor dan Kofaktor untuk $a_{11} = 1$}
$$
$$
M_{11} =
\begin{vmatrix}
6 & 7 & 8 \\
10 & 11 & 12 \\
14 & 15 & 16
\end{vmatrix}
$$
Menghitung determinan minor $M_{11}$:


$$
\det(M_{11}) =
6 \left| \begin{matrix} 11 & 12 \\ 15 & 16 \end{matrix} \right|
-7 \left| \begin{matrix} 10 & 12 \\ 14 & 16 \end{matrix} \right|
+8 \left| \begin{matrix} 10 & 11 \\ 14 & 15 \end{matrix} \right|
$$
$$
= 6(11 \times 16 - 12 \times 15) - 7(10 \times 16 - 12 \times 14) + 8(10 \times 15 - 11 \times 14)
$$
$$
= 6(-4) - 7(-8) + 8(-4)
$$
$$
= -24 + 56 - 32 = 0
$$
$$
C_{11} = (-1)^{1+1} M_{11} = 0
$$
$$
\textbf{Minor dan Kofaktor untuk $a_{12} = 2$}
$$
$$
M_{12} =
\begin{vmatrix}
5 & 7 & 8 \\
9 & 11 & 12 \\
13 & 15 & 16
\end{vmatrix}
$$
$$
C_{12} = (-1)^{1+2} M_{12} = 0
$$
$$
\textbf{Minor dan Kofaktor untuk $a_{13} = 3$}
$$
$$
M_{13} =
\begin{vmatrix}
5 & 6 & 8 \\
9 & 10 & 12 \\
13 & 14 & 16
\end{vmatrix}
$$
$$
C_{13} = (-1)^{1+3} M_{13} = 0
$$
$$
\textbf{Minor dan Kofaktor untuk $a_{14} = 4$}
$$
$$
M_{14} =
\begin{vmatrix}
5 & 6 & 7 \\
9 & 10 & 11 \\
13 & 14 & 15
\end{vmatrix}
$$
$$
C_{14} = (-1)^{1+4} M_{14} = 0
$$
$$
\textbf{Menghitung Determinan}
$$
$$
\det(A) = (1 \times 0) + (2 \times 0) + (3 \times 0) + (4 \times 0) = 0
$$
Jadi, determinan dari matriks $A$ adalah:
$$
\det(A) = 0
$$

Karena determinan nol, matriks ini $\textbf{singular}$ dan tidak memiliki invers.

* Contoh matriks 5x5
Misalkan kita memiliki matriks $A$ sebagai berikut:
$$
A =
\begin{bmatrix}
1 & 2 & 3 & 4 & 5 \\
6 & 7 & 8 & 9 & 10 \\
11 & 12 & 13 & 14 & 15 \\
16 & 17 & 18 & 19 & 20 \\
21 & 22 & 23 & 24 & 25
\end{bmatrix}

Kita akan menghitung determinan menggunakan ekspansi kofaktor berdasarkan baris pertama:
$$
\det(A) = a_{11}C_{11} + a_{12}C_{12} + a_{13}C_{13} + a_{14}C_{14} + a_{15}C_{15}
$$
di mana $C_{ij} = (-1)^{i+j} M_{ij}$ adalah kofaktor dari elemen $a_{ij}$, dan $M_{ij}$ adalah minor dari elemen tersebut.
$$
\textbf{Menghitung Minor dan Kofaktor}
$$
$$
\textbf{Minor dan Kofaktor untuk $a_{11} = 1$}
$$
$$
M_{11} =
\begin{vmatrix}
7 & 8 & 9 & 10 \\
12 & 13 & 14 & 15 \\
17 & 18 & 19 & 20 \\
22 & 23 & 24 & 25
\end{vmatrix}
$$
Menghitung determinan minor $M_{11}$:
$$
\det(M_{11}) = 0
$$
$$
C_{11} = (-1)^{1+1} M_{11} = 0
$$
$$
\textbf{Minor dan Kofaktor untuk $a_{12} = 2$}
$$
$$
M_{12} =
\begin{vmatrix}
6 & 8 & 9 & 10 \\
11 & 13 & 14 & 15 \\
16 & 18 & 19 & 20 \\
21 & 23 & 24 & 25
\end{vmatrix}
$$
$$
C_{12} = (-1)^{1+2} M_{12} = 0
$$
$$
\textbf{Minor dan Kofaktor untuk $a_{13} = 3$}
$$
$$
M_{13} =
\begin{vmatrix}
6 & 7 & 9 & 10 \\
11 & 12 & 14 & 15 \\
16 & 17 & 19 & 20 \\
21 & 22 & 24 & 25
\end{vmatrix}
$$
$$
C_{13} = (-1)^{1+3} M_{13} = 0
$$
$$
\textbf{Minor dan Kofaktor untuk $a_{14} = 4$}
$$
$$
M_{14} =
\begin{vmatrix}
6 & 7 & 8 & 10 \\
11 & 12 & 13 & 15 \\
16 & 17 & 18 & 20 \\
21 & 22 & 23 & 25
\end{vmatrix}
$$
$$
C_{14} = (-1)^{1+4} M_{14} = 0
$$
$$
\textbf{Minor dan Kofaktor untuk $a_{15} = 5$}
$$
$$
M_{15} =
\begin{vmatrix}
6 & 7 & 8 & 9 \\
11 & 12 & 13 & 14 \\
16 & 17 & 18 & 19 \\
21 & 22 & 23 & 24
\end{vmatrix}
$$
$$
C_{15} = (-1)^{1+5} M_{15} = 0
$$
$$
\textbf{Menghitung Determinan}
$$
$$
\det(A) = (1 \times 0) + (2 \times 0) + (3 \times 0) + (4 \times 0) + (5 \times 0) = 0
$$
Jadi, determinan dari matriks $A$ adalah:
$$
\det(A) = 0
$$
Karena determinan nol, matriks ini $\textbf{singular}$ dan tidak memiliki invers.
