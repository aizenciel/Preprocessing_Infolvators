**Data Cleansing**

**A. Handle missing values** 
" Tidak ada missing value pada hasil pengecekan "

**B. Handle duplicated data** 
" Tidak ada Duplicate data pada hasil penecekan "

**C. Handle outliers** 
" Menemukan beberapa outliers menggunakan metode IQR untuk menentukan outliers yang didapatkan sebanyak Number of outliers in balance: 4729 , dilakukan penghapusan outliers untuk mendapatkan  data yang berkualitas "

**D. Feature transformation**
" Kemudian dalam membangun model Machine Learning, kami menambah feature baru berupa melakukan Log Transformation pada kolom Balance , mengapa hal ini dilakukan ? Mengingat dari Data Kolom Balance terdapat skewnes pada kolom tersebut dan perlu melakukan Log untuk memperkecil skala dan mengurangi skewnes yang terjadi karena nilai diluar atau 0 dan minus , Kami menambahkan juga kolom baru berupa “month_num” (nomor bulan) untuk membantu pengurutan data jikalau dilakukan visualisasi berdasarkan bulan "

**E. Feature encoding** 
"Untuk memudahkan membangun model machine learning di tahap selanjutnya, kami akan melakukan convert kolom”Y” yang berisi ‘Yes/No’ menjadi 1/0 (binary) pada kolom "

**F. Handle class imbalance** 
"Melakukan pengecekan value pada kolom y yang berisikan informasi y: Respons target, menunjukkan apakah nasabah telah berlangganan deposito berjangka (biner: "yes", "no") , Pada dataset ini, kami meningkatkan jumlah sample dengan menciptakan sample sintetis menggunakan oversampling metode SMOTE. "


**Feature Engineering**

**A. Feature Selection** 
" Menampilkan hasil yang paling berperngaruh seperti pada kolom numerik yaitu day,campaign dan balance_log "

**B. Feature Extraction**
" Menambahkan 2 features yang akan membantu mendapatkan insight yang jauh lebih jelas lagi yaitu features Balance_per_duration: Rasio saldo bank terhadap durasi panggilan. , Campaign_Duration_Ratio: Rasio jumlah kampanye terhadap durasi panggilan. "

**C. Feature Tambahan**
" Dibuat untuk membantu performansi model, menambahkan features baru seperti age_group.
