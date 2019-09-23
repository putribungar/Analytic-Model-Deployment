# Analytic-Model-Deployment

# 1. Deploy Model Credit Scoring
Credit scoring merupakan sistem/cara yang digunakan oleh bank atau lembaga pembiayaan lainnya dengan melihat prediksi melalui beberapa variabel yang dapat menentukan apakah pelanggan akan terlambat bayar atau tidak terlambat. Sehingga dengan adanya model credit scoring maka lembaga tersebut dapat diketahui prediksi apakah pelanggan layak atau tidak untuk mendapatkan pinjaman.
<br>
Pada sistem ini akan dilakukan credit scoring menggunakan model algoritme random forest classifier. Algoritme Random Forest Classifier merupakan sebuah algoritme pada machine learning yang digunakan untuk menyelesaikan permasalahan. Random Forest merupakan salah satu metode dalam Decision Tree. Decision Tree adalah sebuah diagram alir yang berbentuk seperti pohon yang memiliki sebuah root node yang digunakan untuk mengumpulkan data, inner node yang berada pada root node yang berisi tentang pertanyaan tentang data dan sebuah leaf node yang digunakan untuk memecahkan masalah serta membuat keputusan. Decision tree mengklasifikasikan suatu sampel data yang belum diketahui kelasnya kedalam kelas–kelas yang ada. Random forest adalah kombinasi dari masing–masing tree yang baik kemudian dikombinasikan ke dalam satu model. 
<br>
Variabel yang digunakan pada sistem ini ada 4, yaitu :
1. LIMIT_BAL --> Jumlah maksimum uang yang dapat dipinjam oleh pelanggan
2. AGE --> Umur pelanggan
3. BILL_AMT1 --> Jumlah tagihan kredit
4. PAY_AMT1 --> Jumlah pembayaran kredit yang dilakukan pelanggan
<br>
Dengan adanya ke-4 variabel pada sistem tersebut, maka sistem dapat menghasilkan prediksi apakah pelanggan akan terlambat bayar atau tidak terlambat. Keluaran dari sistem tersebut berupa angka dan keterangan, yaitu :
 - Hasil Prediksi = 1 --> Pelanggan diprediksi akan terlambat dalam membayar
 - Hasil Prediksi = 0 --> Pelanggan diprediksi tidak akan terlambat bayar

------------------------------------------------------------------------------------------------------------------------------------------
# 2. Run "flask_app.py" as server
Sistem ini telah membuat dan melatih model dari credit scoring menggunakan algoritme random forest dengan data training pada Jupyter Notebook. Setelah itu digunakan skrip flask bersama dengan model yang terlatih di pythonanywhere. Sehingga untuk menggunakan sistem ini kalian dapat menjalankan sistemnya pada https://www.pythonanywhere.com dengan menggunakan flask_app.py sebagai servernya. 

Kalian dapat melihat code flask_app.py pada link berikut ini :
https://www.pythonanywhere.com/user/putribungar/shares/4aa23e49bb50421f9c858761b9caaedb/



------------------------------------------------------------------------------------------------------------------------------------------
# 3. Test with postman
