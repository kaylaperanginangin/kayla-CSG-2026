## TASK 1 — Bilangan Kompleks

Diketahui:
$$
z_1=1+i,\qquad z_2=\sqrt3-i
$$

### 1.1 Operasi bilangan kompleks

a. Penjumlahan
$$
\begin{aligned}
z_1+z_2
&=(1+i)+(\sqrt3-i)\\
&=1+\sqrt3+i-i\\
&=\boxed{1+\sqrt3}
\end{aligned}
$$

b. Perkalian
$$
\begin{aligned}
z_1z_2
&=(1+i)(\sqrt3-i)\\
&=\sqrt3-i+i\sqrt3-i^2\\
&=\sqrt3+1+i(\sqrt3-1)
\end{aligned}
$$
$$
\boxed{z_1z_2=(\sqrt3+1)+(\sqrt3-1)i}
$$

c. Konjugat
$$
z_1=1+i
$$
$$
\boxed{z_1^*=1-i}
$$

d. Pembagian
$$
\begin{aligned}
\frac{z_1}{z_2}
&=\frac{1+i}{\sqrt3-i}
\times\frac{\sqrt3+i}{\sqrt3+i}\\
&=\frac{(1+i)(\sqrt3+i)}{(\sqrt3)^2-i^2}\\
&=\frac{\sqrt3-1+(1+\sqrt3)i}{3+1}
\end{aligned}
$$
$$
\boxed{
\frac{z_1}{z_2}
=\frac{\sqrt3-1}{4}
+\frac{1+\sqrt3}{4}i
}
$$

### 1.2 Menghitung modulus

Rumus:
$$
|z|=\sqrt{a^2+b^2}
$$

a. Modulus $z_1$
$$
\begin{aligned}
|z_1|
&=\sqrt{1^2+1^2}\\
&=\boxed{\sqrt2}
\end{aligned}
$$

b. Modulus $z_2$
$$
\begin{aligned}
|z_2|
&=\sqrt{(\sqrt3)^2+(-1)^2}\\
&=\sqrt{3+1}\\
&=\boxed{2}
\end{aligned}
$$

c. Modulus $z_1z_2$
$$
\begin{aligned}
|z_1z_2|
&=\sqrt{(\sqrt3+1)^2+(\sqrt3-1)^2}\\
&=\sqrt{(4+2\sqrt3)+(4-2\sqrt3)}\\
&=\sqrt8\\
&=\boxed{2\sqrt2}
\end{aligned}
$$

Verifikasi:
$$
\begin{aligned}
|z_1||z_2|
&=\sqrt2(2)\\
&=2\sqrt2
\end{aligned}
$$
$$
\boxed{|z_1z_2|=|z_1||z_2|}
$$

### 1.3 Bentuk polar

Rumus:
$$
z=re^{i\theta}
$$

a. $z_1=1+i$
$$
r_1=\sqrt{1^2+1^2}=\sqrt2
$$
$$
\theta_1=\tan^{-1}\left(\frac11\right)
=\frac{\pi}{4}
$$
$$
\boxed{z_1=\sqrt2e^{i\pi/4}}
$$

b. $z_2=\sqrt3-i$
$$
r_2=\sqrt{3+1}=2
$$
$$
\theta_2=\tan^{-1}\left(\frac{-1}{\sqrt3}\right)
=-\frac{\pi}{6}
$$
$$
\boxed{z_2=2e^{-i\pi/6}}
$$

### 1.4 Menghitung $z_1^8$

Menggunakan teorema De Moivre:
$$
(re^{i\theta})^n=r^ne^{in\theta}
$$
$$
\begin{aligned}
z_1^8
&=(\sqrt2e^{i\pi/4})^8\\
&=(\sqrt2)^8e^{i2\pi}\\
&=16(\cos2\pi+i\sin2\pi)\\
&=16(1+0i)
\end{aligned}
$$
$$
\boxed{z_1^8=16}
$$

### 1.5 Membuktikan $|e^{i\theta}|^2=1$

Berdasarkan formula Euler:
$$
e^{i\theta}=\cos\theta+i\sin\theta
$$
$$
\begin{aligned}
|e^{i\theta}|^2
&=|\cos\theta+i\sin\theta|^2\\
&=\cos^2\theta+\sin^2\theta\\
&=1
\end{aligned}
$$
$$
\boxed{|e^{i\theta}|^2=1}
$$

---

## TASK 2 — State, Inner Product, & Normalisasi

Diketahui:
$$
|a\rangle=
\begin{pmatrix}1\\2i\end{pmatrix},
\quad
|b\rangle=
\begin{pmatrix}2\\-i\end{pmatrix}
$$
$$
|c\rangle=
\frac12|0\rangle+
\frac{\sqrt3}{2}e^{i\pi/4}|1\rangle
$$

### 2.1 Mencari bra $\langle a|$ dan $\langle b|$

Rumus:
$$
\langle\psi|=(|\psi\rangle^\dagger)
$$

a. 
$$
|a\rangle=
\begin{pmatrix}1\\2i\end{pmatrix}
$$
Transpose dan konjugasi:
$$
\boxed{\langle a|=\begin{pmatrix}1&-2i\end{pmatrix}}
$$

b. 
$$
|b\rangle=
\begin{pmatrix}2\\-i\end{pmatrix}
$$
$$
\boxed{\langle b|=\begin{pmatrix}2&i\end{pmatrix}}
$$

### 2.2 Menghitung inner product

a. $\langle a|b\rangle$
$$
\begin{aligned}
\langle a|b\rangle
&=\begin{pmatrix}1&-2i\end{pmatrix}
\begin{pmatrix}2\\-i\end{pmatrix}\\
&=2+2i^2\\
&=2-2\\
&=\boxed{0}
\end{aligned}
$$

b. $\langle b|a\rangle$
$$
\begin{aligned}
\langle b|a\rangle
&=\begin{pmatrix}2&i\end{pmatrix}
\begin{pmatrix}1\\2i\end{pmatrix}\\
&=2+2i^2\\
&=2-2\\
&=\boxed{0}
\end{aligned}
$$

Verifikasi:
$$
\langle a|b\rangle
=\langle b|a\rangle^*
$$
$$
\boxed{0=0^*}
$$

### 2.3 Menentukan ortogonalitas

Syarat ortogonal:
$$
\langle a|b\rangle=0
$$
Dari hasil 2.2:
$$
\boxed{|a\rangle\perp|b\rangle}
$$

### 2.4 Normalisasi state

Rumus:
$$
\|\psi\|=\sqrt{\langle\psi|\psi\rangle}
$$
$$
|\psi_{\text{norm}}\rangle
=\frac{|\psi\rangle}{\|\psi\|}
$$

a. Normalisasi $|a\rangle$
$$
\begin{aligned}
\|a\|
&=\sqrt{(1)(1)+(-2i)(2i)}\\
&=\sqrt{1-4i^2}\\
&=\sqrt5
\end{aligned}
$$
Maka:
$$
\boxed{
|a_{\text{norm}}\rangle
=\frac1{\sqrt5}
\begin{pmatrix}1\\2i\end{pmatrix}
}
$$
Verifikasi:
$$
\frac15+\frac45=1
$$

b. Normalisasi $|b\rangle$
$$
\begin{aligned}
\|b\|
&=\sqrt{(2)(2)+(i)(-i)}\\
&=\sqrt{4-i^2}\\
&=\sqrt5
\end{aligned}
$$
Maka:
$$
\boxed{
|b_{\text{norm}}\rangle
=\frac1{\sqrt5}
\begin{pmatrix}2\\-i\end{pmatrix}
}
$$
Verifikasi:
$$
\frac45+\frac15=1
$$

### 2.5 Normalisasi $|c\rangle$ dan probabilitas

Diketahui:
$$
|c\rangle=
\frac12|0\rangle+
\frac{\sqrt3}{2}e^{i\pi/4}|1\rangle
$$

a. Memeriksa normalisasi
$$
\begin{aligned}
\langle c|c\rangle
&=\left|\frac12\right|^2+
\left|\frac{\sqrt3}{2}e^{i\pi/4}\right|^2\\
&=\frac14+\frac34|e^{i\pi/4}|^2\\
&=\frac14+\frac34(1)\\
&=\boxed{1}
\end{aligned}
$$
Jadi state sudah ternormalisasi.

b. Probabilitas $P(0)$
$$
\begin{aligned}
P(0)
&=|\langle0|c\rangle|^2\\
&=\left|\frac12\right|^2\\
&=\boxed{\frac14=25\%}
\end{aligned}
$$

c. Probabilitas $P(1)$
$$
\begin{aligned}
P(1)
&=|\langle1|c\rangle|^2\\
&=\left|\frac{\sqrt3}{2}e^{i\pi/4}\right|^2\\
&=\frac34(1)\\
&=\boxed{\frac34=75\%}
\end{aligned}
$$

Verifikasi:
$$
P(0)+P(1)=\frac14+\frac34=1
$$

### 2.6 Mengubah ke Hadamard basis dan menghitung probabilitas

Diketahui:
$$
|+\rangle=\frac1{\sqrt2}
\begin{pmatrix}1\\1\end{pmatrix}
$$
$$
|-\rangle=\frac1{\sqrt2}
\begin{pmatrix}1\\-1\end{pmatrix}
$$

Koefisien:
$$
c_+=\langle+|c\rangle
$$
$$
\begin{aligned}
c_+
&=\frac1{\sqrt2}
\left(\frac12+\frac{\sqrt3}{2}e^{i\pi/4}\right)\\
&=\boxed{\frac{1+\sqrt3e^{i\pi/4}}{2\sqrt2}}
\end{aligned}
$$

Koefisien kedua:
$$
c_-=\langle-|c\rangle
$$
$$
\begin{aligned}
c_-
&=\frac1{\sqrt2}
\left(\frac12-\frac{\sqrt3}{2}e^{i\pi/4}\right)\\
&=\boxed{\frac{1-\sqrt3e^{i\pi/4}}{2\sqrt2}}
\end{aligned}
$$

Maka:
$$
\boxed{
|c\rangle=
\frac{1+\sqrt3e^{i\pi/4}}{2\sqrt2}|+\rangle
+
\frac{1-\sqrt3e^{i\pi/4}}{2\sqrt2}|-\rangle
}
$$

a. Menghitung $P(+)$
$$
\begin{aligned}
P(+)
&=|c_+|^2\\
&=\frac18|1+\sqrt3e^{i\pi/4}|^2\\
&=\frac18\left(1+3+2\sqrt3\cos\frac\pi4\right)\\
&=\frac18(4+\sqrt6)
\end{aligned}
$$
$$
\boxed{P(+)=\frac{4+\sqrt6}{8}\approx80{,}62\%}
$$

b. Menghitung $P(-)$
$$
\begin{aligned}
P(-)
&=|c_-|^2\\
&=\frac18|1-\sqrt3e^{i\pi/4}|^2\\
&=\frac18\left(1+3-2\sqrt3\cos\frac\pi4\right)\\
&=\frac18(4-\sqrt6)
\end{aligned}
$$
$$
\boxed{P(-)=\frac{4-\sqrt6}{8}\approx19{,}38\%}
$$

Verifikasi:
$$
\begin{aligned}
P(+)+P(-)
&=\frac{4+\sqrt6}{8}+\frac{4-\sqrt6}{8}\\
&=\frac88\\
&=\boxed{1}
\end{aligned}
$$

### 2.7 Membuktikan Hadamard basis ortonormal

Syarat:
$$
\langle e_i|e_j\rangle=\delta_{ij}
$$

a. 
$$
\begin{aligned}
\langle+|+\rangle
&=\frac12(1\quad1)
\begin{pmatrix}1\\1\end{pmatrix}\\
&=\frac12(1+1)\\
&=\boxed{1}
\end{aligned}
$$

b. 
$$
\begin{aligned}
\langle- |-\rangle
&=\frac12(1\quad-1)
\begin{pmatrix}1\\-1\end{pmatrix}\\
&=\frac12(1+1)\\
&=\boxed{1}
\end{aligned}
$$

c. 
$$
\begin{aligned}
\langle+|-\rangle
&=\frac12(1\quad1)
\begin{pmatrix}1\\-1\end{pmatrix}\\
&=\frac12(1-1)\\
&=\boxed{0}
\end{aligned}
$$

Jadi:
$$
\boxed{\{|+\rangle,|-\rangle\}\text{ ortonormal}}
$$

---

## TASK 3 — Operator: Hermitian, Unitary, Commutator

Diketahui:
$$
A=\begin{pmatrix}
2&1-i\\
1+i&3
\end{pmatrix}
$$
$$
S=\begin{pmatrix}1&0\\0&i\end{pmatrix}
$$
$$
B=\begin{pmatrix}1&1\\0&1\end{pmatrix}
$$

### 3.1 Menghitung conjugate transpose

Rumus:
$$
M^\dagger=(M^*)^T
$$

a. Matriks $A$
$$
A^*=
\begin{pmatrix}
2&1+i\\
1-i&3
\end{pmatrix}
$$
$$
\boxed{
A^\dagger=
\begin{pmatrix}
2&1-i\\
1+i&3
\end{pmatrix}
}
$$

b. Matriks $S$
$$
S^*=
\begin{pmatrix}1&0\\0&-i\end{pmatrix}
$$
$$
\boxed{
S^\dagger=
\begin{pmatrix}1&0\\0&-i\end{pmatrix}
}
$$

c. Matriks $B$
$$
B^*=
\begin{pmatrix}1&1\\0&1\end{pmatrix}
$$
$$
\boxed{
B^\dagger=
\begin{pmatrix}1&0\\1&1\end{pmatrix}
}
$$

### 3.2 Menentukan Hermitian dan Unitary

Syarat:
$$
\text{Hermitian: }M^\dagger=M
$$
$$
\text{Unitary: }M^\dagger M=I
$$

a. Matriks $A$
Hermitian:
$$
A^\dagger=
\begin{pmatrix}2&1-i\\1+i&3\end{pmatrix}=A
$$
$$
\boxed{A\text{ Hermitian}}
$$

Unitary:
$$
\begin{aligned}
A^\dagger A
&=
\begin{pmatrix}2&1-i\\1+i&3\end{pmatrix}
\begin{pmatrix}2&1-i\\1+i&3\end{pmatrix}\\
&=
\begin{pmatrix}
6&5-5i\\
5+5i&11
\end{pmatrix}
\end{aligned}
$$
$$
A^\dagger A\neq I
$$
$$
\boxed{A\text{ bukan Unitary}}
$$

b. Matriks $S$
Hermitian:
$$
S^\dagger=
\begin{pmatrix}1&0\\0&-i\end{pmatrix}
\neq S
$$
$$
\boxed{S\text{ bukan Hermitian}}
$$

Unitary:
$$
\begin{aligned}
S^\dagger S
&=
\begin{pmatrix}1&0\\0&-i\end{pmatrix}
\begin{pmatrix}1&0\\0&i\end{pmatrix}\\
&=\begin{pmatrix}1&0\\0&1\end{pmatrix}\\
&=I
\end{aligned}
$$
$$
\boxed{S\text{ Unitary}}
$$

c. Matriks $B$
Hermitian:
$$
B^\dagger=
\begin{pmatrix}1&0\\1&1\end{pmatrix}
\neq B
$$
$$
\boxed{B\text{ bukan Hermitian}}
$$

Unitary:
$$
\begin{aligned}
B^\dagger B
&=
\begin{pmatrix}1&0\\1&1\end{pmatrix}
\begin{pmatrix}1&1\\0&1\end{pmatrix}\\
&=\begin{pmatrix}1&1\\1&2\end{pmatrix}
\end{aligned}
$$
$$
B^\dagger B\neq I
$$
$$
\boxed{B\text{ bukan Unitary}}
$$

**Ringkasan:**

| Matriks | Hermitian | Unitary |
| :---: | :---: | :---: |
| **A** | Ya | Tidak |
| **S** | Tidak | Ya |
| **B** | Tidak | Tidak |

### 3.3 Menghitung $S|+\rangle$

Diketahui:
$$
S=\begin{pmatrix}1&0\\0&i\end{pmatrix}
$$
$$
|+\rangle=\frac1{\sqrt2}
\begin{pmatrix}1\\1\end{pmatrix}
$$
$$
\begin{aligned}
S|+\rangle
&=\frac1{\sqrt2}
\begin{pmatrix}1&0\\0&i\end{pmatrix}
\begin{pmatrix}1\\1\end{pmatrix}\\
&=\frac1{\sqrt2}
\begin{pmatrix}1\\i\end{pmatrix}
\end{aligned}
$$
$$
\boxed{S|+\rangle=|+i\rangle}
$$

### 3.4 Menghitung $HZH$ dan $HXH$

Diketahui:
$$
H=\frac1{\sqrt2}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}
$$
$$
Z=\begin{pmatrix}1&0\\0&-1\end{pmatrix}
,\quad
X=\begin{pmatrix}0&1\\1&0\end{pmatrix}
$$

a. Menghitung $HZH$
$$
\begin{aligned}
HZH
&=\frac12
\begin{pmatrix}1&1\\1&-1\end{pmatrix}
\begin{pmatrix}1&0\\0&-1\end{pmatrix}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}\\
&=\frac12
\begin{pmatrix}1&-1\\1&1\end{pmatrix}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}\\
&=\frac12
\begin{pmatrix}0&2\\2&0\end{pmatrix}\\
&=\boxed{X}
\end{aligned}
$$

b. Menghitung $HXH$
$$
\begin{aligned}
HXH
&=\frac12
\begin{pmatrix}1&1\\1&-1\end{pmatrix}
\begin{pmatrix}0&1\\1&0\end{pmatrix}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}\\
&=\frac12
\begin{pmatrix}1&1\\-1&1\end{pmatrix}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}\\
&=\frac12
\begin{pmatrix}2&0\\0&-2\end{pmatrix}\\
&=\boxed{Z}
\end{aligned}
$$

Hasil:
$$
\boxed{HZH=X,\qquad HXH=Z}
$$

### 3.5 Menghitung commutator $[X,Y]$

Rumus:
$$
[X,Y]=XY-YX
$$

Diketahui:
$$
X=\begin{pmatrix}0&1\\1&0\end{pmatrix}
$$
$$
Y=\begin{pmatrix}0&-i\\i&0\end{pmatrix}
$$

Hitung $XY$:
$$
\begin{aligned}
XY
&=\begin{pmatrix}0&1\\1&0\end{pmatrix}
\begin{pmatrix}0&-i\\i&0\end{pmatrix}\\
&=\begin{pmatrix}i&0\\0&-i\end{pmatrix}\\
&=iZ
\end{aligned}
$$

Hitung $YX$:
$$
\begin{aligned}
YX
&=\begin{pmatrix}0&-i\\i&0\end{pmatrix}
\begin{pmatrix}0&1\\1&0\end{pmatrix}\\
&=\begin{pmatrix}-i&0\\0&i\end{pmatrix}\\
&=-iZ
\end{aligned}
$$

Maka:
$$
\begin{aligned}
[X,Y]
&=XY-YX\\
&=iZ-(-iZ)\\
&=\boxed{2iZ}
\end{aligned}
$$

### 3.6 Membuktikan $X^2=Y^2=Z^2=I$

a. 
$$
\begin{aligned}
X^2
&=\begin{pmatrix}0&1\\1&0\end{pmatrix}
\begin{pmatrix}0&1\\1&0\end{pmatrix}\\
&=\begin{pmatrix}1&0\\0&1\end{pmatrix}\\
&=\boxed{I}
\end{aligned}
$$

b. 
$$
\begin{aligned}
Y^2
&=\begin{pmatrix}0&-i\\i&0\end{pmatrix}
\begin{pmatrix}0&-i\\i&0\end{pmatrix}\\
&=\begin{pmatrix}1&0\\0&1\end{pmatrix}\\
&=\boxed{I}
\end{aligned}
$$

c. 
$$
\begin{aligned}
Z^2
&=\begin{pmatrix}1&0\\0&-1\end{pmatrix}
\begin{pmatrix}1&0\\0&-1\end{pmatrix}\\
&=\begin{pmatrix}1&0\\0&1\end{pmatrix}\\
&=\boxed{I}
\end{aligned}
$$

Jadi:
$$
\boxed{X^2=Y^2=Z^2=I}
$$

### 3.7 Mengapa matriks $B$ tidak bisa menjadi quantum gate?

Syarat quantum gate:
$$
B^\dagger B=I
$$

Dari nomor 3.2:
$$
B^\dagger B=
\begin{pmatrix}1&1\\1&2\end{pmatrix}
\neq I
$$

Buktikan dengan state:
$$
|\psi\rangle=|+\rangle=
\frac1{\sqrt2}\begin{pmatrix}1\\1\end{pmatrix}
$$

Norm awal:
$$
\|\psi\|=1
$$

Kalikan dengan $B$:
$$
\begin{aligned}
B|\psi\rangle
&=\frac1{\sqrt2}
\begin{pmatrix}1&1\\0&1\end{pmatrix}
\begin{pmatrix}1\\1\end{pmatrix}\\
&=\frac1{\sqrt2}
\begin{pmatrix}2\\1\end{pmatrix}
\end{aligned}
$$

Norm hasil:
$$
\begin{aligned}
\|B|\psi\rangle\|
&=\sqrt{\left|\frac2{\sqrt2}\right|^2+
\left|\frac1{\sqrt2}\right|^2}\\
&=\sqrt{2+\frac12}\\
&=\boxed{\sqrt{\frac52}\neq1}
\end{aligned}
$$
$$
\boxed{B\text{ bukan quantum gate karena tidak unitary}}
$$

---

## TASK 4 — Eigenvalue & Eigenvector

Rumus dasar:
$$
A|v\rangle=\lambda|v\rangle
$$
Eigenvalue:
$$
\det(A-\lambda I)=0
$$
Eigenvector:
$$
(A-\lambda I)|v\rangle=0
$$

### 4.1 Eigenvalue dan eigenvector Pauli Y

Diketahui:
$$
Y=\begin{pmatrix}0&-i\\i&0\end{pmatrix}
$$

a. Mencari eigenvalue
$$
\begin{aligned}
\det(Y-\lambda I)&=0\\
\begin{vmatrix}-\lambda&-i\\i&-\lambda\end{vmatrix}&=0\\
\lambda^2-(-i)(i)&=0\\
\lambda^2-1&=0\\
(\lambda-1)(\lambda+1)&=0
\end{aligned}
$$
$$
\boxed{\lambda_1=1,\quad\lambda_2=-1}
$$

b. Eigenvector untuk $\lambda=+1$
$$
(Y-I)|v\rangle=0
$$
$$
\begin{pmatrix}-1&-i\\i&-1\end{pmatrix}
\begin{pmatrix}x\\y\end{pmatrix}
=
\begin{pmatrix}0\\0\end{pmatrix}
$$

Baris pertama:
$$
-x-iy=0
$$
$$
x=-iy
$$
Ambil $y=i$, maka $x=1$.
$$
|v_+\rangle=\begin{pmatrix}1\\i\end{pmatrix}
$$

Norm:
$$
\begin{aligned}
\|v_+\|
&=\sqrt{|1|^2+|i|^2}\\
&=\sqrt2
\end{aligned}
$$

Normalisasi:
$$
\boxed{
|v_+\rangle=\frac1{\sqrt2}
\begin{pmatrix}1\\i\end{pmatrix}
}
$$

c. Eigenvector untuk $\lambda=-1$
$$
(Y+I)|v\rangle=0
$$
$$
\begin{pmatrix}1&-i\\i&1\end{pmatrix}
\begin{pmatrix}x\\y\end{pmatrix}
=
\begin{pmatrix}0\\0\end{pmatrix}
$$

Baris pertama:
$$
x-iy=0
$$
$$
x=iy
$$
Ambil $y=-i$, maka $x=1$.
$$
|v_-\rangle=\begin{pmatrix}1\\-i\end{pmatrix}
$$

Norm:
$$
\|v_-\|=\sqrt{1+1}=\sqrt2
$$

Normalisasi:
$$
\boxed{
|v_-\rangle=\frac1{\sqrt2}
\begin{pmatrix}1\\-i\end{pmatrix}
}
$$

### 4.2 Eigenvalue dan eigenvector matriks A

Diketahui:
$$
A=\begin{pmatrix}2&1-i\\1+i&3\end{pmatrix}
$$

a. Mencari eigenvalue
$$
\det(A-\lambda I)=0
$$
$$
\begin{aligned}
\begin{vmatrix}
2-\lambda&1-i\\
1+i&3-\lambda
\end{vmatrix}&=0\\
(2-\lambda)(3-\lambda)-(1-i)(1+i)&=0
\end{aligned}
$$

Karena:
$$
(1-i)(1+i)=1-i^2=2
$$

Maka:
$$
\begin{aligned}
(2-\lambda)(3-\lambda)-2&=0\\
6-5\lambda+\lambda^2-2&=0\\
\lambda^2-5\lambda+4&=0\\
(\lambda-1)(\lambda-4)&=0
\end{aligned}
$$
$$
\boxed{\lambda_1=1,\quad\lambda_2=4}
$$

b. Eigenvector untuk $\lambda=1$
$$
(A-I)|v_1\rangle=0
$$
$$
\begin{pmatrix}1&1-i\\1+i&2\end{pmatrix}
\begin{pmatrix}x\\y\end{pmatrix}
=
\begin{pmatrix}0\\0\end{pmatrix}
$$

Baris pertama:
$$
x+(1-i)y=0
$$
$$
x=(-1+i)y
$$
Ambil $y=1$, maka $x=-1+i$.
$$
|v_1\rangle=
\begin{pmatrix}-1+i\\1\end{pmatrix}
$$

Norm:
$$
\begin{aligned}
\|v_1\|
&=\sqrt{|-1+i|^2+|1|^2}\\
&=\sqrt{1+1+1}\\
&=\sqrt3
\end{aligned}
$$

Normalisasi:
$$
\boxed{
|v_1\rangle=\frac1{\sqrt3}
\begin{pmatrix}-1+i\\1\end{pmatrix}
}
$$

c. Eigenvector untuk $\lambda=4$
$$
(A-4I)|v_2\rangle=0
$$
$$
\begin{pmatrix}-2&1-i\\1+i&-1\end{pmatrix}
\begin{pmatrix}x\\y\end{pmatrix}
=
\begin{pmatrix}0\\0\end{pmatrix}
$$

Baris pertama:
$$
-2x+(1-i)y=0
$$
$$
x=\frac{1-i}{2}y
$$
Ambil $y=2$, maka $x=1-i$.
$$
|v_2\rangle=
\begin{pmatrix}1-i\\2\end{pmatrix}
$$

Norm:
$$
\begin{aligned}
\|v_2\|
&=\sqrt{|1-i|^2+|2|^2}\\
&=\sqrt{2+4}\\
&=\sqrt6
\end{aligned}
$$

Normalisasi:
$$
\boxed{
|v_2\rangle=\frac1{\sqrt6}
\begin{pmatrix}1-i\\2\end{pmatrix}
}
$$

d. Apakah eigenvalue real?
$$
\lambda_1=1,\qquad\lambda_2=4
$$
Karena:
$$
A^\dagger=A
$$
Maka $A$ Hermitian, sehingga eigenvalue-nya real.
$$
\boxed{\lambda_1,\lambda_2\in\mathbb R}
$$

### 4.3 Membuktikan kedua eigenvector A ortogonal

Diketahui:
$$
|v_1\rangle=\frac1{\sqrt3}
\begin{pmatrix}-1+i\\1\end{pmatrix}
$$
$$
|v_2\rangle=\frac1{\sqrt6}
\begin{pmatrix}1-i\\2\end{pmatrix}
$$

Bra:
$$
\langle v_1|=\frac1{\sqrt3}
\begin{pmatrix}-1-i&1\end{pmatrix}
$$

Inner product:
$$
\begin{aligned}
\langle v_1|v_2\rangle
&=\frac1{\sqrt{18}}
\begin{pmatrix}-1-i&1\end{pmatrix}
\begin{pmatrix}1-i\\2\end{pmatrix}\\
&=\frac1{\sqrt{18}}
[(-1-i)(1-i)+2]
\end{aligned}
$$

Hitung:
$$
\begin{aligned}
(-1-i)(1-i)
&=-1+i-i+i^2\\
&=-2
\end{aligned}
$$

Maka:
$$
\begin{aligned}
\langle v_1|v_2\rangle
&=\frac1{\sqrt{18}}(-2+2)\\
&=\boxed{0}
\end{aligned}
$$
$$
\boxed{|v_1\rangle\perp|v_2\rangle}
$$

### 4.4 Menghitung eigenvalue Hadamard H

Diketahui:
$$
H=\frac1{\sqrt2}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}
$$
$$
\det(H-\lambda I)=0
$$
$$
\begin{aligned}
\begin{vmatrix}
\frac1{\sqrt2}-\lambda&\frac1{\sqrt2}\\
\frac1{\sqrt2}&-\frac1{\sqrt2}-\lambda
\end{vmatrix}&=0\\
\left(\frac1{\sqrt2}-\lambda\right)
\left(-\frac1{\sqrt2}-\lambda\right)-\frac12&=0\\
\lambda^2-\frac12-\frac12&=0\\
\lambda^2-1&=0\\
(\lambda-1)(\lambda+1)&=0
\end{aligned}
$$
$$
\boxed{\lambda_1=+1,\quad\lambda_2=-1}
$$

### 4.5 Menuliskan Pauli Z dalam bentuk outer product

Diketahui:
$$
Z=\begin{pmatrix}1&0\\0&-1\end{pmatrix}
$$

Eigenvalue dan eigenvector:
$$
\lambda_1=+1,\quad
|v_1\rangle=|0\rangle=
\begin{pmatrix}1\\0\end{pmatrix}
$$
$$
\lambda_2=-1,\quad
|v_2\rangle=|1\rangle=
\begin{pmatrix}0\\1\end{pmatrix}
$$

Rumus spectral decomposition:
$$
Z=\sum_k\lambda_k|v_k\rangle\langle v_k|
$$

Substitusi:
$$
Z=|0\rangle\langle0|-|1\rangle\langle1|
$$

Hitung outer product:
$$
|0\rangle\langle0|=
\begin{pmatrix}1\\0\end{pmatrix}
\begin{pmatrix}1&0\end{pmatrix}
=
\begin{pmatrix}1&0\\0&0\end{pmatrix}
$$
$$
|1\rangle\langle1|=
\begin{pmatrix}0\\1\end{pmatrix}
\begin{pmatrix}0&1\end{pmatrix}
=
\begin{pmatrix}0&0\\0&1\end{pmatrix}
$$

Maka:
$$
\begin{aligned}
Z&=
\begin{pmatrix}1&0\\0&0\end{pmatrix}
-
\begin{pmatrix}0&0\\0&1\end{pmatrix}\\
&=\begin{pmatrix}1&0\\0&-1\end{pmatrix}
\end{aligned}
$$
$$
\boxed{Z=|0\rangle\langle0|-|1\rangle\langle1|}
$$
