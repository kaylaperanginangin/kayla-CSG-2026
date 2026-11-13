# Task 1 — Bilangan Kompleks

Diketahui:

$$
z_1 = 1 + i, \qquad z_2 = \sqrt{3} - i
$$

## 1. Hitung $z_1 + z_2$, $z_1 z_2$, $z_1^*$, dan $z_1 / z_2$

### a. Penjumlahan $z_1 + z_2$

$$
\begin{aligned}
z_1 + z_2 &= (1 + i) + (\sqrt{3} - i) \\
&= (1 + \sqrt{3}) + (1 - 1)i \\
&= \boxed{1 + \sqrt{3}}
\end{aligned}
$$

### b. Perkalian $z_1 z_2$

Ingat bahwa $i^2 = -1$, sehingga:

$$
\begin{aligned}
z_1 z_2 &= (1 + i)(\sqrt{3} - i) \\
&= \sqrt{3} - i + i\sqrt{3} - i^2 \\
&= \sqrt{3} - i + i\sqrt{3} - (-1) \\
&= \boxed{(\sqrt{3} + 1) + (\sqrt{3} - 1)i}
\end{aligned}
$$

### c. Konjugat kompleks $z_1^*$

Untuk $z = a + bi$, konjugatnya adalah $z^* = a - bi$:

$$
z_1 = 1 + i \;\Rightarrow\; \boxed{z_1^* = 1 - i}
$$

### d. Pembagian $z_1 / z_2$

Kalikan pembilang dan penyebut dengan konjugat penyebut ($z_2^* = \sqrt{3} + i$):

$$
\begin{aligned}
\frac{z_1}{z_2} &= \frac{1 + i}{\sqrt{3} - i} \cdot \frac{\sqrt{3} + i}{\sqrt{3} + i} \\
&= \frac{\sqrt{3} + i + i\sqrt{3} + i^2}{(\sqrt{3})^2 - i^2} \\
&= \frac{\sqrt{3} - 1 + (1 + \sqrt{3})i}{3 - (-1)} \\
&= \boxed{\frac{\sqrt{3} - 1}{4} + \frac{1 + \sqrt{3}}{4}i}
\end{aligned}
$$

---

## 2. Hitung $|z_1|$, $|z_2|$, dan $|z_1 z_2|$. Verifikasi bahwa $|z_1 z_2| = |z_1||z_2|$

Modulus didefinisikan sebagai $|z| = \sqrt{a^2 + b^2} = \sqrt{z z^*}$:

* **Modulus $z_1$:**
  $$
  |z_1| = \sqrt{1^2 + 1^2} = \boxed{\sqrt{2}}
  $$

* **Modulus $z_2$:**
  $$
  |z_2| = \sqrt{(\sqrt{3})^2 + (-1)^2} = \sqrt{3 + 1} = \boxed{2}
  $$

* **Modulus $z_1 z_2$:**
  Dari hasil bagian 1b, $z_1 z_2 = (\sqrt{3} + 1) + (\sqrt{3} - 1)i$, sehingga:
  $$
  \begin{aligned}
  |z_1 z_2| &= \sqrt{(\sqrt{3} + 1)^2 + (\sqrt{3} - 1)^2} \\
  &= \sqrt{(3 + 2\sqrt{3} + 1) + (3 - 2\sqrt{3} + 1)} \\
  &= \sqrt{8} = \boxed{2\sqrt{2}}
  \end{aligned}
  $$

* **Verifikasi:**
  $$
  |z_1||z_2| = \sqrt{2} \cdot 2 = 2\sqrt{2} = |z_1 z_2| \quad (\text{Terbukti})
  $$

---

## 3. Tuliskan $z_1$ dan $z_2$ dalam bentuk polar $r e^{i\theta}$

Bentuk polar bilangan kompleks adalah $z = r e^{i\theta}$ dengan $r = |z|$ dan $\theta = \text{atan2}(b, a)$.

* **Untuk $z_1 = 1 + i$:**
  Titik $(1, 1)$ berada di Kuadran I:
  $$
  r_1 = \sqrt{2}, \qquad \theta_1 = \tan^{-1}\left(\frac{1}{1}\right) = \frac{\pi}{4}
  $$
  Maka:
  $$
  \boxed{z_1 = \sqrt{2}\,e^{i\pi/4}}
  $$

* **Untuk $z_2 = \sqrt{3} - i$:**
  Titik $(\sqrt{3}, -1)$ berada di Kuadran IV:
  $$
  r_2 = 2, \qquad \theta_2 = \tan^{-1}\left(\frac{-1}{\sqrt{3}}\right) = -\frac{\pi}{6}
  $$
  Maka:
  $$
  \boxed{z_2 = 2\,e^{-i\pi/6}}
  $$

---

## 4. Gunakan bentuk polar untuk menghitung $z_1^8$

Gunakan $z_1 = \sqrt{2}\,e^{i\pi/4}$ dan formula Euler $e^{i\theta} = \cos\theta + i\sin\theta$:

$$
\begin{aligned}
z_1^8 &= \left(\sqrt{2}\,e^{i\pi/4}\right)^8 \\
&= (\sqrt{2})^8 \cdot e^{i(8 \cdot \pi/4)} \\
&= 2^4 \cdot e^{i2\pi} \\
&= 16(\cos 2\pi + i\sin 2\pi) \\
&= 16(1 + 0) = \boxed{16}
\end{aligned}
$$

---

## 5. Tunjukkan bahwa $|e^{i\theta}|^2 = 1$ untuk sembarang $\theta$ real

Menggunakan formula Euler $e^{i\theta} = \cos\theta + i\sin\theta$ serta identitas $|z|^2 = z z^*$:

$$
\begin{aligned}
|e^{i\theta}|^2 &= e^{i\theta} \left(e^{i\theta}\right)^* \\
&= (\cos\theta + i\sin\theta)(\cos\theta - i\sin\theta) \\
&= \cos^2\theta - i^2\sin^2\theta \\
&= \cos^2\theta + \sin^2\theta = \boxed{1}
\end{aligned}
$$

---

# Task 2 — State, Inner Product, & Normalisasi

Diketahui:

$$
|a\rangle = \begin{pmatrix} 1 \\ 2i \end{pmatrix}, \qquad
|b\rangle = \begin{pmatrix} 2 \\ -i \end{pmatrix}, \qquad
|c\rangle = \frac{1}{2}|0\rangle + \frac{\sqrt{3}}{2}e^{i\pi/4}|1\rangle
$$

## 1. Tuliskan $\langle a|$ dan $\langle b|$

Bra adalah *conjugate transpose* dari ket ($\langle\psi| = (|\psi\rangle)^*$ dalam bentuk baris):

$$
\boxed{\langle a| = \begin{pmatrix} 1 & -2i \end{pmatrix}}, \qquad
\boxed{\langle b| = \begin{pmatrix} 2 & i \end{pmatrix}}
$$

---

## 2. Hitung $\langle a|b\rangle$ dan $\langle b|a\rangle$. Verifikasi bahwa $\langle a|b\rangle = \langle b|a\rangle^*$

Menggunakan rumus $\langle\phi|\psi\rangle = \phi_1^*\psi_1 + \phi_2^*\psi_2$:

$$
\begin{aligned}
\langle a|b\rangle &= \begin{pmatrix} 1 & -2i \end{pmatrix} \begin{pmatrix} 2 \\ -i \end{pmatrix} = (1)(2) + (-2i)(-i) = 2 + 2i^2 = 2 - 2 = \boxed{0} \\
\langle b|a\rangle &= \begin{pmatrix} 2 & i \end{pmatrix} \begin{pmatrix} 1 \\ 2i \end{pmatrix} = (2)(1) + (i)(2i) = 2 + 2i^2 = 2 - 2 = \boxed{0}
\end{aligned}
$$

**Verifikasi:**

$$
\langle b|a\rangle^* = 0^* = 0 = \langle a|b\rangle \quad (\text{Terbukti})
$$

---

## 3. Apakah $|a\rangle$ dan $|b\rangle$ ortogonal?

**Ya**, karena inner product keduanya bernilai nol ($\langle a|b\rangle = 0$).

---

## 4. Normalisasi $|a\rangle$ dan $|b\rangle$

Norm vektor didefinisikan sebagai $\|\psi\| = \sqrt{\langle\psi|\psi\rangle}$, dan vektor ternormalisasi adalah $\dfrac{|\psi\rangle}{\|\psi\|}$:

* **Normalisasi $|a\rangle$:**
  $$
  \|a\| = \sqrt{\langle a|a\rangle} = \sqrt{(1)(1) + (-2i)(2i)} = \sqrt{1 - 4i^2} = \sqrt{1 + 4} = \sqrt{5}
  $$
  $$
  \boxed{|a_{\text{norm}}\rangle = \frac{1}{\sqrt{5}}\begin{pmatrix} 1 \\ 2i \end{pmatrix}}
  $$

* **Normalisasi $|b\rangle$:**
  $$
  \|b\| = \sqrt{\langle b|b\rangle} = \sqrt{(2)(2) + (i)(-i)} = \sqrt{4 - i^2} = \sqrt{4 + 1} = \sqrt{5}
  $$
  $$
  \boxed{|b_{\text{norm}}\rangle = \frac{1}{\sqrt{5}}\begin{pmatrix} 2 \\ -i \end{pmatrix}}
  $$

---

## 5. Apakah $|c\rangle$ sudah ternormalisasi? Hitung $P(0)$ dan $P(1)$ jika $|c\rangle$ diukur di computational basis

* **Cek normalisasi:**
  Syarat state ternormalisasi adalah $\langle c|c\rangle = |\alpha|^2 + |\beta|^2 = 1$:
  $$
  \begin{aligned}
  \langle c|c\rangle &= \left|\frac{1}{2}\right|^2 + \left|\frac{\sqrt{3}}{2}e^{i\pi/4}\right|^2 \\
  &= \frac{1}{4} + \frac{3}{4}\underbrace{|e^{i\pi/4}|^2}_{=1} \\
  &= \frac{1}{4} + \frac{3}{4} = 1
  \end{aligned}
  $$
  Karena $\langle c|c\rangle = 1$, maka **$|c\rangle$ sudah ternormalisasi**.

* **Probabilitas pengukuran (Born rule $P(k) = |\langle k|c\rangle|^2$):**
  $$
  \begin{aligned}
  P(0) &= |\langle 0|c\rangle|^2 = \left|\frac{1}{2}\right|^2 = \boxed{\frac{1}{4}} \\
  P(1) &= |\langle 1|c\rangle|^2 = \left|\frac{\sqrt{3}}{2}e^{i\pi/4}\right|^2 = \boxed{\frac{3}{4}}
  \end{aligned}
  $$

---

## 6. Tuliskan $|c\rangle$ dalam Hadamard basis $\{|+\rangle, |-\rangle\}$, lalu hitung $P(+)$ dan $P(-)$

Diketahui $|+\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ 1 \end{pmatrix}$, $|-\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ -1 \end{pmatrix}$, dan $|c\rangle = \begin{pmatrix} \frac{1}{2} \\ \frac{\sqrt{3}}{2}e^{i\pi/4} \end{pmatrix}$.

* **Koefisien ekspansi $|c\rangle = c_+|+\rangle + c_-|-\rangle$:**
  $$
  \begin{aligned}
  c_+ &= \langle +|c\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \end{pmatrix}\begin{pmatrix} \frac{1}{2} \\ \frac{\sqrt{3}}{2}e^{i\pi/4} \end{pmatrix} = \frac{1 + \sqrt{3}e^{i\pi/4}}{2\sqrt{2}} \\
  c_- &= \langle -|c\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & -1 \end{pmatrix}\begin{pmatrix} \frac{1}{2} \\ \frac{\sqrt{3}}{2}e^{i\pi/4} \end{pmatrix} = \frac{1 - \sqrt{3}e^{i\pi/4}}{2\sqrt{2}}
  \end{aligned}
  $$

  Sehingga dalam Hadamard basis:
  $$
  \boxed{|c\rangle = \frac{1 + \sqrt{3}e^{i\pi/4}}{2\sqrt{2}}|+\rangle + \frac{1 - \sqrt{3}e^{i\pi/4}}{2\sqrt{2}}|-\rangle}
  $$

* **Probabilitas $P(+)$ dan $P(-)$:**
  Jabarkan $e^{i\pi/4} = \cos\frac{\pi}{4} + i\sin\frac{\pi}{4} = \frac{\sqrt{2}}{2} + i\frac{\sqrt{2}}{2}$, maka $\sqrt{3}e^{i\pi/4} = \frac{\sqrt{6}}{2} + i\frac{\sqrt{6}}{2}$:

  $$
  \begin{aligned}
  P(+) &= |\langle +|c\rangle|^2 = \left|\frac{\left(1 + \frac{\sqrt{6}}{2}\right) + i\frac{\sqrt{6}}{2}}{2\sqrt{2}}\right|^2 \\
  &= \frac{\left(1 + \frac{\sqrt{6}}{2}\right)^2 + \left(\frac{\sqrt{6}}{2}\right)^2}{8} \\
  &= \frac{1 + \sqrt{6} + \frac{6}{4} + \frac{6}{4}}{8} = \boxed{\frac{4 + \sqrt{6}}{8}} \approx 0{,}8062
  \end{aligned}
  $$

  $$
  \begin{aligned}
  P(-) &= |\langle -|c\rangle|^2 = \left|\frac{\left(1 - \frac{\sqrt{6}}{2}\right) - i\frac{\sqrt{6}}{2}}{2\sqrt{2}}\right|^2 \\
  &= \frac{\left(1 - \frac{\sqrt{6}}{2}\right)^2 + \left(-\frac{\sqrt{6}}{2}\right)^2}{8} \\
  &= \frac{1 - \sqrt{6} + \frac{6}{4} + \frac{6}{4}}{8} = \boxed{\frac{4 - \sqrt{6}}{8}} \approx 0{,}1938
  \end{aligned}
  $$

---

## 7. Buktikan bahwa $\{|+\rangle, |-\rangle\}$ adalah basis ortonormal

Syarat basis ortonormal adalah $\langle e_i|e_j\rangle = \delta_{ij}$ (norm masing-masing 1 dan saling ortogonal):

1. $\langle +|+\rangle = \frac{1}{2}\begin{pmatrix} 1 & 1 \end{pmatrix}\begin{pmatrix} 1 \\ 1 \end{pmatrix} = \frac{1 + 1}{2} = 1$
2. $\langle -|-\rangle = \frac{1}{2}\begin{pmatrix} 1 & -1 \end{pmatrix}\begin{pmatrix} 1 \\ -1 \end{pmatrix} = \frac{1 + 1}{2} = 1$
3. $\langle +|-\rangle = \frac{1}{2}\begin{pmatrix} 1 & 1 \end{pmatrix}\begin{pmatrix} 1 \\ -1 \end{pmatrix} = \frac{1 - 1}{2} = 0$

Karena $\langle +|+\rangle = \langle -|-\rangle = 1$ dan $\langle +|-\rangle = \langle -|+\rangle = 0$, maka **terbukti $\{|+\rangle, |-\rangle\}$ adalah basis ortonormal**.

---

# Task 3 — Operator: Hermitian, Unitary, Commutator

Diketahui:

$$
A = \begin{pmatrix} 2 & 1 - i \\ 1 + i & 3 \end{pmatrix}, \qquad
S = \begin{pmatrix} 1 & 0 \\ 0 & i \end{pmatrix}, \qquad
B = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}
$$

## 1. Hitung $A^\dagger$, $S^\dagger$, dan $B^\dagger$

Dengan definisi $M^\dagger = (M^*)^T$ (transpose lalu konjugasi setiap elemen):

* $A^T = \begin{pmatrix} 2 & 1 + i \\ 1 - i & 3 \end{pmatrix} \;\Rightarrow\; \boxed{A^\dagger = \begin{pmatrix} 2 & 1 - i \\ 1 + i & 3 \end{pmatrix}}$
* $S^T = \begin{pmatrix} 1 & 0 \\ 0 & i \end{pmatrix} \;\Rightarrow\; \boxed{S^\dagger = \begin{pmatrix} 1 & 0 \\ 0 & -i \end{pmatrix}}$
* $B^T = \begin{pmatrix} 1 & 0 \\ 1 & 1 \end{pmatrix} \;\Rightarrow\; \boxed{B^\dagger = \begin{pmatrix} 1 & 0 \\ 1 & 1 \end{pmatrix}}$

---

## 2. Tentukan mana yang Hermitian dan mana yang unitary

Syarat: **Hermitian** jika $M^\dagger = M$; **Unitary** jika $M^\dagger M = M M^\dagger = I$.

### a. Matriks $A$
* **Hermitian:** $A^\dagger = \begin{pmatrix} 2 & 1 - i \\ 1 + i & 3 \end{pmatrix} = A$ (**Ya, Hermitian**).
* **Unitary:**
  $$
  A^\dagger A = \begin{pmatrix} 2 & 1 - i \\ 1 + i & 3 \end{pmatrix}\begin{pmatrix} 2 & 1 - i \\ 1 + i & 3 \end{pmatrix} = \begin{pmatrix} 4 + 2 & 2(1-i) + 3(1-i) \\ 2(1+i) + 3(1+i) & 2 + 9 \end{pmatrix} = \begin{pmatrix} 6 & 5 - 5i \\ 5 + 5i & 11 \end{pmatrix} \neq I
  $$
  (**Bukan Unitary**).

### b. Matriks $S$
* **Hermitian:** $S^\dagger = \begin{pmatrix} 1 & 0 \\ 0 & -i \end{pmatrix} \neq S$ (**Bukan Hermitian**).
* **Unitary:**
  $$
  S^\dagger S = \begin{pmatrix} 1 & 0 \\ 0 & -i \end{pmatrix}\begin{pmatrix} 1 & 0 \\ 0 & i \end{pmatrix} = \begin{pmatrix} 1 & 0 \\ 0 & -i^2 \end{pmatrix} = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} = I
  $$
  Demikian juga $S S^\dagger = I$ (**Ya, Unitary**).

### c. Matriks $B$
* **Hermitian:** $B^\dagger = \begin{pmatrix} 1 & 0 \\ 1 & 1 \end{pmatrix} \neq B$ (**Bukan Hermitian**).
* **Unitary:**
  $$
  B^\dagger B = \begin{pmatrix} 1 & 0 \\ 1 & 1 \end{pmatrix}\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 1 & 1 \\ 1 & 2 \end{pmatrix} \neq I
  $$
  (**Bukan Unitary**).

| Matriks | Hermitian | Unitary |
| :---: | :---: | :---: |
| $A$ | Ya | Tidak |
| $S$ | Tidak | Ya |
| $B$ | Tidak | Tidak |

---

## 3. Hitung $S|+\rangle$. State apa yang dihasilkan?

$$
S|+\rangle = \begin{pmatrix} 1 & 0 \\ 0 & i \end{pmatrix} \cdot \frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ 1 \end{pmatrix} = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ i \end{pmatrix} = \boxed{|+i\rangle}
$$

State yang dihasilkan adalah **$|+i\rangle$**, yaitu eigenvector dari matriks Pauli $Y$ dengan eigenvalue $+1$.

---

## 4. Hitung $HZH$ dan $HXH$. Apa yang Anda amati?

* **Menghitung $HZH$:**
  $$
  \begin{aligned}
  HZH &= \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}\begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}\frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} \\
  &= \frac{1}{2}\begin{pmatrix} 1 & -1 \\ 1 & 1 \end{pmatrix}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} \\
  &= \frac{1}{2}\begin{pmatrix} 0 & 2 \\ 2 & 0 \end{pmatrix} = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} = \boxed{X}
  \end{aligned}
  $$

* **Menghitung $HXH$:**
  $$
  \begin{aligned}
  HXH &= \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}\frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} \\
  &= \frac{1}{2}\begin{pmatrix} 1 & 1 \\ -1 & 1 \end{pmatrix}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} \\
  &= \frac{1}{2}\begin{pmatrix} 2 & 0 \\ 0 & -2 \end{pmatrix} = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix} = \boxed{Z}
  \end{aligned}
  $$

**Pengamatan:** Konjugasi oleh gerbang Hadamard ($H$) menukar basis komputasi ($Z$) dengan basis Hadamard ($X$), yakni mengubah bit-flip ($X$) menjadi phase-flip ($Z$) dan sebaliknya.

---

## 5. Hitung commutator $[X, Y]$

Gunakan $[X, Y] = XY - YX$:

$$
\begin{aligned}
XY &= \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}\begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix} = \begin{pmatrix} i & 0 \\ 0 & -i \end{pmatrix} = iZ \\
YX &= \begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix}\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} -i & 0 \\ 0 & i \end{pmatrix} = -iZ
\end{aligned}
$$

Sehingga:

$$
[X, Y] = iZ - (-iZ) = \boxed{2iZ}
$$

---

## 6. Tunjukkan bahwa $X^2 = Y^2 = Z^2 = I$

* $X^2 = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} = I$
* $Y^2 = \begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix}\begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix} = \begin{pmatrix} -i^2 & 0 \\ 0 & -i^2 \end{pmatrix} = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} = I$
* $Z^2 = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}\begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix} = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} = I$

Terbukti bahwa $\boxed{X^2 = Y^2 = Z^2 = I}$.

---

## 7. Mengapa $B$ tidak bisa menjadi quantum gate?

Quantum gate wajib berupa operator **unitary** ($U^\dagger U = I$) agar norm vektor state tetap terjaga ($\|U|\psi\rangle\| = \|\psi\| = 1$) sehingga total probabilitas pengukuran tetap bernilai $1$. Matriks $B$ **tidak unitary** ($B^\dagger B \neq I$).

**Contoh penyangkal:** Ambil state ternormalisasi $|\psi\rangle = |+\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ 1 \end{pmatrix}$ dengan $\|\psi\| = 1$. Setelah dikenai $B$:

$$
B|+\rangle = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} \cdot \frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ 1 \end{pmatrix} = \frac{1}{\sqrt{2}}\begin{pmatrix} 2 \\ 1 \end{pmatrix}
$$

Norm barunya menjadi:

$$
\|B|+\rangle\| = \sqrt{\left(\frac{2}{\sqrt{2}}\right)^2 + \left(\frac{1}{\sqrt{2}}\right)^2} = \sqrt{\frac{4}{2} + \frac{1}{2}} = \sqrt{\frac{5}{2}} \neq 1
$$

Karena melanggar kekekalan probabilitas, $B$ tidak dapat menjadi quantum gate.

---

# Task 4 — Eigenvalue & Eigenvector

## 1. Hitung eigenvalue dan eigenvector ternormalisasi dari Pauli $Y$

### a. Mencari Eigenvalue
Selesaikan persamaan karakteristik $\det(Y - \lambda I) = 0$:

$$
\det\begin{pmatrix} -\lambda & -i \\ i & -\lambda \end{pmatrix} = (-\lambda)(-\lambda) - (-i)(i) = \lambda^2 - 1 = 0 \;\Rightarrow\; \boxed{\lambda_1 = +1, \quad \lambda_2 = -1}
$$

### b. Mencari Eigenvector & Normalisasi

* **Untuk $\lambda_1 = +1$:**
  Selesaikan $(Y - I)|v\rangle = 0$:
  $$
  \begin{pmatrix} -1 & -i \\ i & -1 \end{pmatrix}\begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix} \;\Rightarrow\; -x - iy = 0 \;\Rightarrow\; y = ix
  $$
  Pilih $x = 1 \Rightarrow y = i$, didapat $|v\rangle = \begin{pmatrix} 1 \\ i \end{pmatrix}$ dengan norm $\|v\| = \sqrt{1^2 + |i|^2} = \sqrt{2}$. Setelah dinormalisasi:
  $$
  \boxed{|+i\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ i \end{pmatrix}}
  $$

* **Untuk $\lambda_2 = -1$:**
  Selesaikan $(Y + I)|v\rangle = 0$:
  $$
  \begin{pmatrix} 1 & -i \\ i & 1 \end{pmatrix}\begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix} \;\Rightarrow\; x - iy = 0 \;\Rightarrow\; y = -ix
  $$
  Pilih $x = 1 \Rightarrow y = -i$, didapat $|v\rangle = \begin{pmatrix} 1 \\ -i \end{pmatrix}$ dengan norm $\sqrt{2}$. Setelah dinormalisasi:
  $$
  \boxed{|-i\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 \\ -i \end{pmatrix}}
  $$

---

## 2. Hitung eigenvalue dan eigenvector ternormalisasi dari matriks $A$

### a. Mencari Eigenvalue
Selesaikan $\det(A - \lambda I) = 0$:

$$
\begin{aligned}
\det\begin{pmatrix} 2 - \lambda & 1 - i \\ 1 + i & 3 - \lambda \end{pmatrix} &= (2 - \lambda)(3 - \lambda) - (1 - i)(1 + i) = 0 \\
(6 - 5\lambda + \lambda^2) - (1 - i^2) &= 0 \\
\lambda^2 - 5\lambda + 4 &= 0 \\
(\lambda - 1)(\lambda - 4) &= 0 \;\Rightarrow\; \boxed{\lambda_1 = 1, \quad \lambda_2 = 4}
\end{aligned}
$$

### b. Mencari Eigenvector & Normalisasi

* **Untuk $\lambda_1 = 1$:**
  Selesaikan $(A - I)|v_1\rangle = 0$:
  $$
  \begin{pmatrix} 1 & 1 - i \\ 1 + i & 2 \end{pmatrix}\begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix} \;\Rightarrow\; x + (1 - i)y = 0 \;\Rightarrow\; x = (-1 + i)y
  $$
  Pilih $y = 1 \Rightarrow x = -1 + i$. Norm vektor: $\|v_1\| = \sqrt{|-1 + i|^2 + 1^2} = \sqrt{(1 + 1) + 1} = \sqrt{3}$.
  $$
  \boxed{|v_1\rangle = \frac{1}{\sqrt{3}}\begin{pmatrix} -1 + i \\ 1 \end{pmatrix}}
  $$

* **Untuk $\lambda_2 = 4$:**
  Selesaikan $(A - 4I)|v_2\rangle = 0$:
  $$
  \begin{pmatrix} -2 & 1 - i \\ 1 + i & -1 \end{pmatrix}\begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix} \;\Rightarrow\; (1 + i)x - y = 0 \;\Rightarrow\; y = (1 + i)x
  $$
  Pilih $x = 1 \Rightarrow y = 1 + i$. Norm vektor: $\|v_2\| = \sqrt{1^2 + |1 + i|^2} = \sqrt{1 + (1 + 1)} = \sqrt{3}$.
  $$
  \boxed{|v_2\rangle = \frac{1}{\sqrt{3}}\begin{pmatrix} 1 \\ 1 + i \end{pmatrix}}
  $$
  *(Catatan: bentuk ini ekuivalen hingga global phase dengan $\frac{1}{\sqrt{6}}\begin{pmatrix} 1 - i \\ 2 \end{pmatrix}$).*

### c. Analisis Nilai Eigenvalue
**Ya, kedua eigenvalue bernilai real** ($\lambda_1 = 1$ dan $\lambda_2 = 4$). Hal ini sudah dapat diprediksi sejak awal karena $A$ merupakan matriks **Hermitian** ($A^\dagger = A$), dan menurut sifat operator kuantum, semua matriks Hermitian pasti memiliki eigenvalue real.

---

## 3. Verifikasi bahwa kedua eigenvector dari $A$ saling ortogonal

Hitung inner product $\langle v_1|v_2\rangle$ dengan $\langle v_1| = \frac{1}{\sqrt{3}}\begin{pmatrix} -1 - i & 1 \end{pmatrix}$:

$$
\begin{aligned}
\langle v_1|v_2\rangle &= \frac{1}{\sqrt{3}}\begin{pmatrix} -1 - i & 1 \end{pmatrix} \cdot \frac{1}{\sqrt{3}}\begin{pmatrix} 1 \\ 1 + i \end{pmatrix} \\
&= \frac{1}{3}\Big[(-1 - i)(1) + (1)(1 + i)\Big] \\
&= \frac{1}{3}(-1 - i + 1 + i) = \boxed{0}
\end{aligned}
$$

Karena $\langle v_1|v_2\rangle = 0$, **terbukti kedua eigenvector saling ortogonal**.

---

## 4. Hitung eigenvalue dari Hadamard $H$

Selesaikan $\det(H - \lambda I) = 0$:

$$
\begin{aligned}
\det\begin{pmatrix} \frac{1}{\sqrt{2}} - \lambda & \frac{1}{\sqrt{2}} \\ \frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}} - \lambda \end{pmatrix} &= \left(\frac{1}{\sqrt{2}} - \lambda\right)\left(-\frac{1}{\sqrt{2}} - \lambda\right) - \left(\frac{1}{\sqrt{2}}\right)^2 = 0 \\
\left(\lambda^2 - \frac{1}{2}\right) - \frac{1}{2} &= 0 \\
\lambda^2 - 1 &= 0 \;\Rightarrow\; \boxed{\lambda_1 = +1, \quad \lambda_2 = -1}
\end{aligned}
$$

---

## 5. Tuliskan Pauli $Z$ dalam bentuk outer product (*spectral decomposition*)

Matriks $Z = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}$ memiliki pasangan eigenvalue dan eigenvector:
* $\lambda_1 = +1 \;\leftrightarrow\; |v_1\rangle = |0\rangle = \begin{pmatrix} 1 \\ 0 \end{pmatrix}$
* $\lambda_2 = -1 \;\leftrightarrow\; |v_2\rangle = |1\rangle = \begin{pmatrix} 0 \\ 1 \end{pmatrix}$

Substitusikan ke dalam rumus *spectral decomposition* $Z = \sum_k \lambda_k |v_k\rangle\langle v_k|$:

$$
\begin{aligned}
Z &= (+1)|0\rangle\langle 0| + (-1)|1\rangle\langle 1| \\
&= \boxed{|0\rangle\langle 0| - |1\rangle\langle 1|}
\end{aligned}
$$

**Verifikasi matriks:**

$$
|0\rangle\langle 0| - |1\rangle\langle 1| = \begin{pmatrix} 1 \\ 0 \end{pmatrix}\begin{pmatrix} 1 & 0 \end{pmatrix} - \begin{pmatrix} 0 \\ 1 \end{pmatrix}\begin{pmatrix} 0 & 1 \end{pmatrix} = \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix} - \begin{pmatrix} 0 & 0 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix} = Z
$$
