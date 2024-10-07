---
title: Algoritma

---

# Algoritma
## Definisi Algoritma
Dalam Kamus Besar Bahasa Indonesia (KBBI) daring, algoritma adalah prosedur sistematis untuk memecahkan masalah matematis dalam langkah-langkah terbatas. Selain itu, algoritma juga bisa diartikan sebagai urutan logis dalam pengambilan keputusan untuk memecahkan masalah.

#### Ciri-ciri Algoritma
Adapun sejumlah ciri-ciri algoritma yang baik sehingga lebih mudah ketika diproses, yakni sebagai berikut:

##### 1. Precise
Ciri-ciri algoritma yang pertama adalah precise, maksudnya adalah harus tepat, benar, dan teliti. Jadi, setiap instruksi dalam algoritma wajib ditulis secara benar dan teliti tanpa adanya keraguan.

Jika algoritma diterapkan secara presisi, maka setiap instruksi dapat dinyatakan secara eksplisit tanpa menghilangkan bagian apapun, karena dianggap sudah mengerti.

##### 2. Menyusun Jumlah Langkah atau Instruksi
Setiap langkah dalam menyusun algoritma harus tertata dengan baik, artinya disusun dari awal hingga akhir, meskipun saat diproses akan ada sejumlah data yang berbeda.

##### 3. Efektif
Seluruh instruksi yang ingin dikerjakan harus disampaikan secara jelas dan efektif. Dengan begitu, tidak ada lagi kesalahan ataupun kebingungan saat sedang memproses data.

##### 4. Terminate
Dalam menyusun algoritma pemrograman, tentu harus terminate (berakhir) sehingga tidak berjalan terus.

##### 5. Output yang Dihasilkan Tepat
Ciri-ciri yang terakhir adalah setiap output yang dihasilkan dalam algoritma harus tepat dan sesuai yang dikehendaki. Hal ini dapat terjadi jika setiap langkah dalam algoritma terbilang logis dan bisa diikuti dengan seksama.

#### Jenis-jenis Proses Algoritma
Dalam buku Struktur Data dan Algoritma dengan C ++ oleh Anita Sindar, ada berbagai jenis dalam proses algoritma, yakni sebagai berikut:

##### 1. Sequence Process
Sequence process adalah instruksi yang dikerjakan secara sekuensial atau berurutan.

##### 2. Selection Process
Dalam hal ini, instruksi akan dikerjakan apabila telah memenuhi berbagai kriteria tertentu.

##### 3. Iteration Process
Jenis algoritma ini mengharuskan instruksi dikerjakan selama memenuhi situasi dan kondisi tertentu.

##### 4. Concurrent Process
Concurrent process adalah sejumlah instruksi yang dikerjakan secara bersamaan.

#### Syarat Algoritma
Menurut Donald E. Knuth yang dikutip dari E-jurnal milik binus.ac.id, sebuah algoritma harus memenuhi sejumlah syarat, yakni sebagai berikut:

##### 1. Finiteness
Syarat yang pertama harus memenuhi finiteness, yakni algoritma harus berakhir (terminate) setelah melakukan sejumlah langkah proses.

##### 2. Definiteness
Dalam hal ini, setiap langkah algoritma harus didefinisikan dengan tepat dan tidak menimbulkan makna ganda (ambiguous).

##### 3. Input
Setiap algoritma memerlukan data sebagai masukkan untuk diolah.

##### 4. Output
Setiap algoritma memberikan satu atau lebih hasil setelah diproses.

##### 5. Effectiveness
Syarat yang terakhir adalah memenuhi effectiveness, artinya langkah-langkah algoritma dikerjakan dalam batas waktu yang wajar.

#### Contoh Penulisan Algoritma
Setelah memahami apa itu algoritma, kini detikers perlu mengetahui contoh penulisan algoritma yang benar. Simak di bawah ini contoh penulisan algoritma dalam menghitung luas dan volume sebuah bak tampung:

Start

Program Hitung_Luas_Volume_Bak_Tampung

Deklarasi

float panjang, lebar, tinggi, L_Bak, V_Bak

Deskripsi

Baca Panjang

Baca lebar

Baca tinggi

Hitung L_Bak = panjang x lebar

Hitung V_Bak = panjang x lebar x tinggi

Cetak L_Bak

Cetak V_Bak

End 

### Algoritm squential Search
#### Pengertian Sequential Search
Sequential search adalah teknik pencarian data yang dilakukan dengan cara membandingkan setiap elemen data satu per satu, mulai dari elemen pertama hingga elemen yang dicari ditemukan. Proses ini terus berlanjut hingga data ditemukan atau seluruh elemen telah diperiksa.

Algoritma ini termasuk salah satu algoritma pencarian yang paling sederhana dan sering digunakan dalam situasi di mana data tidak memiliki struktur tertentu.

#### Fungsi Sequential Search
**1.** Digunakan untuk mencari data dengan melakukan        proses membandingkan setiap elemen larik secara beruntun satu persatu, mulai dari elemen pertama, sampai elemen yang dicari ditemukan, atau seluruh elemen sudah diperiksa .

**2**.Dapat digunakan untuk pengelolaan data, seperti fungsi pencarian data barang pada master data barang .

**3**.Dalam konteks pengujian kecepatan pencarian, Algoritma Sequential Search dapat digunakan dengan fungsi microtime untuk mengevaluasi kecepatan pencarian data

#### Cara Kerja Sequential Search
Algoritma Sequential Search bekerja dengan melakukan perbandingan satu persatu secara beruntun dalam kumpulan data dengan data yang dicari sampai data tersebut ditemukan atau tidak ditemukan.

Proses pencarian ini hanya melakukan pengulangan data dari 1 sampai dengan jumlah data (N). Setiap pengulangan, dilakukan perbandingan data ke-i dengan data yang sedang dicari. Jika data sama dengan yang dicari, berarti data telah berhasil ditemukan. Sebaliknya, jika sampai akhir pengulangan tidak ada data yang sama dengan yang dicari, berarti data tidak ditemukan.

#### Langkah-langkah urutan Algoritma Sequential Search:
**1.** i <- 0
**2.** Ketemu <- false
**3.** Selama (tidak ketemu) dan ( i < N ) kerjakan baris 4.
**4**.Jika ( Data [i]=key ) maka ketemu <- true. Jika tidak, i ditambah 1. Jika ketemu, maka i adalah indeks dari data yang dicari.
#### Contoh Penerapan Algoritma Sequential Search
def sequential_search(data, target):
i = 0
found = False

while not found and i < len(data):
if data[i] == target:
found = True
else:
i += 1

if found:
return i # Mengembalikan indeks elemen yang ditemukan
else:
return -1 # Mengembalikan -1 jika elemen tidak ditemukan

#### Contoh penggunaan
data_list = [4, 2, 7, 1, 9, 5, 8]
target_element = 7

result = sequential_search(data_list, target_element)

if result != -1:
print(f”Elemen {target_element} ditemukan pada indeks {result}.”)
else:
print(f”Elemen {target_element} tidak ditemukan dalam list.”)

#### Penjelasan program di atas:
* Fungsi sequential_search: Menerima list data dan elemen target yang dicari. Melakukan pencarian sekuensial dengan menggunakan algoritma Sequential Search.
* Iterasi While:Selama belum ditemukan (not found) dan indeks i masih dalam rentang data, lakukan perulangan.
* Pemeriksaan Elemen:Pada setiap iterasi, periksa apakah elemen pada indeks ke-i sama dengan elemen yang dicari (target).
* Penentuan Hasil:Jika elemen ditemukan, fungsi mengembalikan indeks elemen tersebut.Jika elemen tidak ditemukan, fungsi mengembalikan -1.

#### Contoh Penggunaan:
Sebuah list data_list dibuat sebagai himpunan data.
Elemen yang dicari adalah 7.
Hasil pencarian disimpan dalam variabel result dan kemudian ditampilkan.
Dalam contoh ini, kita dapat melihat bahwa elemen 7 ditemukan pada indeks ke-2 dalam list data_list
### Kelebihan dan Kekurangan Algoritma Sequential Search
#### Kelebihan:
* Proses pencarian menggunakan Sequential Search cenderung lebih cepat dan efisien untuk jumlah data yang terbatas atau tidak terlalu banyak
* Algoritma yang digunakan juga lebih sederhana atau tidak terlalu rumit.
* Untuk data yang jumlahnya terbatas, pencarian relatif lebih cepat .
* Jika data yang dicari berada di awal atau dekat awal, proses pencarian dapat lebih efisien .
#### Kekurangan:
* Kurang efisien dan kurang cepat untuk mencari suatu data dalam jumlah yang besar .
* Algoritma Sequential Search kurang efisien jika data yang dicari berada di posisi akhir .
* Tidak baik untuk pencarian data dalam jumlah yang besar karena algoritma pemrogramannya lebih rumit dibandingkan dengan Binary Search .
* Jika data yang dicari berada di posisi akhir, pencarian secara sekuensial dari awal sampai akhir menjadi kelemahan

### Algoritma Binary Search
Binary search adalah sebuah algoritma pencarian yang digunakan untuk mencari elemen tertentu dalam sebuah array atau daftar yang sudah diurutkan. Algoritma ini bekerja dengan membagi daftar menjadi dua bagian, kemudian memeriksa elemen tengahnya. Jika elemen yang dicari sama dengan elemen tengah ini, pencarian selesai. Jika tidak, algoritma akan menentukan apakah elemen yang dicari lebih besar atau lebih kecil dari elemen tengah, dan kemudian hanya memeriksa salah satu bagian dari daftar yang masih mungkin mengandung elemen yang dicari. Proses ini terus berlanjut hingga elemen yang dicari ditemukan atau daftar habis diperiksa.

#### Cara Kerja Binary Search
Cara kerja binary search sangat sederhana. Algoritma ini beroperasi pada daftar yang sudah diurutkan. Berikut adalah langkah-langkah utama dalam binary search:

1. Tentukan Rentang Pencarian Awal: Di awal pencarian, kita memiliki seluruh daftar sebagai rentang pencarian. Rentang ini didefinisikan dengan dua indeks, yaitu awal dan akhir, yang mengacu pada elemen pertama dan terakhir dalam daftar.
2.  Hitung Elemen Tengah: Temukan indeks tengah di dalam rentang pencarian dengan rumus tengah = (awal + akhir) / 
3. Periksa Elemen Tengah: Bandingkan elemen tengah dengan elemen yang ingin Anda cari. Jika elemen tengah sama dengan elemen yang dicari, maka pencarian selesai, dan Anda telah menemukan elemennya.
4. Perkecil Rentang Pencarian: Jika elemen tengah lebih besar dari elemen yang dicari, maka Anda dapat memastikan bahwa elemen yang dicari hanya mungkin ada di sebelah kiri elemen tengah. Oleh karena itu, perkecil rentang pencarian menjadi antara awal dan tengah - 1. Jika elemen tengah lebih kecil, perkecil rentang menjadi antara tengah + 1 dan akhir.
5. Ulangi Langkah 2–4: Ulangi proses ini sampai Anda menemukan elemen yang dicari atau rentang pencarian menjadi kosong.

Algoritma ini terus membagi rentang pencarian menjadi setengah hingga elemen yang dicari ditemukan atau rentang habis. Hal ini menghasilkan kompleksitas waktu O(log n), di mana n adalah jumlah elemen dalam daftar. Ini sangat efisien dibandingkan dengan pencarian linear yang memiliki kompleksitas waktu O(n).
#### Contoh kasus dengan menggunakan pemrograman python
![image](https://hackmd.io/_uploads/SywtEAwAC.png)
Mari kita ilustrasikan penggunaan binary search dengan sebuah contoh. Misalkan kita memiliki kumpulan data berupa [1, 3, 5, 7, 9, 11, 13, 15] dan kita ingin mencari target dengan angka 7.

Dalam binary search, langkah pertama adalah membagi panjang data dengan 2. Panjang data awal adalah 8, kemudian kita bagi 2, yang menghasilkan 4. Sekarang, kita lihat indeks ke-4 dari data, yaitu angka 9.

Selanjutnya, kita bandingkan angka target (7) dengan hasil indeks ke-4 (9). Jika target lebih besar dari 9, maka angka [1, 3, 5, 7, 9] akan dihilangkan dari kumpulan data. Namun, jika target lebih kecil dari 9, maka angka [9, 11, 13, 15] akan dihilangkan.

Proses ini terus berlanjut, dengan data yang tersisa, hingga target menemukan angka yang sama dalam kumpulan data. Binary search memungkinkan kita untuk secara efisien mencari nilai yang diinginkan dalam set data yang besar dengan mengurangi setengah opsi pada setiap langkahnya.

**Berikut contoh dengan menggunakan python.**
```
def binary_search(sorted_list, target):
    left = 0
    right = len(sorted_list) 
    
    while left < right:
        middle = (left + right) // 2
        if sorted_list[middle] == target:
            return middle
        elif sorted_list[middle] < target:
            left = middle + 1
        else:
            right = middle

    return None

def main():
    sorted_data = [1, 3, 5, 7, 9, 11, 13, 15]
    target = 7*

    index = binary_search(sorted_data, target)
    if index is not None:
        print(f"Elemen {target} ditemukan di indeks {index}.")
    else:
        print(f"Elemen {target} tidak ditemukan dalam daftar.")

if __name__ == "__main__":
    main()
```
Dalam implementasi Python di atas, fungsi binary_search menerima daftar yang sudah diurutkan dan elemen yang ingin dicari. Kemudian, ia mengembalikan indeks elemen yang dicari jika ditemukan atau None jika tidak ditemukan. Fungsi main digunakan untuk menguji pencarian elemen tertentu dalam contoh daftar yang sudah diurutkan.

## Pseudocode adalah....
Pseudocode adalah rangkaian kode/instruksi sederhana yang digunakan programmer untuk merencanakan program komputer. Ini membantu mereka menyusun alur kerja program sebelum ditulis dalam bahasa pemrograman yang sesungguhnya.

Penggunaan struktur pseudocode ini jauh lebih sederhana sehingga mudah dipahami oleh orang awam dengan latar belakang apapun. 

Dalam proses pengembangan perangkat lunak, pseudocode adalah kode yang sangat bermanfaat untuk merencanakan dan menggambarkan algoritma program sebelum mereka mulai menulis kode sebenarnya dalam bahasa pemrograman tertentu.

### Ciri-Ciri Pseudocode
* Tidak memiliki aturan baku secara sintaks, sehingga setiap tim pengembang dapat menyusun pseudocode sesuai gaya dan preferensi mereka. 
* Pseudocode umumnya ditulis dengan bahasa Inggris untuk memudahkan integrasi ke dalam bahasa pemrograman.
* Pseudocode bukan termasuk bahasa pemrograman karena hanya berfungsi sebagai kode semu yang bersifat sementara. 
* Pseudocode umumnya lebih ringkas dibandingkan dengan algoritma dalam bahasa pemrograman yang sesungguhnya
* Penulisannya tidak menggunakan bentuk diagram karena sering kali ditulis dalam urutan suatu kejadian atau permasalahan.
* Pseudocode menggunakan bahasa yang mudah dipahami secara universal sehingga dapat diakses dan dimengerti oleh berbagai pihak, terlepas dari latar belakang pemrograman mereka.



## Big O algoritma

Notasi Big-0 adalah cara untuk mengekspresikan kompleksitas waktu (atau ruang) suatu algoritma. Notasi ini memberikan perkiraan kasar tentang berapa lama waktu yang dibutuhkan suatu algoritma untuk berjalan (atau berapa banyak memori yang digunakannya), berdasarkan ukuran input. Misalnya, suatu algoritma dengan kompleksitas waktu berarti waktu berjalan meningkat secara linear seiring dengan ukuran input.

#### Hitung Big O dari Algoritma Sequential Search

### Kompleksitas waktu

Kompleksitas waktu adalah ukuran seberapa lama waktu yang dibutuhkan suatu algoritma untuk berjalan, berdasarkan ukuran input. Hal ini dinyatakan menggunakan notasi Big-0, yang memberikan perkiraan kasar waktu berjalan. Suatu algoritma dengan kompleksitas waktu yang lebih rendah umumnya akan lebih cepat daripada suatu algoritma dengan kompleksitas waktu yang lebih tinggi.

*** Kompleksitas ruang

## referensi
Baca artikel detikedu, "Algoritma Adalah: Pengertian, Ciri-ciri, dan Berbagai Jenisnya" selengkapnya https://www.detik.com/edu/detikpedia/d-6817970/algoritma-adalah-pengertian-ciri-ciri-dan-berbagai-jenisnya

https://engineerpalsu.medium.com/mengenal-algoritma-binary-search-40a9047dab62#:~:text=Mengenal%20Algoritma%20Binary%20Search