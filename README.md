# Web-Service-DTD

#PCDATA
Konten yang terkandung di dalam elemen yang dimaksud adalah text. Meskipun data yang ada di elemen tersebut berupa angka, tetap dianggap  sebagai text. Contoh :
<!ELEMENT telp (#PCDATA)>
2. Elemen anak Nama anak ditulis di dalam tanda kurung. Misalnya :
ELEMENT fax (phone_number)>
3. Sequence Kita dapat menuliskan elemen anak lebih dari satu pada deklarasinya. Dengan penulisan ini dimaksudkan untuk menuliskan elemen anak lebih dari satu elemen. Misalnya :
<!ELEMENT nama (nama_depan,nama_belakang)>
4. Jumlah anak Penulisan jumlah anak dari suatu elemen dapat kita tuliskan dengan cara menambahkan tanda berikut pada akhir nama elemen. Karakter Arti
+ Muncul satu kali atau lebih. Minimal muncul satu kali
* Muncul 0 kali atau lebih
? Boleh tidak muncul, tapi jika muncul maksimal 1 kali
| Fungsi ATAU
Contoh penggunaannya sebagai berikut :
<!ELEMENT mahasiswa (telp+)>
Artinya, elemen mahasiswa memiliki satu atau lebih elemen telp.
5. Elemen Kosong adalah sebuah tag yang tidak memiliki elemen nilai. Penulisannya dapat berupa :
<image source="bus.jpg" width="152" height="345" alt="Alan Turing
standing in front of bus"/>
Dengan deklarasi elemennya :
<!ELEMENT image EMPTY>
6. Any Kita dapat mengijinkan apapun dapat berada pada suatu elemen. Penulisan deklarasinya adalah :
<!ELEMENT page ANY>
