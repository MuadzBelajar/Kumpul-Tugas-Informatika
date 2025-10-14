<h1>CATATAN</h1>

<h4>Hello word</h4>
<p>Konsep paling dasar pada pemrograman: program yang menampilkan teks “Hello World” ke layar. Tujuan utamanya adalah memverifikasi lingkungan kerja (browser/editor) dan memahami cara menjalankan kode. Di JavaScript ada beberapa cara menampilkan: console.log() (untuk developer console), alert() (popup), atau output ke dokumen dengan document.write()/DOM.</p> 

<h4>OPERATOR ARITMATIKA</h4>
<p>Operator untuk operasi matematika dasar: + (tambah), - (kurang), * (kali), / (bagi), % (modulus/sisa bagi), ** (pangkat). Digunakan pada tipe number. Perlu hati-hati dengan pembagian nol (menghasilkan Infinity atau -Infinity) dan floating point (ketidakakuratan representasi desimal).</p>

<h4>OPERATOR AUGMENTED ASSIGNMENT</h4>
<P>Singkatan untuk menulis operasi lalu menugaskannya kembali ke variabel: +=, -=, *=, /=, %=. Memperpendek x = x + y menjadi x += y. Berguna untuk memperjelas niat dan mengurangi panjang kode. Perhatikan prioritas operator: x += y * z berarti x = x + (y * z).</P>

<h4>OPERATOR LOGIKA</h4>
<P>Digunakan untuk menggabungkan ekspresi boolean: && (AND), || (OR), ! (NOT). Dalam JavaScript operator ini juga melakukan short-circuit evaluation dan mengembalikan nilai operand (bukan selalu boolean) — mis. a || b mengembalikan a jika truthy, kalau tidak b. Penting untuk memahami truthy/falsy (0, "", null, undefined, NaN, false adalah falsy).</P>

<h4>OPERATOR UNARY</h4>
<P>Operator yang hanya bekerja pada satu operand. Contoh umum: typeof (mengembalikan tipe), ! (negasi), unary + (konversi ke number), unary - (mengubah tanda), ++/-- (increment/decrement). ++/-- memiliki bentuk prefix (++x) dan postfix (x++) yang berbeda hasil/kapan efeknya terjadi.</P>

<h4>OPERATOR PEMBANDING</h4>
<P>Digunakan untuk membandingkan nilai: == (loose equality), === (strict equality), !=, !==, >, <, >=, <=. Di JavaScript disarankan pakai ===/!== untuk menghindari coercion (konversi tipe otomatis) yang bisa menyebabkan hasil tak terduga.</P>

<h4>TIPE DATA ARRAY</h4>
<P>Array adalah struktur data urutan (indexed) yang menyimpan elemen. Di JS array bersifat dinamis (bisa bertambah) dan dapat menyimpan berbagai tipe dalam satu array. Akses via indeks mulai dari 0. Banyak metode penting: push, pop, shift, unshift, slice, splice, map, filter, reduce.</P>

<h4>TIPE DATA BOOLEAN</h4>
<P>Hanya dua nilai: true atau false. Sering dihasilkan dari operator pembanding atau logika. Digunakan untuk pengambilan keputusan (percabangan, loops).</P>

<h4>TIPE DATA NUMBER</h4>
<P>Menampung angka (integer dan floating point) dalam satu tipe. Semua angka di JS menggunakan format 64-bit floating point (IEEE 754). Perlu hati-hati terhadap presisi desimal; gunakan toFixed, Math.round, atau library untuk presisi tinggi apabila diperlukan. Ada juga BigInt untuk bilangan sangat besar.</P>

<h4>TIPE DATA OBJECT</h4>
<P>Struktur yang menyimpan pasangan kunci-nilai (key-value). Kunci biasanya string (atau Symbol), nilai bisa apa saja (termasuk function → method). Object basis untuk banyak struktur di JS (mis. array, fungsi juga objek). Akses via dot notation atau bracket notation.</P>

<h4>TIPE STRING</h4>
<P>Teks yang diapit tanda kutip ('...', "...", atau template literal `...`). Template literal mendukung interpolasi ${expr} dan multiline. String immutable (operasi menghasilkan string baru).</P>

<h4>VARIABLE</h4>
<P>Nama penyimpanan nilai: var, let, const. var lama, memiliki function-scope dan hoisting; let dan const diperkenalkan ES6, bersifat block-scope. Gunakan const untuk nilai yang tidak akan di-assign ulang; let bila perlu diubah. Nama variabel harus mengikuti aturan identifier.</P>

<h4>IF EXPRESSION</h4>
<P>Struktur percabangan untuk mengeksekusi blok kode berdasarkan kondisi boolean. if pertama dievaluasi; jika false, JavaScript memeriksa else if berikutnya; jika semua false, blok else dijalankan (jika ada). Bisa menangani kondisi kompleks menggunakan operator logika/perbandingan.</P>

<h4>SWICTH</h4>
<P>Struktur percabangan yang membandingkan satu ekspresi dengan beberapa case nilai. Cocok bila kita memeriksa satu variabel terhadap banyak nilai yang sudah diketahui. Gunakan break untuk menghentikan “fall-through” antar case (kecuali memang ingin bergabung beberapa case).</P>

<h4>PERBEDAAN ANTARA IF DAN SWITCH</h4>
 <p>Struktur if digunakan ketika kita ingin memeriksa kondisi logika yang kompleks, seperti perbandingan nilai, rentang angka, atau kondisi gabungan yang melibatkan operator logika seperti &&, ||, >, dan <. Kelebihan dari penggunaan if adalah fleksibilitasnya yang tinggi karena bisa digunakan untuk berbagai jenis kondisi. Namun, jika jumlah kondisinya terlalu banyak, struktur if-else bisa menjadi panjang dan sulit dibaca.</p>
<br>
<p>struktur switch digunakan untuk membandingkan satu nilai dengan beberapa kemungkinan tetap. Biasanya, switch lebih cocok digunakan ketika kita memiliki satu variabel yang memiliki beberapa pilihan nilai yang pasti, seperti huruf nilai ujian (“A”, “B”, “C”, dan seterusnya), status pengguna, atau menu pilihan. Kelebihan switch adalah tampilannya yang lebih rapi dan mudah dibaca dibandingkan dengan if ketika digunakan untuk banyak kondisi. Namun, switch memiliki keterbatasan karena tidak bisa menangani kondisi logika yang kompleks — ia hanya membandingkan nilai secara langsung.</p>
