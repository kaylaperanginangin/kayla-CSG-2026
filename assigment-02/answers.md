# Task 1 — Bilangan Kompleks

Dik:

$$
z_1=1+i,\qquad z_2=\sqrt{3}-i
$$

## 1 Hitung $z_1+z_2$, $z_1z_2$, $z_1^\*$, dan $z_1/z_2$

### a. Penjumlahan $z_1+z_2$

$$
\begin{aligned}
z_1+z_2
&=(1+i)+(\sqrt{3}-i)\\
&=1+\sqrt{3}+i-i\\
&=\boxed{1+\sqrt{3}}
\end{aligned}
$$

### b. Perkalian $z_1z_2$

$$
\begin{aligned}
z_1z_2
&=(1+i)(\sqrt{3}-i)\\
&=\sqrt{3}-i+i\sqrt{3}-i^2
\end{aligned}
$$

Karena $i^2=-1$, maka:

$$
\begin{aligned}
z_1z_2
&=\sqrt{3}-i+i\sqrt{3}+1\\
&=(\sqrt{3}+1)+(\sqrt{3}-1)i
\end{aligned}
$$

$$
\boxed{z_1z_2=(\sqrt{3}+1)+(\sqrt{3}-1)i}
$$

### c. Konjugat kompleks $z_1^\*$

$$
z_1=1+i
$$

$$
\boxed{z_1^\*=1-i}
$$

### d. Pembagian $z_1/z_2$

$$
\begin{aligned}
\frac{z_1}{z_2}
&=\frac{1+i}{\sqrt{3}-i}
\times\frac{\sqrt{3}+i}{\sqrt{3}+i}\\
&=\frac{(1+i)(\sqrt{3}+i)}{(\sqrt{3}-i)(\sqrt{3}+i)}
\end{aligned}
$$

Hitung pembilang:

$$
\begin{aligned}
(1+i)(\sqrt{3}+i)
&=\sqrt{3}+i+i\sqrt{3}+i^2\\
&=\sqrt{3}-1+(1+\sqrt{3})i
\end{aligned}
$$

Hitung penyebut:

$$
\begin{aligned}
(\sqrt{3}-i)(\sqrt{3}+i)
&=(\sqrt{3})^2-i^2\\
&=3-(-1)=4
\end{aligned}
$$

Maka:

$$
\boxed{
\frac{z_1}{z_2}
=\frac{\sqrt{3}-1}{4}
+\frac{1+\sqrt{3}}{4}i
}
$$

## 2 Hitung $|z_1|$, $|z_2|$, dan $|z_1z_2|$

Rumus modulus bilangan kompleks:

$$
|z|=\sqrt{a^2+b^2}
$$

### a. Modulus $z_1$

$$
\begin{aligned}
|z_1|
&=|1+i|\\
&=\sqrt{1^2+1^2}\\
&=\boxed{\sqrt{2}}
\end{aligned}
$$

### b. Modulus $z_2$

$$
\begin{aligned}
|z_2|
&=|\sqrt{3}-i|\\
&=\sqrt{(\sqrt{3})^2+(-1)^2}\\
&=\sqrt{3+1}\\
&=\boxed{2}
\end{aligned}
$$

### c. Modulus $z_1z_2$

Dari hasil nomor 1.1:

$$
z_1z_2=(\sqrt{3}+1)+(\sqrt{3}-1)i
$$

$$
\begin{aligned}
|z_1z_2|
&=\sqrt{(\sqrt{3}+1)^2+(\sqrt{3}-1)^2}\\
&=\sqrt{(4+2\sqrt{3})+(4-2\sqrt{3})}\\
&=\sqrt{8}\\
&=\boxed{2\sqrt{2}}
\end{aligned}
$$

### d. Verifikasi sifat modulus perkalian

$$
|z_1||z_2|=\sqrt{2}\times 2=2\sqrt{2}
$$

Sementara itu:

$$
|z_1z_2|=2\sqrt{2}
$$

Maka:

$$
\boxed{|z_1z_2|=|z_1||z_2|}
$$

## 3 Tuliskan $z_1$ dan $z_2$ dalam bentuk polar $re^{i\theta}$.

Bentuk polar bilangan kompleks:

$$
z=re^{i\theta}
$$

Dengan:

$$
r=|z|,\qquad \theta=\tan^{-1}\left(\frac{b}{a}\right)
$$

### a. Bentuk polar $z_1=1+i$

Modulus:

$$
r_1=\sqrt{1^2+1^2}=\sqrt{2}
$$

Sudut:

$$
\theta_1=\tan^{-1}\left(\frac{1}{1}\right)
=\frac{\pi}{4}
$$

Karena $z_1$ berada di kuadran I, sudutnya tetap $\pi/4$.

Jadi:

$$
\boxed{z_1=\sqrt{2}e^{i\pi/4}}
$$

### b. Bentuk polar $z_2=\sqrt{3}-i$

Modulus:

$$
r_2=\sqrt{(\sqrt{3})^2+(-1)^2}=2
$$

Sudut:

$$
\theta_2=\tan^{-1}\left(\frac{-1}{\sqrt{3}}\right)
=-\frac{\pi}{6}
$$

Karena $z_2$ berada di kuadran IV, sudutnya adalah $-\pi/6$.

Jadi:

$$
\boxed{z_2=2e^{-i\pi/6}}
$$

## 4 Gunakan bentuk polar untuk menghitung $z_1^{8}$

Dari nomor 1.3:

$$
z_1=\sqrt{2}e^{i\pi/4}
$$

Gunakan teorema De Moivre:

$$
(re^{i\theta})^n=r^ne^{in\theta}
$$

Maka:

$$
\begin{aligned}
z_1^8
&=(\sqrt{2}e^{i\pi/4})^8\\
&=(\sqrt{2})^8e^{i(8\pi/4)}\\
&=2^4e^{i2\pi}\\
&=16(\cos 2\pi+i\sin 2\pi)\\
&=16(1+0i)
\end{aligned}
$$

$$
\boxed{z_1^8=16}
$$

## 5 Tunjukkan bahwa $|e^{i\theta}|^2 = 1$ untuk sembarang $\theta$ real.

Berdasarkan formula Euler:

$$
e^{i\theta}=\cos\theta+i\sin\theta
$$

Modulus kuadrat:

$$
\begin{aligned}
|e^{i\theta}|^2
&=|\cos\theta+i\sin\theta|^2\\
&=\cos^2\theta+\sin^2\theta
\end{aligned}
$$

Menggunakan identitas trigonometri:

$$
\cos^2\theta+\sin^2\theta=1
$$

Maka:

$$
\boxed{|e^{i\theta}|^2=1}
$$

---

# Task 2 — State, Inner Product, & Normalisasi

Diketahui:

$$
|a\rangle=
\begin{pmatrix}
1\\
2i
\end{pmatrix},
\qquad
|b\rangle=
\begin{pmatrix}
2\\
-i
\end{pmatrix}
$$

$$
|c\rangle=\frac{1}{2}|0\rangle+
\frac{\sqrt{3}}{2}e^{i\pi/4}|1\rangle
$$

## 1 Tuliskan $\langle a|$ dan $\langle b|$.

Menurut Dirac notation, bra merupakan conjugate transpose dari ket:

$$
\langle\psi|=(|\psi\rangle^\dagger)
$$

### a. Bra dari $|a\rangle$

$$
|a\rangle=
\begin{pmatrix}
1\\
2i
\end{pmatrix}
$$

Transpose:

$$
\begin{pmatrix}
1&2i
\end{pmatrix}
$$

Konjugasikan setiap elemen:

$$
\boxed{\langle a|=\begin{pmatrix}1&-2i\end{pmatrix}}
$$

### b. Bra dari $|b\rangle$

$$
|b\rangle=
\begin{pmatrix}
2\\
-i
\end{pmatrix}
$$

Transpose:

$$
\begin{pmatrix}
2&-i
\end{pmatrix}
$$

Konjugasikan setiap elemen:

$$
\boxed{\langle b|=\begin{pmatrix}2&i\end{pmatrix}}
$$

## 2 Hitung $\langle a|b\rangle$ dan $\langle b|a\rangle$. Verifikasi bahwa $\langle a|b\rangle = \langle b|a\rangle^*$.

Rumus inner product:

$$
\langle a|b\rangle=a_1^*b_1+a_2^*b_2
$$

### a. Menghitung $\langle a|b\rangle$

$$
\begin{aligned}
\langle a|b\rangle
&=\begin{pmatrix}1&-2i\end{pmatrix}
\begin{pmatrix}2\\-i\end{pmatrix}\\
&=(1)(2)+(-2i)(-i)\\
&=2+2i^2\\
&=2-2\\
&=\boxed{0}
\end{aligned}
$$

### b. Menghitung $\langle b|a\rangle$

$$
\begin{aligned}
\langle b|a\rangle
&=\begin{pmatrix}2&i\end{pmatrix}
\begin{pmatrix}1\\2i\end{pmatrix}\\
&=(2)(1)+(i)(2i)\\
&=2+2i^2\\
&=2-2\\
&=\boxed{0}
\end{aligned}
$$

### c. Verifikasi sifat inner product

Sifat inner product:

$$
\langle a|b\rangle=\langle b|a\rangle^\*
$$

Karena:

$$
\langle a|b\rangle=0
$$

dan:

$$
\langle b|a\rangle^_=0^_=0
$$

Maka:

$$
\boxed{\langle a|b\rangle=\langle b|a\rangle^\*}
$$

## 3 Apakah $|a\rangle$ dan $|b\rangle$ ortogonal?

Dua state dikatakan ortogonal apabila:

$$
\langle a|b\rangle=0
$$

Dari perhitungan nomor 2.2:

$$
\langle a|b\rangle=0
$$

Jadi:

$$
\boxed{|a\rangle\text{ dan }|b\rangle\text{ saling ortogonal}}
$$

## 4 Normalisasi $|a\rangle$ dan $|b\rangle$

Rumus norm:

$$
\|\psi\|=\sqrt{\langle\psi|\psi\rangle}
$$

Rumus normalisasi:

$$
|\psi\_{\text{norm}}\rangle=
\frac{|\psi\rangle}{\|\psi\|}
$$

### a. Normalisasi $|a\rangle$

$$
\begin{aligned}
\|a\|
&=\sqrt{\langle a|a\rangle}\\
&=\sqrt{(1)(1)+(-2i)(2i)}\\
&=\sqrt{1-4i^2}\\
&=\sqrt{1+4}\\
&=\sqrt{5}
\end{aligned}
$$

Maka:

$$
\begin{aligned}
|a\_{\text{norm}}\rangle
&=\frac{1}{\sqrt{5}}
\begin{pmatrix}
1\\2i
\end{pmatrix}\\
&=\boxed{
\begin{pmatrix}
\frac{1}{\sqrt{5}}\\[2pt]
\frac{2i}{\sqrt{5}}
\end{pmatrix}}
\end{aligned}
$$

Verifikasi:

$$
\left\|a\_{\text{norm}}\right\|^2
=\frac{1}{5}+\frac{4}{5}=1
$$

### b. Normalisasi $|b\rangle$

$$
\begin{aligned}
\|b\|
&=\sqrt{\langle b|b\rangle}\\
&=\sqrt{(2)(2)+(i)(-i)}\\
&=\sqrt{4-i^2}\\
&=\sqrt{4+1}\\
&=\sqrt{5}
\end{aligned}
$$

Maka:

$$
\begin{aligned}
|b\_{\text{norm}}\rangle
&=\frac{1}{\sqrt{5}}
\begin{pmatrix}
2\\-i
\end{pmatrix}\\
&=\boxed{
\begin{pmatrix}
\frac{2}{\sqrt{5}}\\[2pt]
-\frac{i}{\sqrt{5}}
\end{pmatrix}}
\end{aligned}
$$

Verifikasi:

$$
\left\|b\_{\text{norm}}\right\|^2
=\frac{4}{5}+\frac{1}{5}=1
$$

## 5 Apakah $|c\rangle$ sudah ternormalisasi? Hitung $P(0)$ dan $P(1)$ jika $|c\rangle$ diukur di computational basis.

Dik:

$$
|c\rangle=\frac{1}{2}|0\rangle+
\frac{\sqrt{3}}{2}e^{i\pi/4}|1\rangle
$$

Berdasarkan Born rule:

$$
P(k)=|\langle k|c\rangle|^2
$$

### a. Memeriksa apakah state sudah ternormalisasi

Syarat state ternormalisasi:

$$
\langle c|c\rangle=1
$$

Dengan amplitudo:

$$
\alpha=\frac{1}{2},\qquad
\beta=\frac{\sqrt{3}}{2}e^{i\pi/4}
$$

Maka:

$$
\begin{aligned}
\langle c|c\rangle
&=|\alpha|^2+|\beta|^2\\
&=\left|\frac{1}{2}\right|^2+
\left|\frac{\sqrt{3}}{2}e^{i\pi/4}\right|^2\\
&=\frac{1}{4}+\frac{3}{4}|e^{i\pi/4}|^2\\
&=\frac{1}{4}+\frac{3}{4}(1)\\
&=1
\end{aligned}
$$

Jadi:

$$
\boxed{|c\rangle\text{ sudah ternormalisasi}}
$$

### b. Probabilitas mendapatkan hasil $0$

$$
\begin{aligned}
P(0)
&=|\langle0|c\rangle|^2\\
&=\left|\frac{1}{2}\right|^2\\
&=\boxed{\frac{1}{4}=0{,}25=25\%}
\end{aligned}
$$

### c. Probabilitas mendapatkan hasil $1$

$$
\begin{aligned}
P(1)
&=|\langle1|c\rangle|^2\\
&=\left|\frac{\sqrt{3}}{2}e^{i\pi/4}\right|^2\\
&=\frac{3}{4}|e^{i\pi/4}|^2\\
&=\boxed{\frac{3}{4}=0{,}75=75\%}
\end{aligned}
$$

Verifikasi:

$$
P(0)+P(1)=\frac{1}{4}+\frac{3}{4}=1
$$

## 6 Tuliskan $|c\rangle$ dalam **Hadamard basis** $\{|+\rangle, |-\rangle\}$, lalu hitung $P(+)$ dan $P(-)$.

Hadamard basis:

$$
|+\rangle=\frac{1}{\sqrt{2}}
\begin{pmatrix}1\\1\end{pmatrix},
\qquad
|-\rangle=\frac{1}{\sqrt{2}}
\begin{pmatrix}1\\-1\end{pmatrix}
$$

State dalam basis Hadamard:

$$
|c\rangle=c*+|+\rangle+c*-|-\rangle
$$

Koefisien diperoleh menggunakan inner product:

$$
c*+=\langle+|c\rangle,\qquad
c*-=\langle-|c\rangle
$$

### a. Menghitung koefisien $c\_+$

$$
\begin{aligned}
c\_+
&=\langle+|c\rangle\\
&=\frac{1}{\sqrt{2}}
\left(\frac{1}{2}+
\frac{\sqrt{3}}{2}e^{i\pi/4}\right)\\
&=\frac{1}{2\sqrt{2}}
\left(1+\sqrt{3}e^{i\pi/4}\right)
\end{aligned}
$$

### b. Menghitung koefisien $c\_-$

$$
\begin{aligned}
c\_-
&=\langle-|c\rangle\\
&=\frac{1}{\sqrt{2}}
\left(\frac{1}{2}-
\frac{\sqrt{3}}{2}e^{i\pi/4}\right)\\
&=\frac{1}{2\sqrt{2}}
\left(1-\sqrt{3}e^{i\pi/4}\right)
\end{aligned}
$$

Jadi, representasi state dalam Hadamard basis:

$$
\boxed{
|c\rangle=
\frac{1+\sqrt{3}e^{i\pi/4}}{2\sqrt{2}}|+\rangle

- \frac{1-\sqrt{3}e^{i\pi/4}}{2\sqrt{2}}|-\rangle
  }
$$

### c. Menghitung probabilitas $P(+)$

$$
\begin{aligned}
P(+)
&=|c\_+|^2\\
&=\frac{1}{8}
\left|1+\sqrt{3}e^{i\pi/4}\right|^2
\end{aligned}
$$

Gunakan:

$$
|1+re^{i\theta}|^2
=1+r^2+2r\cos\theta
$$

Sehingga:

$$
\begin{aligned}
P(+)
&=\frac{1}{8}
\left(1+3+2\sqrt{3}\cos\frac{\pi}{4}\right)\\
&=\frac{1}{8}
\left(4+2\sqrt{3}\cdot\frac{\sqrt{2}}{2}\right)\\
&=\boxed{\frac{4+\sqrt{6}}{8}}
\end{aligned}
$$

Nilai pendekatan:

$$
P(+)\approx0{,}8062=80{,}62\%
$$

### d. Menghitung probabilitas $P(-)$

$$
\begin{aligned}
P(-)
&=|c\_-|^2\\
&=\frac{1}{8}
\left|1-\sqrt{3}e^{i\pi/4}\right|^2
\end{aligned}
$$

Gunakan:

$$
|1-re^{i\theta}|^2
=1+r^2-2r\cos\theta
$$

Sehingga:

$$
\begin{aligned}
P(-)
&=\frac{1}{8}
\left(1+3-2\sqrt{3}\cos\frac{\pi}{4}\right)\\
&=\frac{1}{8}
\left(4-\sqrt{6}\right)\\
&=\boxed{\frac{4-\sqrt{6}}{8}}
\end{aligned}
$$

Nilai pendekatan:

$$
P(-)\approx0{,}1938=19{,}38\%
$$

Verifikasi:

$$
\begin{aligned}
P(+)+P(-)
&=\frac{4+\sqrt{6}}{8}+
\frac{4-\sqrt{6}}{8}\\
&=\frac{8}{8}\\
&=1
\end{aligned}
$$

## 7 Buktikan bahwa $\{|+\rangle, |-\rangle\}$ adalah basis ortonormal.

Syarat basis ortonormal:

$$
\langle e*i|e_j\rangle=\delta*{ij}
$$

### a. Membuktikan $\langle+|+\rangle=1$

$$
\begin{aligned}
\langle+|+\rangle
&=\frac{1}{\sqrt{2}}(1\quad1)
\frac{1}{\sqrt{2}}
\begin{pmatrix}1\\1\end{pmatrix}\\
&=\frac{1}{2}(1+1)\\
&=\boxed{1}
\end{aligned}
$$

### b. Membuktikan $\langle-|-\rangle=1$

$$
\begin{aligned}
\langle-|- \rangle
&=\frac{1}{\sqrt{2}}(1\quad-1)
\frac{1}{\sqrt{2}}
\begin{pmatrix}1\\-1\end{pmatrix}\\
&=\frac{1}{2}(1+1)\\
&=\boxed{1}
\end{aligned}
$$

### c. Membuktikan $\langle+|-\rangle=0$

$$
\begin{aligned}
\langle+|-\rangle
&=\frac{1}{2}(1\quad1)
\begin{pmatrix}1\\-1\end{pmatrix}\\
&=\frac{1}{2}(1-1)\\
&=\boxed{0}
\end{aligned}
$$

Dengan demikian, kedua vektor memiliki norm 1 dan saling ortogonal.

$$
\boxed{\{|+\rangle,|-\rangle\}\text{ adalah basis ortonormal}}
$$

---

# Task 3 — Operator: Hermitian, Unitary, Commutator

Dik:

$$
A=\begin{pmatrix}
2&1-i\\
1+i&3
\end{pmatrix}
$$

$$
S=\begin{pmatrix}
1&0\\
0&i
\end{pmatrix},
\qquad
B=\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

## 1 Hitung $A^\dagger$, $S^\dagger$, dan $B^\dagger$.

Conjugate transpose atau dagger:

$$
M^\dagger=(M^\*)^T
$$

Artinya, setiap elemen dikonjugasi kemudian matriks ditranspose.

### a. Menghitung $A^\dagger$

$$
A=
\begin{pmatrix}
2&1-i\\
1+i&3
\end{pmatrix}
$$

Konjugasi:

$$
A^\*=
\begin{pmatrix}
2&1+i\\
1-i&3
\end{pmatrix}
$$

Transpose:

$$
\boxed{
A^\dagger=
\begin{pmatrix}
2&1-i\\
1+i&3
\end{pmatrix}
}
$$

### b. Menghitung $S^\dagger$

$$
S=
\begin{pmatrix}
1&0\\
0&i
\end{pmatrix}
$$

Konjugasi:

$$
S^\*=
\begin{pmatrix}
1&0\\
0&-i
\end{pmatrix}
$$

Transpose tidak mengubah matriks diagonal.

$$
\boxed{
S^\dagger=
\begin{pmatrix}
1&0\\
0&-i
\end{pmatrix}
}
$$

### c. Menghitung $B^\dagger$

$$
B=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

Karena semua elemen real, konjugasinya tidak berubah:

$$
B^\*=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

Transpose:

$$
\boxed{
B^\dagger=
\begin{pmatrix}
1&0\\
1&1
\end{pmatrix}
}
$$

## 2 Tentukan mana yang Hermitian, mana yang unitary (boleh keduanya atau tidak sama sekali). Tunjukkan perhitungannya.

Menurut Lesson 02:

**Syarat Hermitian:**

$$
M^\dagger=M
$$

**Syarat Unitary:**

$$
M^\dagger M=MM^\dagger=I
$$

dengan:

$$
I=\begin{pmatrix}1&0\\0&1\end{pmatrix}
$$

### a. Matriks $A$

**Pemeriksaan Hermitian:**

$$
A^\dagger=
\begin{pmatrix}
2&1-i\\
1+i&3
\end{pmatrix}=A
$$

Maka:

$$
\boxed{A\text{ adalah Hermitian}}
$$

**Pemeriksaan Unitary:**

Karena $A^\dagger=A$, hitung $A^\dagger A=A^2$.

$$
\begin{aligned}
A^\dagger A
&=
\begin{pmatrix}
2&1-i\\
1+i&3
\end{pmatrix}
\begin{pmatrix}
2&1-i\\
1+i&3
\end{pmatrix}\\
&=
\begin{pmatrix}
4+(1-i)(1+i)&2(1-i)+3(1-i)\\
2(1+i)+3(1+i)&(1+i)(1-i)+9
\end{pmatrix}\\
&=
\begin{pmatrix}
6&5-5i\\
5+5i&11
\end{pmatrix}
\end{aligned}
$$

Hasil tersebut tidak sama dengan matriks identitas.

$$
\boxed{A\text{ bukan Unitary}}
$$

### b. Matriks $S$

**Pemeriksaan Hermitian:**

$$
S^\dagger=
\begin{pmatrix}
1&0\\
0&-i
\end{pmatrix}
\neq
\begin{pmatrix}
1&0\\
0&i
\end{pmatrix}=S
$$

Maka:

$$
\boxed{S\text{ bukan Hermitian}}
$$

**Pemeriksaan Unitary:**

$$
\begin{aligned}
S^\dagger S
&=
\begin{pmatrix}
1&0\\
0&-i
\end{pmatrix}
\begin{pmatrix}
1&0\\
0&i
\end{pmatrix}\\
&=
\begin{pmatrix}
1&0\\
0&(-i)(i)
\end{pmatrix}\\
&=
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix}\\
&=I
\end{aligned}
$$

Selain itu, $SS^\dagger=I$ juga berlaku.

$$
\boxed{S\text{ adalah Unitary}}
$$

### c. Matriks $B$

**Pemeriksaan Hermitian:**

$$
B^\dagger=
\begin{pmatrix}
1&0\\
1&1
\end{pmatrix}
\neq
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}=B
$$

Maka:

$$
\boxed{B\text{ bukan Hermitian}}
$$

**Pemeriksaan Unitary:**

$$
\begin{aligned}
B^\dagger B
&=
\begin{pmatrix}
1&0\\
1&1
\end{pmatrix}
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}\\
&=
\begin{pmatrix}
1&1\\
1&2
\end{pmatrix}
\end{aligned}
$$

Hasil tidak sama dengan matriks identitas.

$$
\boxed{B\text{ bukan Unitary}}
$$

### Ringkasan Task 3 nomor 2

| Matriks | Hermitian | Unitary |
| ------- | --------- | ------- |
| $A$   | Ya        | Tidak   |
| $S$   | Tidak     | Ya      |
| $B$   | Tidak     | Tidak   |

## 3 Hitung $S|+\rangle$. State apa yang dihasilkan? _(Hint: bandingkan dengan eigenvector Pauli Y.)_

Diketahui:

$$
S=\begin{pmatrix}1&0\\0&i\end{pmatrix}
$$

$$
|+\rangle=\frac{1}{\sqrt{2}}
\begin{pmatrix}1\\1\end{pmatrix}
$$

Kalikan matriks dengan vektor:

$$
\begin{aligned}
S|+\rangle
&=
\begin{pmatrix}1&0\\0&i\end{pmatrix}
\frac{1}{\sqrt{2}}
\begin{pmatrix}1\\1\end{pmatrix}\\
&=\frac{1}{\sqrt{2}}
\begin{pmatrix}
1(1)+0(1)\\
0(1)+i(1)
\end{pmatrix}\\
&=\frac{1}{\sqrt{2}}
\begin{pmatrix}1\\i\end{pmatrix}
\end{aligned}
$$

Jadi:

$$
\boxed{
S|+\rangle=
\frac{1}{\sqrt{2}}
\begin{pmatrix}1\\i\end{pmatrix}
=|+i\rangle
}
$$

State yang dihasilkan adalah eigenvector Pauli $Y$ dengan eigenvalue $+1$, sesuai tabel eigenvector Pauli pada Lesson 02.

## 4 Hitung $HZH$ dan $HXH$, dengan $H$ adalah Hadamard. Apa yang Anda amati?

Matriks Hadamard dan Pauli:

$$
H=\frac{1}{\sqrt{2}}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}
$$

$$
Z=\begin{pmatrix}1&0\\0&-1\end{pmatrix},
\qquad
X=\begin{pmatrix}0&1\\1&0\end{pmatrix}
$$

### a. Menghitung $HZH$

$$
\begin{aligned}
HZH
&=\frac{1}{\sqrt{2}}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}
\begin{pmatrix}1&0\\0&-1\end{pmatrix}
\frac{1}{\sqrt{2}}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}\\
&=\frac{1}{2}
\begin{pmatrix}1&-1\\1&1\end{pmatrix}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}\\
&=\frac{1}{2}
\begin{pmatrix}
1-1&1+1\\
1+1&1-1
\end{pmatrix}\\
&=\frac{1}{2}
\begin{pmatrix}0&2\\2&0\end{pmatrix}
\end{aligned}
$$

$$
\boxed{HZH=X}
$$

### b. Menghitung $HXH$

$$
\begin{aligned}
HXH
&=\frac{1}{\sqrt{2}}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}
\begin{pmatrix}0&1\\1&0\end{pmatrix}
\frac{1}{\sqrt{2}}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}\\
&=\frac{1}{2}
\begin{pmatrix}1&1\\-1&1\end{pmatrix}
\begin{pmatrix}1&1\\1&-1\end{pmatrix}\\
&=\frac{1}{2}
\begin{pmatrix}
1+1&1-1\\
-1+1&-1-1
\end{pmatrix}\\
&=\frac{1}{2}
\begin{pmatrix}2&0\\0&-2\end{pmatrix}\\
&=\boxed{\begin{pmatrix}1&0\\0&-1\end{pmatrix}=Z}
\end{aligned}
$$

## 5 Hitung commutator $[X, Y]$ dan nyatakan hasilnya dalam bentuk kelipatan salah satu Pauli matrix.

Definisi commutator:

$$
[X,Y]=XY-YX
$$

Matriks Pauli:

$$
X=\begin{pmatrix}0&1\\1&0\end{pmatrix},
\qquad
Y=\begin{pmatrix}0&-i\\i&0\end{pmatrix}
$$

Hitung $XY$:

$$
\begin{aligned}
XY
&=
\begin{pmatrix}0&1\\1&0\end{pmatrix}
\begin{pmatrix}0&-i\\i&0\end{pmatrix}\\
&=\begin{pmatrix}i&0\\0&-i\end{pmatrix}\\
&=iZ
\end{aligned}
$$

Hitung $YX$:

$$
\begin{aligned}
YX
&=
\begin{pmatrix}0&-i\\i&0\end{pmatrix}
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
&=2iZ
\end{aligned}
$$

$$
\boxed{[X,Y]=2iZ}
$$

## 6 Tunjukkan bahwa $X^2 = Y^2 = Z^2 = I$.

### a. Membuktikan $X^2=I$

$$
\begin{aligned}
X^2
&=\begin{pmatrix}0&1\\1&0\end{pmatrix}
\begin{pmatrix}0&1\\1&0\end{pmatrix}\\
&=\begin{pmatrix}1&0\\0&1\end{pmatrix}\\
&=\boxed{I}
\end{aligned}
$$

### b. Membuktikan $Y^2=I$

$$
\begin{aligned}
Y^2
&=\begin{pmatrix}0&-i\\i&0\end{pmatrix}
\begin{pmatrix}0&-i\\i&0\end{pmatrix}\\
&=\begin{pmatrix}
(-i)(i)&0\\
0&i(-i)
\end{pmatrix}\\
&=\begin{pmatrix}1&0\\0&1\end{pmatrix}\\
&=\boxed{I}
\end{aligned}
$$

### c. Membuktikan $Z^2=I$

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

## 7 Mengapa $B$ **tidak bisa** menjadi quantum gate? Tunjukkan dengan contoh state ternormalisasi yang norm-nya berubah setelah dikenai $B$.

Menurut Lesson 02, quantum gate harus berupa matriks unitary:

$$
U^\dagger U=I
$$

Sifat unitary menjaga norm state sehingga probabilitas total tetap 1.

Dari nomor 3.2 telah diperoleh:

$$
B^\dagger B=
\begin{pmatrix}1&1\\1&2\end{pmatrix}
\neq I
$$

Untuk memperlihatkan perubahan norm, gunakan contoh state ternormalisasi:

$$
|\psi\rangle=|+\rangle=
\frac{1}{\sqrt{2}}
\begin{pmatrix}1\\1\end{pmatrix}
$$

Norm awal:

$$
\begin{aligned}
\|\psi\|
&=\sqrt{\frac{1}{2}+\frac{1}{2}}\\
&=1
\end{aligned}
$$

Terapkan matriks $B$:

$$
\begin{aligned}
B|\psi\rangle
&=
\begin{pmatrix}1&1\\0&1\end{pmatrix}
\frac{1}{\sqrt{2}}
\begin{pmatrix}1\\1\end{pmatrix}\\
&=\frac{1}{\sqrt{2}}
\begin{pmatrix}2\\1\end{pmatrix}
\end{aligned}
$$

Hitung norm hasil:

$$
\begin{aligned}
\|B|\psi\rangle\|
&=\sqrt{\left|\frac{2}{\sqrt{2}}\right|^2+
\left|\frac{1}{\sqrt{2}}\right|^2}\\
&=\sqrt{\frac{4}{2}+\frac{1}{2}}\\
&=\sqrt{\frac{5}{2}}\\
&\approx1{,}581
\end{aligned}
$$

Karena:

$$
\sqrt{\frac{5}{2}}\neq1
$$

maka norm state berubah setelah dikenai matriks $B$.

$$
\boxed{B\text{ bukan quantum gate karena tidak unitary}}
$$

---

# Task 4 — Eigenvalue & Eigenvector

Rumus dasar eigenvalue dan eigenvector:

$$
A|v\rangle=\lambda|v\rangle
$$

Untuk mencari eigenvalue:

$$
\boxed{\det(A-\lambda I)=0}
$$

Untuk mencari eigenvector:

$$
\boxed{(A-\lambda I)|v\rangle=0}
$$

## 1 Hitung eigenvalue dan eigenvector ternormalisasi dari **Pauli Y** secara manual.

Dik:

$$
Y=\begin{pmatrix}0&-i\\i&0\end{pmatrix}
$$

### a. Mencari eigenvalue

$$
\det(Y-\lambda I)=0
$$

$$
\begin{aligned}
\det
\begin{pmatrix}
-\lambda&-i\\
i&-\lambda
\end{pmatrix}
&=0\\
(-\lambda)(-\lambda)-(-i)(i)&=0\\
\lambda^2-1&=0
\end{aligned}
$$

Faktorkan:

$$
(\lambda-1)(\lambda+1)=0
$$

Maka:

$$
\boxed{\lambda_1=+1,\qquad\lambda_2=-1}
$$

### b. Mencari eigenvector untuk $\lambda=+1$

Gunakan:

$$
(Y-I)|v\rangle=0
$$

$$
\begin{pmatrix}
-1&-i\\
i&-1
\end{pmatrix}
\begin{pmatrix}x\\y\end{pmatrix}
=
\begin{pmatrix}0\\0\end{pmatrix}
$$

Persamaan baris pertama:

$$
-x-iy=0
$$

$$
x=-iy
$$

Ambil $y=i$, sehingga $x=1$.

Vektor:

$$
|v\_+\rangle=\begin{pmatrix}1\\i\end{pmatrix}
$$

Norm:

$$
\|v\_+\|=\sqrt{|1|^2+|i|^2}=\sqrt{2}
$$

Normalisasi:

$$
\boxed{
|v\_+\rangle=
\frac{1}{\sqrt{2}}
\begin{pmatrix}1\\i\end{pmatrix}
=|+i\rangle
}
$$

### c. Mencari eigenvector untuk $\lambda=-1$

Gunakan:

$$
(Y+I)|v\rangle=0
$$

$$
\begin{pmatrix}
1&-i\\
i&1
\end{pmatrix}
\begin{pmatrix}x\\y\end{pmatrix}
=
\begin{pmatrix}0\\0\end{pmatrix}
$$

Persamaan baris pertama:

$$
x-iy=0
$$

$$
x=iy
$$

Ambil $y=-i$, sehingga $x=1$.

Vektor:

$$
|v\_-\rangle=\begin{pmatrix}1\\-i\end{pmatrix}
$$

Norm:

$$
\|v\_-\|=\sqrt{|1|^2+|-i|^2}=\sqrt{2}
$$

Normalisasi:

$$
\boxed{
|v\_-\rangle=
\frac{1}{\sqrt{2}}
\begin{pmatrix}1\\-i\end{pmatrix}
=|-i\rangle
}
$$

**Hasil akhir:**

| Eigenvalue | Eigenvector ternormalisasi                              |
| ---------- | ------------------------------------------------------- |
| $+1$     | $\frac{1}{\sqrt{2}}\begin{pmatrix}1\\i\end{pmatrix}$  |
| $-1$     | $\frac{1}{\sqrt{2}}\begin{pmatrix}1\\-i\end{pmatrix}$ |

## 2 Hitung eigenvalue dan eigenvector ternormalisasi dari matriks $A$ pada Task 3. Apakah eigenvalue-nya real? Mengapa hal ini sudah dapat diprediksi?

Dari Task 3:

$$
A=\begin{pmatrix}
2&1-i\\
1+i&3
\end{pmatrix}
$$

### a. Mencari eigenvalue

Gunakan persamaan karakteristik:

$$
\det(A-\lambda I)=0
$$

$$
\begin{aligned}
\det
\begin{pmatrix}
2-\lambda&1-i\\
1+i&3-\lambda
\end{pmatrix}
&=0\\
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
\lambda^2-5\lambda+4&=0
\end{aligned}
$$

Faktorkan:

$$
(\lambda-1)(\lambda-4)=0
$$

Jadi:

$$
\boxed{\lambda_1=1,\qquad\lambda_2=4}
$$

### b. Mencari eigenvector untuk $\lambda=1$

Gunakan:

$$
(A-I)|v_1\rangle=0
$$

$$
\begin{pmatrix}
1&1-i\\
1+i&2
\end{pmatrix}
\begin{pmatrix}x\\y\end{pmatrix}
=
\begin{pmatrix}0\\0\end{pmatrix}
$$

Persamaan baris pertama:

$$
x+(1-i)y=0
$$

$$
x=-(1-i)y=(-1+i)y
$$

Ambil $y=1$, maka $x=-1+i$.

Vektor:

$$
|v_1\rangle=
\begin{pmatrix}-1+i\\1\end{pmatrix}
$$

Hitung norm:

$$
\begin{aligned}
\|v_1\|
&=\sqrt{|-1+i|^2+|1|^2}\\
&=\sqrt{((-1)^2+1^2)+1}\\
&=\sqrt{3}
\end{aligned}
$$

Normalisasi:

$$
\boxed{
|v_1\rangle=
\frac{1}{\sqrt{3}}
\begin{pmatrix}-1+i\\1\end{pmatrix}
}
$$

### c. Mencari eigenvector untuk $\lambda=4$

Gunakan:

$$
(A-4I)|v_2\rangle=0
$$

$$
\begin{pmatrix}
-2&1-i\\
1+i&-1
\end{pmatrix}
\begin{pmatrix}x\\y\end{pmatrix}
=
\begin{pmatrix}0\\0\end{pmatrix}
$$

Persamaan baris pertama:

$$
-2x+(1-i)y=0
$$

$$
2x=(1-i)y
$$

$$
x=\frac{1-i}{2}y
$$

Ambil $y=2$, maka $x=1-i$.

Vektor:

$$
|v_2\rangle=
\begin{pmatrix}1-i\\2\end{pmatrix}
$$

Hitung norm:

$$
\begin{aligned}
\|v_2\|
&=\sqrt{|1-i|^2+|2|^2}\\
&=\sqrt{(1^2+(-1)^2)+4}\\
&=\sqrt{6}
\end{aligned}
$$

Normalisasi:

$$
\boxed{
|v_2\rangle=
\frac{1}{\sqrt{6}}
\begin{pmatrix}1-i\\2\end{pmatrix}
}
$$

### d. Apakah eigenvalue real? Mengapa?

Hasil eigenvalue:

$$
\lambda_1=1,\qquad\lambda_2=4
$$

Keduanya merupakan bilangan real.

Hal ini dapat diprediksi karena matriks $A$ adalah Hermitian:

$$
A^\dagger=A
$$

Berdasarkan Lesson 02, eigenvalue dari matriks Hermitian selalu real.

$$
\boxed{\text{Kedua eigenvalue real karena }A\text{ Hermitian}}
$$

## 3 Verifikasi bahwa kedua eigenvector dari $A$ saling ortogonal.

Dari nomor 2:

$$
|v_1\rangle=
\frac{1}{\sqrt{3}}
\begin{pmatrix}-1+i\\1\end{pmatrix}
$$

$$
|v_2\rangle=
\frac{1}{\sqrt{6}}
\begin{pmatrix}1-i\\2\end{pmatrix}
$$

Bra dari eigenvector pertama:

$$
\langle v_1|=
\frac{1}{\sqrt{3}}
\begin{pmatrix}-1-i&1\end{pmatrix}
$$

Hitung inner product:

$$
\begin{aligned}
\langle v_1|v_2\rangle
&=\frac{1}{\sqrt{3}}\begin{pmatrix}-1-i&1\end{pmatrix}
\frac{1}{\sqrt{6}}
\begin{pmatrix}1-i\\2\end{pmatrix}\\
&=\frac{1}{\sqrt{18}}
\left[(-1-i)(1-i)+(1)(2)\right]
\end{aligned}
$$

Hitung:

$$
\begin{aligned}
(-1-i)(1-i)
&=-1+i-i+i^2\\
&=-1-1\\
&=-2
\end{aligned}
$$

Maka:

$$
\begin{aligned}
\langle v_1|v_2\rangle
&=\frac{1}{\sqrt{18}}(-2+2)\\
&=\boxed{0}
\end{aligned}
$$

## 4 Hitung eigenvalue dari Hadamard $H$.

Dik:

$$
H=\frac{1}{\sqrt{2}}
\begin{pmatrix}
1&1\\
1&-1
\end{pmatrix}
$$

Cari eigenvalue dengan:

$$
\det(H-\lambda I)=0
$$

$$
\begin{aligned}
\det
\begin{pmatrix}
\frac{1}{\sqrt{2}}-\lambda&\frac{1}{\sqrt{2}}\\
\frac{1}{\sqrt{2}}&-\frac{1}{\sqrt{2}}-\lambda
\end{pmatrix}
&=0
\end{aligned}
$$

$$
\begin{aligned}
\left(\frac{1}{\sqrt{2}}-\lambda\right)
\left(-\frac{1}{\sqrt{2}}-\lambda\right)
-\frac{1}{2}&=0\\
\left(\lambda^2-\frac{1}{2}\right)-\frac{1}{2}&=0\\
\lambda^2-1&=0
\end{aligned}
$$

Faktorkan:

$$
(\lambda-1)(\lambda+1)=0
$$

Maka:

$$
\boxed{\lambda_1=+1,\qquad\lambda_2=-1}
$$

## 5 Tuliskan Pauli Z dalam bentuk **outer product**: $Z = \sum_k \lambda_k |v_k\rangle\langle v_k|$ (_spectral decomposition_).

Dik:

$$
Z=\begin{pmatrix}1&0\\0&-1\end{pmatrix}
$$

Eigenvalue dan eigenvector Pauli $Z$:

$$
\lambda_1=+1,\quad |v_1\rangle=|0\rangle=
\begin{pmatrix}1\\0\end{pmatrix}
$$

$$
\lambda_2=-1,\quad |v_2\rangle=|1\rangle=
\begin{pmatrix}0\\1\end{pmatrix}
$$

Rumus spectral decomposition:

$$
Z=\sum_k\lambda_k|v_k\rangle\langle v_k|
$$

Substitusi:

$$
Z=(+1)|0\rangle\langle0|+(-1)|1\rangle\langle1|
$$

Hitung outer product pertama:

$$
|0\rangle\langle0|=
\begin{pmatrix}1\\0\end{pmatrix}
\begin{pmatrix}1&0\end{pmatrix}
=
\begin{pmatrix}1&0\\0&0\end{pmatrix}
$$

Hitung outer product kedua:

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
Z
&=\begin{pmatrix}1&0\\0&0\end{pmatrix}
-\begin{pmatrix}0&0\\0&1\end{pmatrix}\\
&=\begin{pmatrix}1&0\\0&-1\end{pmatrix}
\end{aligned}
$$

$$
\boxed{Z=|0\rangle\langle0|-|1\rangle\langle1|}
$$
