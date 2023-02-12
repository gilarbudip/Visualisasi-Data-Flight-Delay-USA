# Visualisasi-Data-Flight-Delay-USA
Berikut adalah visualisasi terhadap data Flight Delay oleh beberapa maskapai yang terjadi di kota Amerika Serikat.
## Dataset
Data bersumber dari kaggle, dengan tautan sebagai berikut https://www.kaggle.com/datasets/jawadkhattak/us-flight-delay-from-january-2017-july-2022.
Data meliputi informasi mengenai Delay penerbangan pesawat dari beberapa maskapai yang tersebar di beberapa kota di Amerika Serikat. Data meliputi informasi waktu (bulan dan tahun), nama maskapai, nama kota, nama airport, dan beberapa informasi delay.
## Tujuan 
Tujuan dari project ini adalah memvisualisasi data fligth delay di Amerika menjadi sebuah informasi yang lebih mudah dipahami.
## Penjelasan Dataset
Data terdiri dari 101316 baris dan 24 kolom, di mana kolom terdiri dari informasi : 

![image](https://user-images.githubusercontent.com/125176865/218297494-78bcf1b9-a8ac-48f5-bc65-912b1932c00e.png)
## Steps
1. Understanding dan Cleansing data
2. Visualisasi data
## 1. Understanding dan Cleansing Data
1. Import data csv hasil pengunduhan dari Kaggle ke dalama Ms. Excel.
2. Terdapat 1 sheet data, 101316 baris data dan 24 kolom
3. Data tanggal masih terpisah menjadi kolom year dan date, untuk mempermudah visualasi gabungkan data date dan year menjadi satu kolom
4. Data nama airport, nama kota, dan nama state masih tergabung dalam satu kolom, sehingga perlu untuk dipisahkan
5. Mengapus spasi berlebih pada kolom airport, city, dan state menggunakan formula (=trim)
## 2. Visualisasi Data
Data yang sudah melewati proses cleansing selanjutnya dilakukan visualisasi menggunakan Tableau Publik.
### a. Visualisasi Delay pada Masing-masing Maskapai
Visualisasi data delay dari masing-masing maskapai diperoleh berdasarkan data (Carrier) dan data SUM(Arr Delay) 
Kemudian, pilih jenis visualisasi berupa diagram batang, serta dalam rangka mempercantik tampilan tambahkan warna pada diagram batang untuk menggambarkan nama maskapai.
### b. Visualisasi Peta Sebaran Lama Delay Berdasarkan pada Masing-masing City
Data city dan state mengandung informasi geografi mencakup longitude dan latitude, sehingga dapat dilakukan visualisi peta sebaran delay. Dalam membuat peta sebaran delay, data yang dibutuhkan adalah data (state), data (city), SUM(Arr Delay), dan Airport Name.
### c. Visualisasi Carrier Delay Percentage
Data carrier delay percentage diperoleh dari pembagian nilai pada data (Carrier Delay) terhadap (Arr Delay), kemudian pada "Measure" setting menjadi 'average'. Sesuaikan format nilai menjadi 'percentage', untuk merubah nilai menjadi persentase.
### d. Visualisasi  Total Delay
Visualisasi total delay diperoleh dari data Measure Name, yang terdiri dari SUM(Arr Delay), SUM(Carrier Delay), SUM(Carrier Delay Percentage), SUM(Late Aircraft Delay), SUM(Nas Delay), SUM(Security Delay), SUM(Weather Delay).
### e. Dashboard Visualisasi
Dashboard merupakan media akhir dari semua visualiasi yang telah dilakukan. Dashboard memungkinkan dalam membuat visualisasi akhir yang interaktif, sehingga informasi yang ditampilkan menjadi lebih menarik.
![image](https://user-images.githubusercontent.com/125176865/218299097-475c9423-ba6a-43db-a31d-5a116e5aacc5.png)

Berikut merupakan hasil visualisasi data Flight Delay dari beberapa Maskapai yang ada di Amerika Serikat. Visualisasi menghasilkan informasi yang lebih mudah dipahami, sehingga mempermudah dalam pengambilan suatu keputusan ataupun untuk dilakukannya analisis yang lebih lanjut.
