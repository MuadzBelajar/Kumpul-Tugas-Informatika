<h1>CATATAN MATERI</h1>

<h4>1. HELLO WORLD</h4>
<p>Konsep paling dasar pada pemrograman: program yang menampilkan teks “Hello World” ke layar. Tujuan utamanya adalah memverifikasi lingkungan kerja (browser/editor) dan memahami cara menjalankan kode. Di JavaScript ada beberapa cara menampilkan: console.log() (untuk developer console), alert() (popup), atau output ke dokumen dengan document.write()/DOM.</p> 
<pre><code>
&lt;script&gt;
console.log("Hello World!");
alert("Hello World!");
document.write("Hello World!");
&lt;/script&gt;
</code></pre>

<h4>2. OPERATOR ARITMATIKA</h4>
<p>Operator untuk operasi matematika dasar: + (tambah), - (kurang), * (kali), / (bagi), % (modulus/sisa bagi), ** (pangkat). Digunakan pada tipe number. Perlu hati-hati dengan pembagian nol (menghasilkan Infinity atau -Infinity) dan floating point (ketidakakuratan representasi desimal).</p>
<pre><code>
&lt;script&gt;
let a = 10, b = 3;
document.write(a + b + "&lt;br&gt;"); // 13
document.write(a - b + "&lt;br&gt;"); // 7
document.write(a * b + "&lt;br&gt;"); // 30
document.write(a / b + "&lt;br&gt;"); // 3.3333
document.write(a % b + "&lt;br&gt;"); // 1
document.write(a ** b);           // 1000
&lt;/script&gt;
</code></pre>

<h4>3. OPERATOR AUGMENTED ASSIGNMENT</h4>
<p>Singkatan untuk menulis operasi lalu menugaskannya kembali ke variabel: +=, -=, *=, /=, %=. Memperpendek x = x + y menjadi x += y.</p>
<pre><code>
&lt;script&gt;
let x = 5;
x += 3; // 8
x *= 2; // 16
document.write("Nilai x sekarang adalah " + x);
&lt;/script&gt;
</code></pre>

<h4>4. OPERATOR LOGIKA</h4>
<p>Digunakan untuk menggabungkan ekspresi boolean: && (AND), || (OR), ! (NOT).</p>
<pre><code>
&lt;script&gt;
let a = true, b = false;
document.write(a && b + "&lt;br&gt;"); // false
document.write(a || b + "&lt;br&gt;"); // true
document.write(!a); // false
&lt;/script&gt;
</code></pre>

<h4>5. OPERATOR UNARY</h4>
<p>Operator yang hanya bekerja pada satu operand seperti typeof, !, ++, dan --.</p>
<pre><code>
&lt;script&gt;
let n = 5;
document.write(typeof n + "&lt;br&gt;"); // number
document.write(++n + "&lt;br&gt;"); // 6
document.write(-n); // -6
&lt;/script&gt;
</code></pre>

<h4>6. OPERATOR PEMBANDING</h4>
<p>Digunakan untuk membandingkan nilai: ==, ===, !=, !==, >, <, >=, <=.</p>
<pre><code>
&lt;script&gt;
let angka = 10;
document.write(angka == "10" + "&lt;br&gt;"); // true
document.write(angka === "10" + "&lt;br&gt;"); // false
document.write(angka > 5); // true
&lt;/script&gt;
</code></pre>

<h4>7. TIPE DATA ARRAY</h4>
<p>Array menyimpan kumpulan data dengan urutan indeks.</p>
<pre><code>
&lt;script&gt;
let buah = ["Apel", "Jeruk", "Mangga"];
buah.push("Pisang");
document.write(buah.join(", "));
&lt;/script&gt;
</code></pre>

<h4>8. TIPE DATA BOOLEAN</h4>
<p>Tipe data boolean hanya memiliki dua nilai: true dan false.</p>
<pre><code>
&lt;script&gt;
let nilai = 70;
let lulus = nilai >= 60;
document.write("Apakah lulus? " + lulus);
&lt;/script&gt;
</code></pre>

<h4>9. TIPE DATA NUMBER</h4>
<p>Menampung angka, baik integer maupun desimal.</p>
<pre><code>
&lt;script&gt;
let a = 0.1 + 0.2;
document.write(a + "&lt;br&gt;"); // 0.30000000000000004
document.write(a.toFixed(2)); // 0.30
&lt;/script&gt;
</code></pre>

<h4>10. TIPE DATA OBJECT</h4>
<p>Struktur yang menyimpan pasangan key dan value.</p>
<pre><code>
&lt;script&gt;
let siswa = {
  nama: "Aldi",
  umur: 17,
  jurusan: "RPL"
};
document.write(siswa.nama + " berumur " + siswa.umur);
&lt;/script&gt;
</code></pre>

<h4>11. TIPE DATA STRING</h4>
<p>Teks yang diapit tanda kutip, bisa menggunakan template literal.</p>
<pre><code>
&lt;script&gt;
let nama = "Muadz";
document.write("Halo " + nama + "&lt;br&gt;");
document.write(`Selamat datang, ${nama}!`);
&lt;/script&gt;
</code></pre>

<h4>12. VARIABLE</h4>
<p>Variabel digunakan untuk menyimpan data sementara. Tiga jenis deklarasi: var, let, const.</p>
<pre><code>
&lt;script&gt;
var a = 10;
let b = 20;
const c = 30;
document.write(a + b + c);
&lt;/script&gt;
</code></pre>

<h4>13. IF EXPRESSION</h4>
<p>Struktur percabangan untuk menjalankan perintah berdasarkan kondisi tertentu.</p>
<pre><code>
&lt;script&gt;
let nilai = 85;
if (nilai >= 90) {
  document.write("Nilai A");
} else if (nilai >= 75) {
  document.write("Nilai B");
} else {
  document.write("Nilai C");
}
&lt;/script&gt;
</code></pre>

<h4>14. SWITCH</h4>
<p>Struktur percabangan untuk membandingkan satu nilai dengan beberapa kemungkinan.</p>
<pre><code>
&lt;script&gt;
let grade = "B";
switch (grade) {
  case "A":
    document.write("Sangat Baik");
    break;
  case "B":
  case "C":
    document.write("Baik");
    break;
  case "D":
    document.write("Kurang");
    break;
  default:
    document.write("Tidak Valid");
}
&lt;/script&gt;
</code></pre>

<h4>15. PERBEDAAN ANTARA IF DAN SWITCH</h4>
<p>Struktur <b>if</b> digunakan ketika kita ingin memeriksa kondisi logika yang kompleks, seperti perbandingan nilai, rentang angka, atau kondisi gabungan yang melibatkan operator logika seperti &&, ||, >, dan <. Kelebihan dari penggunaan if adalah fleksibilitasnya yang tinggi karena bisa digunakan untuk berbagai jenis kondisi. Namun, jika jumlah kondisinya terlalu banyak, struktur if-else bisa menjadi panjang dan sulit dibaca.</p>

<p>Struktur <b>switch</b> digunakan untuk membandingkan satu nilai dengan beberapa kemungkinan tetap. Biasanya, switch lebih cocok digunakan ketika kita memiliki satu variabel yang memiliki beberapa pilihan nilai yang pasti, seperti huruf nilai ujian (“A”, “B”, “C”, dan seterusnya), status pengguna, atau menu pilihan. Kelebihan switch adalah tampilannya yang lebih rapi dan mudah dibaca dibandingkan dengan if ketika digunakan untuk banyak kondisi. Namun, switch memiliki keterbatasan karena tidak bisa menangani kondisi logika yang kompleks — ia hanya membandingkan nilai secara langsung.</p>

<pre><code>
&lt;script&gt;
// Contoh penggunaan IF
let usia = 20;
if (usia >= 18) {
  document.write("Dewasa");
} else {
  document.write("Anak-anak");
}

// Contoh penggunaan SWITCH
let hari = "Senin";
switch (hari) {
  case "Senin":
    document.write("&lt;br&gt;Hari kerja dimulai!");
    break;
  case "Sabtu":
  case "Minggu":
    document.write("&lt;br&gt;Akhir pekan!");
    break;
  default:
    document.write("&lt;br&gt;Hari biasa.");
}
&lt;/script&gt;
</code></pre>

<h4>16. OPERATOR TYPE OF</h4>
<p>Operator <b>typeof</b> digunakan untuk memeriksa tipe data dari sebuah nilai atau variabel. Hasilnya berupa string seperti "string", "number", "boolean", "object", dan sebagainya. Operator ini sangat berguna saat kita ingin memastikan tipe data sebelum melakukan operasi tertentu.</p>
<pre><code>
&lt;script&gt;
let nama = "Muadz";
let umur = 17;
let aktif = true;

document.write(typeof nama + "&lt;br&gt;");  // string
document.write(typeof umur + "&lt;br&gt;");  // number
document.write(typeof aktif);             // boolean
&lt;/script&gt;
</code></pre>

<h4>17. OPERATOR IN</h4>
<p>Operator <b>in</b> digunakan untuk memeriksa apakah sebuah properti ada di dalam objek atau sebuah indeks ada di dalam array. Jika ditemukan, hasilnya <b>true</b>; jika tidak, <b>false</b>. Operator ini membantu untuk mencegah error ketika mencoba mengakses properti yang belum tentu ada.</p>
<pre><code>
&lt;script&gt;
const person = { name: "Rafi", age: 16 };

document.write("name" in person + "&lt;br&gt;");   // true
document.write("address" in person + "&lt;br&gt;"); // false

const fruits = ["apel", "mangga", "pisang"];
document.write(1 in fruits + "&lt;br&gt;");  // true
document.write(5 in fruits);             // false
&lt;/script&gt;
</code></pre>

<h4>18. OPERATOR TERNARY</h4>
<p>Operator <b>ternary</b> adalah bentuk singkat dari struktur <b>if-else</b>. Operator ini digunakan untuk membuat keputusan sederhana dalam satu baris kode. Formatnya adalah: <code>kondisi ? hasil_jika_benar : hasil_jika_salah</code>.</p>
<pre><code>
&lt;script&gt;
let nilai = 80;
let hasil = nilai >= 75 ? "Lulus" : "Tidak Lulus";
document.write(hasil); // Lulus
&lt;/script&gt;
</code></pre>

<h4>19. NULLISH COALESCING</h4>
<p> Operator <b>Nullish Coalescing (??)</b> digunakan untuk memberikan nilai default ketika suatu variabel bernilai <b>null</b> atau <b>undefined</b>.  
Berbeda dengan operator logika OR (<b>||</b>), operator ini hanya akan menggantikan nilai <b>null</b> dan <b>undefined</b>, bukan nilai falsy lainnya seperti 0 atau string kosong.  
Hal ini membuatnya lebih aman ketika kita ingin memberikan nilai cadangan tanpa mengganggu nilai yang sah seperti 0 atau "".
</p>

<pre><code>
&lt;script&gt;
let parameter; // Belum diberi nilai, jadi undefined

// Cara manual tanpa ?? 
let data = parameter;
if (data === undefined || data === null) {
  data = "Nilai Default";
}

document.writeln(`&lt;p&gt;${data}&lt;/p&gt;`); // Hasil: Nilai Default
</code></pre>

<p>
Dengan menggunakan <b>??</b>, kita dapat menulis kode lebih singkat dan mudah dibaca.
</p>


<h4>20. OPTIONAL CHAINING</h4>
<p><b>Optional Chaining</b> digunakan untuk mengakses properti objek secara aman tanpa menimbulkan error ketika salah satu bagian tidak ada (undefined atau null). Jika jalur yang diakses tidak ada, hasilnya <b>undefined</b> tanpa menghentikan program.</p>
<pre><code>
&lt;script&gt;
const person = {
  address: {
    country: "Indonesia"
  }
};

let country = person?.address?.country;
document.write("&lt;p&gt;" + country + "&lt;/p&gt;"); // Indonesia

// Jika address tidak ada, tidak error, hanya undefined
const user = {};
document.write("&lt;p&gt;" + user?.address?.city + "&lt;/p&gt;"); // undefined
&lt;/script&gt;
</code></pre>
