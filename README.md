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

<h4>21. FALSY DAN TRUTHY</h4> <p><b>Falsy</b> dan <b>Truthy</b> adalah konsep dalam JavaScript yang menentukan apakah suatu nilai dianggap <code>true</code> atau <code>false</code> ketika digunakan dalam kondisi logika seperti <code>if</code>. Nilai yang dianggap <b>false</b> disebut <b>Falsy</b>, sedangkan nilai lainnya disebut <b>Truthy</b>.</p> <p>Pada contoh di bawah, variabel <code>data</code> belum memiliki nilai (<code>undefined</code>), sehingga dianggap <b>Falsy</b> dan menghasilkan tulisan <b>"FALSE"</b> di layar.</p> <pre><code> &lt;script&gt; let data; if (data) { document.writeln("TRUE"); } else { document.writeln("FALSE"); } &lt;/script&gt; </code></pre> <p>Nilai yang termasuk <b>Falsy</b> antara lain: <code>false</code>, <code>0</code>, <code>""</code> (string kosong), <code>null</code>, <code>undefined</code>, dan <code>NaN</code>. Selain nilai-nilai tersebut dianggap <b>Truthy</b>.</p>
<h4>22. FALSY DAN TRUTHY DI NON BOOLEAN</h4>
<p>Operator logika seperti <b>|| (OR)</b> dan <b>&amp;&amp; (AND)</b> tidak hanya bekerja pada nilai boolean.  
Mereka juga bisa digunakan untuk mengembalikan nilai <b>non-boolean</b> berdasarkan nilai <b>Truthy</b> dan <b>Falsy</b>.</p>

<pre><code>
&lt;script&gt;
console.info("Hello" || "");
console.info("" || []);
console.info("0" || "NOL");
console.info(0 || "NOL");
console.info(null || "NULL");
console.info(undefined || "UNDEFINED");
console.info(0 || false);

const person = {
  firstName: "",
  lastName: "Khannedy",
};

const name = person.firstName || person.lastName;
console.info(name);

console.info("HELLO" &amp;&amp; "");
console.info("" &amp;&amp; []);
console.info("0" &amp;&amp; "NOL");
&lt;/script&gt;
</code></pre>

<p><b>Penjelasan:</b></p>
<ul>
  <li><b>Operator OR (||)</b> akan mengembalikan nilai pertama yang <b>Truthy</b>.</li>
  <li><b>Operator AND (&amp;&amp;)</b> akan mengembalikan nilai pertama yang <b>Falsy</b>, atau nilai terakhir jika semua <b>Truthy</b>.</li>
</ul>
<pre><code>
Hasil di console:
Hello
[]
0
NOL
NULL
UNDEFINED
false
Khannedy
""
""
NOL
</code></pre>

<h4>23. FOR LOOP</h4>
<p>
<b>For Loop</b> digunakan untuk melakukan perulangan dengan jumlah yang sudah diketahui. 
Struktur dasarnya terdiri dari tiga bagian: inisialisasi, kondisi, dan increment/decrement.
Perulangan akan berhenti jika kondisi tidak lagi terpenuhi.
</p>
<pre><code>
 <script>
    // Standart Penulisan
    let counter = 1;
    for (; counter <= 10; ) {
      document.writeln(`<p>Perulangan ke ${counter}</p>`);
      counter++;
    }

    // Penulisan yang efisien
    for (let counter = 1; counter <= 10; counter++) {
      document.writeln(`<p>Perulangan ke ${counter}</p>`);
    }
  </script>
</code></pre>

<h4>24. WHILE LOOP</h4>
<p>
<b>While Loop</b> digunakan ketika jumlah perulangan belum diketahui sebelumnya. 
Selama kondisi bernilai <b>true</b>, blok kode di dalamnya akan terus dijalankan.
Jika kondisi langsung <b>false</b>, maka perulangan tidak akan dijalankan sama sekali.
</p>
<pre><code>
<script>
let counter = 1;
while (counter <= 10 ) {
document.writeln(`<p> perulangan ke ${counter}<p>`);
counter++;
}
    </script>
</code></pre>

<h4>25. DO WHILE LOOP</h4>
<p>
<b>Do While Loop</b> hampir sama seperti <b>While Loop</b>, namun bedanya blok kode akan dijalankan 
setidaknya satu kali terlebih dahulu sebelum memeriksa kondisi. 
Jadi, walaupun kondisi bernilai <b>false</b>, perulangan tetap dijalankan sekali.
</p>
<pre><code>
<script>
    let counter = 1;
    do {
      document.writeln(`<p>Perulangan ke ${counter}</p>`);
      counter++;
    } while (counter <= 10);
  </script>
</code></pre>

<h4>26. BREAK</h4>
<p>
  <b>Break</b> digunakan untuk menghentikan perulangan secara paksa, 
  meskipun kondisi loop belum terpenuhi. 
  Biasanya dipakai saat ingin keluar dari loop lebih awal.
</p>
<pre><code>
 <script>
    let counter = 1;

    while (true) {
      document.writeln(`<p>Perulangan ke-${counter}</p>`);
      counter++;

      if (counter > 10) {
        break;
      }
    }
  </script>
</code></pre>

<h4>27. CONTINUE</h4>
<p>
  <b>Continue</b> digunakan untuk melewati satu iterasi pada perulangan 
  dan langsung melanjutkan ke iterasi berikutnya. 
  Biasanya dipakai untuk <i>skip</i> kondisi tertentu tanpa menghentikan loop.
</p>
<pre><code>
 <script>
    for (let i = 1; i <= 100; i++) {
      if (i % 2 === 0) {
        continue;
      }
      document.writeln(`<p>Perulangan Ganjil ${i}</p>`);
    }
  </script>
</code></pre>

<h4>28. LABEL</h4>
<p>
  <b>Label</b> digunakan untuk memberi nama pada perulangan (loop), 
  sehingga kita bisa mengontrol loop mana yang ingin di-<b>break</b> 
  atau di-<b>continue</b> dari dalam loop bersarang (<i>nested loop</i>).
</p>
<pre><code>
   <script>
    for (let i = 1; i <= 100; i++) {
      if (i % 2 === 0) {
        continue;
      }
      document.writeln(`<p>Perulangan Ganjil ${i}</p>`);
    }
  </script>
  </code></pre>
  
<h4>29. FOR IN</h4>
<p>
  <b>For...in</b> digunakan untuk melakukan <i>iterasi</i> terhadap <b>semua properti (key)</b> dalam sebuah objek.
  Setiap kali perulangan berjalan, ia akan mengembalikan nama properti dari objek tersebut.
</p>
<pre><code>
 <script>
    const person = {
      firstName: "Rajie",
      middleName: "Al Qadri",
      lastName: "Anwar",
    };

    for (const property in person) {
      document.writeln(`<p>${property} : ${person[property]}</p>`);
    }

    const names = ["Rajie", "Al Qadri", "Anwar"];
    for (const index in names) {
      document.writeln(`<p>${index} : ${names[index]}</p>`);
    }
  </script>
</code></pre>
<p><b>Catatan:</b> 
Gunakan <code>for...in</code> hanya untuk <b>objek</b>, bukan array. 
Karena <code>for...in</code> mengembalikan nama properti (key), bukan nilai (value).
</p>

---

<h4>30. FOR OF</h4>
<p>
  <b>For...of</b> digunakan untuk melakukan perulangan pada <b>struktur data iterable</b> 
  seperti array atau string, dan mengembalikan <b>nilai</b> dari tiap elemen.
</p>
<pre><code>
  <script>
    const names = ["rajie", "al-qadri", "anwar"];
    for (const name of names) {
      document.writeln(`<p>${name}</p>`);
    }

    const fullName = "rajie al-qadri anwar";
    for (const character of fullName) {
      document.writeln(`<p>${character}</p>`);
    }
  </script>
</code></pre>
<p><b>Catatan:</b>
<code>for...of</code> cocok untuk <b>array</b> dan <b>string</b>, 
namun tidak bisa digunakan untuk objek biasa (non-iterable object).
</p>

<h4>31. WITH STATEMENT</h4>
<p>
  <b>With</b> digunakan untuk <b>memperpendek penulisan properti</b> dari sebuah objek.
  Di dalam blok <code>with</code>, kita bisa langsung mengakses properti tanpa menuliskan nama objeknya.
</p>
<pre><code>
<script>
    const person = {
      firstName: "rajie",
      middleName: "al-qadri",
      lastName: "anwar",
    };

    console.info(person.firstName);
    console.info(person.middleName);
    console.info(person.lastName);

    const firstName = "Anto";
    const lastName = "Hadi Indra";

    with (person) {
      console.info(firstName);
      console.info(middleName);
      console.info(lastName);
    }
  </script>
</code></pre>
<p><b>Catatan:</b>
Meskipun <code>with</code> membuat kode lebih singkat, 
penggunaannya <b>tidak disarankan</b> dalam JavaScript modern karena bisa menimbulkan kebingungan 
jika ada variabel dengan nama sama di luar objek.
</p>


