Deskripsi Data

| Features                  | Description                                                                                                                   |
|---------------------------|-------------------------------------------------------------------------------------------------------------------------------|
|``VendorID``               | Kode ID yang menunjukkan vendor taksi.                                                                                        |
|                           | 1 = Creative Mobile Technologies, LLC                                                                                         |
|                           | 2 = VeriFone Inc.                                                                                                             |   
|``lpep_pickup_datetime``   | Tanggal dan waktu saat perjalanan taksi dimulai.                                                                              |
|``lpep_dropoff_datetime``  | Tanggal dan waktu saat perjalanan taksi berakhir.                                                                             |
|``store_and_fwd_flag``     | Menunjukkan apakah catatan perjalanan disimpan dalam memori kendaraan sebelum dikirim ke vendor. Y berarti "simpan dan lanjutkan", N berarti bukan perjalanan "simpan dan lanjutkan".                                                                                                                    |
|``RatecodeID``             | Kode tarif untuk perjalanan.                                                                                                  |
|                           |1 = Tarif standar                                                                                                              |
|                           |2 = JFK                                                                                                                        |
|                           |3 = Newark                                                                                                                     |
|                           |4 = Nassau atau Westchester                                                                                                    |
|                           |5 = Tarif yang dinegosiasikan                                                                                                  |
|                           |6 = Perjalanan kelompok.                                                                                                       |
|``PULocationID``           | ID lokasi penjemputan, yang sesuai dengan zona taksi di mana meteran (taximeter) diaktifkan.                                  |
|``DOLocationID``           | ID lokasi penurunan, yang sesuai dengan zona taksi di mana meteran (taximeter) dinonaktifkan.                                 |
|``passenger_count``        | Jumlah penumpang di dalam kendaraan.                                                                                          |
|``trip_distance``          | Jarak perjalanan dalam mil.                                                                                                   |
|``fare_amount``            | Tarif yang diukur untuk perjalanan.                                                                                           |
|``extra``                  | Biaya tambahan. Saat ini, ini hanya mencakup biaya tambahan 0,5 dolar dan 1 dolar untuk jam sibuk dan larut malam.            |
|``mta_tax``                | Pajak MTA sebesar 0,50 dolar yang otomatis aktif berdasarkan tarif yang diukur yang digunakan.                                |
|``tip_amount``             | Jumlah tip. Bidang ini otomatis diisi untuk tip kartu kredit. Tip tunai tidak termasuk.                                       |
|``tolls_amount``           | Jumlah total dari semua tol yang dibayar dalam perjalanan.                                                                    |
|``ehail_fee``              | Biaya tambahan sebesar 1 dolar yang otomatis dikenakan untuk setiap perjalanan yang dipesan melalui platform ehail.           |
|``improvement_surcharge``  | Biaya tambahan sebesar 0,30 dolar yang dinilai pada awal perjalanan. Biaya tambahan ini mulai dikenakan pada tahun 2015.      |
|``total_amount``           | Jumlah total yang dikenakan kepada penumpang. Bidang ini mencakup tarif yang diukur, biaya tambahan, mta_tax, tip_amount, dan tolls_amount ditambah biaya tambahan ehail atau improvement_surcharge.                                                                                                   |
|``payment_type``           | Kode numerik yang menunjukkan metode pembayaran.                                                                              |
|``trip_type``              | Kode yang menunjukkan apakah perjalanan adalah dari sisi jalan atau dari pengiriman yang otomatis ditetapkan berdasarkan tarif yang diukur yang digunakan tetapi dapat diubah oleh pengemudi.                                                                                                               |
|                           | 1 = Street-hail                                                                                                               |
|                           | 2 = Dispatch                                                                                                                  |
|``congestion_surcharge``   | Biaya kemacetan sebesar 2,75 dolar untuk perjalanan dengan taksi kuning dan hijau di Manhattan selatan dari 96th St. Biaya tambahan ini mulai dikenakan pada tahun 2019.                                                                                                                                  |

Analysis Conclusion

`Permintaan dan Preferensi Pelanggan`

- Permintaan taksi paling tinggi di bulan januari terjadi pada hari Rabu, 25 Januari 2023, sedangkan permintaan terendah pada 1 Januari 2023.

- Terdapat pola permintaan pada bulan Januari, Permintaan cenderung naik selama weekdays kemudian menurun ketika memasuki hari weekend.

- Puncak permintaan terjadi di sore hari, sementara permintaan paling rendah di tengah malam hingga pagi hari.

- Manhattan adalah wilayah dengan permintaan tertinggi, sedangkan State Island memiliki permintaan terendah.

- Pelanggan lebih cenderung menggunakan taksi dengan jenis tarif dalam kota dengan trip type street-hail (pemanggilan taksi dipinggir jalan) dan metode pembayaran dominan menggunakan kartu kredit atau tunai.

- Durasi perjalanan yang paling umum adalah antara 11-20 menit dan jarak yang kurang dari 2 mil.

`Distribusi Pendapatan Berdasarkan Waktu dan Wilayah`

- Terdapat rute-rute yang permintaan dan rata-rata tarif yang juga tinggi seperti dari East Harlem North ke Upper West Side North.

- Tarif rata-rata cenderung lebih mahal di tengah malam dan lebih murah di malam hari.

- Brooklyn memiliki tarif rata-rata tertinggi di pagi hari, sementara Staten Island memiliki tarif rata-rata termurah dan tidak memiliki perjalanan sama sekali di malam hari.

- Wilayah Manhattan menampilkan pola harga yang stabil sepanjang hari.

- Tip tertinggi biasanya diberikan untuk rute ke Newark Airport, sementara tip sebagai proporsi dari fare amount tertinggi terjadi di rute menuju Battery Park.
