# Analytic-Model-Deployment
----------------------------------------------------------------------------------------------------------------------------------------
# 1. Deploy Model Credit Scoring
Credit scoring merupakan sistem/cara yang digunakan oleh bank atau lembaga pembiayaan lainnya dengan melihat prediksi melalui beberapa variabel yang dapat menentukan apakah pelanggan akan terlambat bayar atau tidak terlambat. Sehingga dengan adanya model credit scoring maka lembaga tersebut dapat diketahui prediksi apakah pelanggan layak atau tidak untuk mendapatkan pinjaman.
<br><br>
Pada sistem ini akan dilakukan credit scoring menggunakan model algoritme random forest classifier. Algoritme Random Forest Classifier merupakan sebuah algoritme pada machine learning yang digunakan untuk menyelesaikan permasalahan. Random Forest merupakan salah satu metode dalam Decision Tree. Decision Tree adalah sebuah diagram alir yang berbentuk seperti pohon yang memiliki sebuah root node yang digunakan untuk mengumpulkan data, inner node yang berada pada root node yang berisi tentang pertanyaan tentang data dan sebuah leaf node yang digunakan untuk memecahkan masalah serta membuat keputusan. Decision tree mengklasifikasikan suatu sampel data yang belum diketahui kelasnya kedalam kelas–kelas yang ada. Random forest adalah kombinasi dari masing–masing tree yang baik kemudian dikombinasikan ke dalam satu model. 
<br><br>
Variabel yang digunakan pada sistem ini ada 4, yaitu :
1. LIMIT_BAL --> Jumlah maksimum uang yang dapat dipinjam oleh pelanggan
2. AGE --> Umur pelanggan
3. BILL_AMT1 --> Jumlah tagihan kredit
4. PAY_AMT1 --> Jumlah pembayaran kredit yang dilakukan pelanggan
<br><br>
Dengan adanya ke-4 variabel pada sistem tersebut, maka sistem dapat menghasilkan prediksi apakah pelanggan akan terlambat bayar atau tidak terlambat. Keluaran dari sistem tersebut berupa angka dan keterangan, yaitu :
 - Hasil Prediksi = 1 --> Pelanggan diprediksi akan terlambat dalam membayar
 - Hasil Prediksi = 0 --> Pelanggan diprediksi tidak akan terlambat bayar

----------------------------------------------------------------------------------------------------------------------------------------
# 2. Run "flask_app.py" as server
Sistem ini telah membuat dan melatih model dari credit scoring menggunakan algoritme random forest dengan data training pada Jupyter Notebook. Setelah itu digunakan skrip flask bersama dengan model yang terlatih di pythonanywhere. Sehingga untuk menggunakan sistem ini kalian dapat menjalankan sistemnya pada https://www.pythonanywhere.com dengan menggunakan flask_app.py sebagai servernya. 
<br><br>
Kalian dapat melihat code flask_app.py pada link berikut ini :
https://www.pythonanywhere.com/user/putribungar/shares/4aa23e49bb50421f9c858761b9caaedb/

------------------------------------------------------------------------------------------------------------------------------------------
# 3. Test with postman
Apabila kalian mau melakukan testing dengan data kalian, kalian dapat langsung memasukkan data kalian pada POSTMAN yang dapat kalian dapatkan dengan memasang POSTMAN sebagai ekstensi dari chrome webstore maka aplikasi atau ekstensi itu hanya akan berjalan di chrome dan tidak ada peramban lain. Atau kalian dapat juga menginstall POSTMAN agar ada pada desktop kalian.
<br><br>
Jika POSTMAN sudah ada, maka kalian dapat membukanya dan memasukkan data kalian untuk kemudian di proses menggunakan model yang telah saya sediakan.
Tahap - tahapnya adalah :
1. Buka Postman
2. Ganti method menjadi "POST" (Kalian dapat melihat screenshot "datatest.png" yang telah saya upload)
3. Masukkan putribungar.pythonanywhere.com/api pada "Enter Request URL" untuk meunggah model yang telah saya kembangkan
3. Klik "Body", lalu klik "raw" dan pilih "JSON(application/json)" (Kalian dapat melihat screenshot "datatest.png")
4. Setelah itu kalian dapat memasukkan data kalian dengan variabel yang telah ditentukan diatas yaitu LIMIT_BAL, AGE, BILL_AMT1, PAY_AMT1 (Kalian dapat melihat formatnya di screenshot "datatest.png", atau kalian dapat melihat scriptnya pada "datatesting.txt" yang telah saya upload)
5. Klik "SEND", kemudian output akan terlihat dibagian bawah (Contoh output dapat dilihat pada "output.png)
<br>
Kalian dapat mengganti nilai dari variabel untuk testing dengan data yang kalian miliki.
<br>
Selamat mencoba ya :)

----------------------------------------------------------------------------------------------------------------------------------------
