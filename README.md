Nama : MUHAMMAD RABBANI ARABI
Kelas : TI.24.a5
Nim : 312410632
1.	Membuat codingan dasar
 

Hasil dari codingan atas
 
2.	Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen

 

Hasil dari menambahkan codingan di atas

 

Selanjutnya

3.	Kemudian tambahkan deklarasi inline CSS pada tag <p> seperti berikut.

 

Hasil dari menambahkan codingan di atas

 



4.	Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut.

 

Hasil dari menambahkan codingan di atas

 


Untuk memisahkan file CSS dari HTML supaya lebih rapih , dan mudah di maintain,dan bisa dipakai ulang di banyak halaman web

   
 
5.	Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file
style_eksternal.css, tambahkan kode berikut.

 

Hasil dari menambahkan codingan di atas

 

Tugas
1.	
 

Ketika klik CSS dasar pada halaman web akan muncul ini
 
2.	H1 {......} 
•	Selector ini langsung memilih semua elemen <h1> di halaman.
•	Artinya, semua <h1> yang ada di halaman akan dapat gaya CSS yang sama.
#Intro h1 {.....}
•	Selector ini lebih spesifik, artinya hanya <h1>yang ada di dalam elemen dengan id="intro" yang akan dipengaruhi.
•	<h1> lain di luar elemen dengan id intro tidak akan terpengaruh.
3.	A. Internal CSS (di dalam <style>...</style>):
  h1 {
  font-size: 24px;
  color: #0F189F;
  text-align: center;
  padding: 20px 10px;
}
Semua <h1> akan berwarna biru tua #0F189F.
B.Eksternal CSS (dipanggil lewat):
<link rel="stylesheet" href="style_eksternal.css" type="text/css">
Misalnya di style_eksternal.css  punya aturan:
h1 {
  color: green;
}
Maka <h1> akan jadi hijau, tapi bisa ditimpa oleh internal CSS (karena internal ditulis setelah eksternal)
C. Inline CSS (langsung di atribut style):
<p style="text-align: center; color: #ccd8e4;">
Walaupun internal atau eksternal mengatur warna <p>, tetap warna yang muncul = abu muda #ccd8e4 karena inline CSS punya prioritas paling tinggi.

4. 
•  Inline CSS → paling tinggi.
•  ID selector (#id) → lebih kuat daripada class.
•  Class selector (.class), pseudo-class (:hover), attribute selector → di bawah ID.
•  Tag selector (p, h1, dll) → paling lemah.
Contoh codingan
•	HTML
<p id="paragraf-1" class="text-paragraf">
  Ini adalah paragraf contoh.
</p>
•	CSS
/* selector class */
.text-paragraf {
  color: blue;
  font-size: 16px;
}

/* selector id */
#paragraf-1 {
  color: red;
  font-size: 20px;
}




