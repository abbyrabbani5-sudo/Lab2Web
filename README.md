Nama : MUHAMMAD RABBANI ARABI
Kelas : TI.24.a5
Nim : 312410632
1.	Membuat codingan dasar
 <img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/65875364-beb1-43da-b364-15aaf3930c07" />


Hasil dari codingan atas

 <img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/78103883-f603-4c91-b9ec-f8e368375310" />

2.	Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen

 <img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/b7af6634-7951-49e6-8a9d-cb61733ee7b3" />


Hasil dari menambahkan codingan di atas

 <img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/764d13a7-f681-4d14-8580-d0c3aea42eca" />


Selanjutnya

3.	Kemudian tambahkan deklarasi inline CSS pada tag <p> seperti berikut.
<img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/a1c93305-d0e3-431d-91d3-91e555dec754" />

 

Hasil dari menambahkan codingan di atas

 
<img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/852b4d46-8690-423c-a1ec-0fb5d697cb1f" />



4.	Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut.
<img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/e229a4c6-59d8-4db7-b0d8-0b3c7a31e1f9" />

 

Hasil dari menambahkan codingan di atas

 
<img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/22238e1f-3023-42a3-b5b8-9bb0ad9cddb2" />


Untuk memisahkan file CSS dari HTML supaya lebih rapih , dan mudah di maintain,dan bisa dipakai ulang di banyak halaman web

  <img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/fcd4f877-f7c3-4cf7-84e2-a068234b26b5" />

 
5.	Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file
style_eksternal.css, tambahkan kode berikut.
<img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/153fc965-0398-485e-870a-0906c33f92ac" />

 

Hasil dari menambahkan codingan di atas

 <img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/83576bdd-4757-4dd5-ab83-8d2d5c2926dc" />


Tugas
1.	<img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/5b56df78-2c2b-456f-b96f-fcc5b7e6bc05" />

 

Ketika klik CSS dasar pada halaman web akan muncul ini
 <img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/ec1ba405-fb7c-4640-90e5-06bdfa121a21" />

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




