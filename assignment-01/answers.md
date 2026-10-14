## Task 1 — Conceptual Questions

Jawab dengan kata-kata Anda sendiri (3–6 kalimat per soal).
1. Apa yang dimaksud dengan *ultraviolet catastrophe*, dan bagaimana hipotesis Planck menyelesaikannya?

Jawaban: Ultraviolet catastrophe itu pada dasarnya adalah kegagalan fisika klasik (rumus Rayleigh–Jeans) waktu mencoba menjelaskan radiasi benda hitam. Menurut perhitungan klasik, energi radiasi yang dipancarkan benda hitam bakal terus naik menuju tak hingga ($\infty$) saat panjang gelombangnya makin pendek (ke arah daerah ultraviolet), yang jelas-jelas nggak masuk akal karena di eksperimen kurvanya justru memuncak lalu turun ke nol. Nah, Max Planck akhirnya menyelesaikan masalah ini lewat hipotesisnya bahwa energi osilator itu nggak kontinu, melainkan terkuantisasi dalam "paket-paket" diskrit sebesar $E = nh\nu$. Karena butuh energi yang besar banget untuk memancarkan foton berfrekuensi tinggi (panjang gelombang pendek), peluang osilator untuk teraktivasi di area UV jadi sangat kecil, sehingga kurva radiasinya otomatis turun kembali ke nol sesuai hasil observasi.

2. Dalam photoelectric effect, mengapa menaikkan **intensitas** cahaya merah tidak membuat elektron terlepas dari logam, sedangkan cahaya ultraviolet redup dapat melakukannya?
   
Jawaban: Di fenomena efek fotolistrik, Einstein menjelaskan kalau cahaya itu terdiri dari partikel-partikel paket energi yang disebut foton, di mana energi tiap satu fotonnya cuma bergantung pada frekuensinya ($E = h\nu$), bukan intensitasnya. Cahaya merah punya frekuensi yang rendah (di bawah frekuensi ambang logam, $\nu_0 = \phi / h$), jadi energi satu fotonnya nggak cukup kuat buat melawan work function ($\phi$) untuk menendang elektron keluar. Mau intensitas cahaya merahnya dinaikkan seterang apa pun, itu cuma nambahin jumlah fotonnya aja, tapi energi per fotonnya tetap kurang. Sebaliknya, cahaya ultraviolet punya frekuensi yang tinggi banget sehingga energi per fotonnya sudah melewati batas $\phi$; makanya, meskipun cahayanya redup (jumlah fotonnya sedikit), tiap satu foton UV yang nabrak logam tetap sanggup melepaskan satu elektron.   

3. Jelaskan apa yang terjadi pada eksperimen double-slit jika elektron ditembakkan satu per satu, dan apa yang berubah jika kita memasang detektor di salah satu celah.

Jawaban: Kalau kita menembakkan elektron satu per satu melewati dua celah, awalnya setiap elektron bakal mendarat di layar sebagai satu titik terpisah layaknya partikel biasa. Tapi yang unik, kalau kita biarkan ribuan elektron ditembakkan terus-menerus, kumpulan titik-titik tadi perlahan bakal membentuk pola gelap-terang (pola interferensi) yang membuktikan kalau tiap elektron sebenarnya punya sifat gelombang dan berada dalam keadaan superposisi (melewati kedua celah sekaligus) sebelum menabrak layar. Namun, begitu kita pasang detektor di salah satu celah buat "mengintip" elektron lewat jalur yang mana, tindakan pengukuran ini langsung meruntuhkan superposisinya (wavefunction collapse). Akibatnya, sifat gelombangnya hilang dan pola interferensi di layar berubah jadi dua garis kumpul biasa layaknya partikel klasik.

4. Wavefunction $\psi$ bernilai kompleks dan tidak dapat diukur langsung. Lalu besaran apa yang memiliki makna fisis, dan apa artinya?

Jawaban: Memang benar kalau wavefunction $\psi(x,t)$ itu bernilai kompleks dan nggak bisa kita ukur secara langsung di laboratorium. Besaran yang punya makna fisis nyata adalah kuadrat nilai mutlaknya, yaitu $\vert{}\psi(x,t)\vert{}^2$ (atau peluang $P(x)\,dx = \vert{}\psi(x,t)\vert{}^2\,dx$). Sesuai dengan Born rule, nilai $\vert{}\psi(x,t)\vert{}^2$ ini mewakili rapat probabilitas untuk menemukan partikel di posisi antara $x$ sampai $x + dx$ ketika kita melakukan pengukuran. Jadi, karena partikelnya pasti ada di suatu tempat di ruang tersebut, total peluang di seluruh ruang kalau diintegralkan harus bernilai 1 (kondisi ternormalisasi). 

5. Seorang teman berkata: *"Uncertainty principle muncul karena alat ukur kita belum cukup canggih."* Apakah pernyataan ini benar? Jelaskan.

Jawaban: Pernyataan temanku itu salah konsep. Heisenberg Uncertainty Principle ($\Delta x \, \Delta p \geq \hbar/2$) muncul bukan karena alat ukur kita yang kurang canggih atau error dari pengamat, melainkan memang sifat bawaan paling mendasar dari alam semesta. Ketidakpastian ini lahir langsung dari sifat dualisme gelombang-partikel materi itu sendiri. Secara fisis, kalau kita mau melokalisasi posisi gelombang partikel secara super akurat ($\Delta x$ sangat sempit), paket gelombangnya harus tersusun dari superposisi banyak panjang gelombang, yang otomatis bikin momentumnya ($\Delta p$) jadi sangat menyebar dan tidak pasti—begitu juga sebaliknya

7. Mengapa kita tidak melihat efek interferensi saat melempar bola melalui dua pintu?

Jawaban: Menurut rumus de Broglie, setiap benda yang bergerak memang punya panjang gelombang sebesar $\lambda = h/p = h/(mv)$. Masalahnya, konstanta Planck ($h = 6.626 \times 10^{-34}\ \text{J}\cdot\text{s}$) itu nilainya luar biasa kecil, sedangkan bola punya massa ($m$) yang sangat besar kalau dibandingkan dengan partikel subatomik. Kalau dihitung, panjang gelombang de Broglie dari bola yang kita lempar itu ukurannya sekitar $\sim 10^{-34}\ \text{m}$, jauh lebih kecil triliunan kali lipat daripada lebar pintu. Karena syarat terjadinya difraksi/interferensi gelombang adalah ukuran celah harus sebanding dengan panjang gelombangnya, maka sifat gelombang bola sama sekali nggak kelihatan di dunia sehari-hari.

## Task 2 — Perhitungan
Daftar Konstanta yang Digunakan:   
$h = 6.626 \times 10^{-34}\ \text{J}\cdot\text{s}$   $\hbar = 1.055 \times 10^{-34}\ \text{J}\cdot\text{s}$   $c = 3.00 \times 10^{8}\ \text{m/s}$   $e = 1.602 \times 10^{-19}\ \text{C}$ (di mana $1\ \text{eV} = 1.602 \times 10^{-19}\ \text{J}$)   $m_e = 9.109 \times 10^{-31}\ \text{kg}$   $m_n = 1.675 \times 10^{-27}\ \text{kg}$

1. **Energi foton.** Sebuah laser pointer merah memancarkan cahaya $\lambda = 650$ nm dengan daya 5 mW.
   - (a) Berapa energi satu foton dalam joule dan eV?
   - (b) Berapa jumlah foton yang dipancarkan per detik?

Jawaban:

Diketahui:
- Panjang gelombang: $\lambda = 650\ \text{nm} = 6.50 \times 10^{-7}\ \text{m}$   
- Daya laser: $P = 5\ \text{mW} = 5 \times 10^{-3}\ \text{W} = 5 \times 10^{-3}\ \text{J/s}$

(a) Energi satu foton dalam Joule dan eV:
- $$E = \frac{hc}{\lambda}$$
- $E = \frac{(6.626 \times 10^{-34}\ \text{J}\cdot\text{s})(3.00 \times 10^{8}\ \text{m/s})}{6.50 \times 10^{-7}\ \text{m}}$
- $E = 3.058 \times 10^{-19}\ \text{J}$
- $E\ (\text{eV}) = \frac{3.058 \times 10^{-19}\ \text{J}}{1.602 \times 10^{-19}\ \text{J/eV}} = \mathbf{1.909\ \text{eV}}$

(b) Jumlah foton yang dipancarkan per detik ($N$):
- $N = \frac{P}{E}$
- $N = \frac{5 \times 10^{-3}\ \text{J/s}}{3.058 \times 10^{-19}\ \text{J/foton}} = \mathbf{1.635 \times 10^{16}\ \text{foton/detik}}$

2. **Photoelectric effect.** Natrium memiliki work function $\phi = 2.28$ eV.
   - (a) Berapa panjang gelombang ambang (threshold) untuk natrium?
   - (b) Jika disinari cahaya $\lambda = 400$ nm, berapa energi kinetik maksimum elektron yang terlepas (dalam eV)?
   - (c) Berapa stopping potential yang diperlukan untuk menghentikan elektron tersebut?
   - (d) Apakah cahaya $\lambda = 600$ nm dapat melepaskan elektron? Jelaskan.

Jawaban:

Diketahui:
- Work function natrium: $\phi = 2.28\ \text{eV}$

(a) Panjang gelombang ambang ($\lambda_0$):
- $\phi = 2.28\ \text{eV} \times 1.602 \times 10^{-19}\ \text{J/eV} = 3.6526 \times 10^{-19}\ \text{J}$
- $\lambda_0 = \frac{hc}{\phi}$
- $\lambda_0 = \frac{(6.626 \times 10^{-34}\ \text{J}\cdot\text{s})(3.00 \times 10^{8}\ \text{m/s})}{3.6526 \times 10^{-19}\ \text{J}}$
- $\lambda_0 = 5.442 \times 10^{-7}\ \text{m} = \mathbf{544.2\ \text{nm}}$

(b) Energi kinetik maksimum elektron ($K_{\max}$) saat disinari $\lambda = 400\ \text{nm}$:
- $E = \frac{hc}{\lambda \cdot e} = \frac{1.9878 \times 10^{-25}\ \text{J}\cdot\text{m}}{(4.00 \times 10^{-7}\ \text{m})(1.602 \times 10^{-19}\ \text{J/eV})} = 3.102\ \text{eV}$
- $K_{\max} = E - \phi$
- $K_{\max} = 3.102\ \text{eV} - 2.28\ \text{eV} = \mathbf{0.822\ \text{eV}}$

(c) Stopping potential ($V_{\text{stop}}$):
- $V_{\text{stop}} = \frac{K_{\max}}{e}$
- $V_{\text{stop}} = \frac{0.822\ \text{eV}}{e} = \mathbf{0.822\ \text{V}}$

(d) Apakah cahaya $\lambda = 600\ \text{nm}$ bisa melepaskan elektron?
- Tidak bisa. Foton $600\ \text{nm}$ hanya memiliki energi $E \approx 1240 / 600 = 2.067\ \text{eV}$, yang mana lebih kecil dari work function natrium sebesar $\phi = 2.28\ \text{eV}$. Selain itu, $\lambda = 600\ \text{nm}$ lebih besar dari panjang gelombang ambang natrium ($\lambda_0 = 544.2\ \text{nm}$), yang berarti frekuensinya lebih rendah dari frekuensi ambang.

3. **de Broglie wavelength.**
   - (a) Pada eksperimen Davisson–Germer (1927), elektron dipercepat dengan beda potensial 54 V. Hitung panjang gelombang de Broglie-nya.
   - (b) Hitung panjang gelombang de Broglie neutron termal yang bergerak dengan kecepatan 2200 m/s.
   - (c) Bandingkan hasil (a) dan (b) dengan jarak antar-atom pada kristal ($\sim 0.1$–$0.3$ nm). Apa implikasinya?
  
Jawaban:

(a) Elektron pada eksperimen Davisson–Germer ($\Delta V = 54\ \text{V}$):
- $K = 54\ \text{eV} \times 1.602 \times 10^{-19}\ \text{J/eV} = 8.6508 \times 10^{-18}\ \text{J}$
- $p = \sqrt{2 m_e K} = \sqrt{2 (9.109 \times 10^{-31}\ \text{kg})(8.6508 \times 10^{-18}\ \text{J})} = 3.970 \times 10^{-24}\ \text{kg}\cdot\text{m/s}$
- $\lambda_e = \frac{h}{p} = \frac{6.626 \times 10^{-34}\ \text{J}\cdot\text{s}}{3.970 \times 10^{-24}\ \text{kg}\cdot\text{m/s}} = 1.669 \times 10^{-10}\ \text{m} = \mathbf{0.167\ \text{nm}}$

(b) Neutron termal ($v = 2200\ \text{m/s}$):
- $p = m_n v = (1.675 \times 10^{-27}\ \text{kg})(2200\ \text{m/s}) = 3.685 \times 10^{-24}\ \text{kg}\cdot\text{m/s}$
- $\lambda_n = \frac{h}{p} = \frac{6.626 \times 10^{-34}\ \text{J}\cdot\text{s}}{3.685 \times 10^{-24}\ \text{kg}\cdot\text{m/s}} = 1.798 \times 10^{-10}\ \text{m} = \mathbf{0.180\ \text{nm}}$

(c) Perbandingan dengan jarak antar-atom kristal ($\sim 0.1\text{–}0.3\ \text{nm}$) & Implikasinya:
- Hasil (a) dan (b) menunjukkan panjang gelombang yang seukuran dengan jarak antar-atom pada kisi kristal. Implikasinya, susunan atom di dalam kristal dapat berfungsi sebagai kisi difraksi. Hal ini memungkinkan berkas elektron dan neutron mengalami interferensi konstruktif atau destruktif, yang dapat dimanfaatkan untuk memetakan struktur atom material.

4. **Uncertainty principle.**
   - (a) Sebuah elektron dibatasi dalam daerah selebar 1 nm. Hitung ketidakpastian minimum momentum dan kecepatannya.
   - (b) Lakukan perhitungan yang sama untuk sebuah debu bermassa $10^{-9}$ kg yang posisinya diketahui dengan ketelitian 1 µm. Bandingkan dan beri komentar.
  
Jawaban:

(a) Elektron di daerah selebar $\Delta x = 1\ \text{nm} = 1.0 \times 10^{-9}\ \text{m}$:
- $\Delta p_{\min} = \frac{\hbar}{2\Delta x} = \frac{1.055 \times 10^{-34}\ \text{J}\cdot\text{s}}{2 (1.0 \times 10^{-9}\ \text{m})} = \mathbf{5.275 \times 10^{-26}\ \text{kg}\cdot\text{m/s}}$
- $\Delta v_{\min} = \frac{\Delta p_{\min}}{m_e} = \frac{5.275 \times 10^{-26}\ \text{kg}\cdot\text{m/s}}{9.109 \times 10^{-31}\ \text{kg}} = \mathbf{5.791 \times 10^{4}\ \text{m/s}}\ (\approx 57.9\ \text{km/s})$

(b) Partikel debu ($m = 10^{-9}\ \text{kg}$) dengan ketelitian $\Delta x = 1\ \mu\text{m} = 1.0 \times 10^{-6}\ \text{m}$:
- $\Delta p_{\min} = \frac{\hbar}{2\Delta x} = \frac{1.055 \times 10^{-34}\ \text{J}\cdot\text{s}}{2 (1.0 \times 10^{-6}\ \text{m})} = \mathbf{5.275 \times 10^{-29}\ \text{kg}\cdot\text{m/s}}$
- $\Delta v_{\min} = \frac{\Delta p_{\min}}{m} = \frac{5.275 \times 10^{-29}\ \text{kg}\cdot\text{m/s}}{10^{-9}\ \text{kg}} = \mathbf{5.275 \times 10^{-20}\ \text{m/s}}$

Perbandingan dan Komentar:
- Terdapat perbedaan yang sangat ekstrem. Elektron yang dibatasi pada skala nanometer memiliki ketidakpastian kecepatan yang sangat besar, mencapai hampir $58\ \text{km/s}$. Sebaliknya, partikel debu memiliki ketidakpastian kecepatan yang sangat kecil ($\sim 10^{-20}\ \text{m/s}$), yang secara praktis bernilai nol. Hal ini menunjukkan bahwa efek ketidakpastian kuantum sangat mendominasi partikel di skala atomik, namun tidak teramati pada benda berskala makroskopis.
