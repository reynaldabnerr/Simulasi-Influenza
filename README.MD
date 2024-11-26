Simulasi Penyebaran Penyakit Influenza

Proyek ini adalah simulasi berbasis Agent-Based Modeling (ABM) menggunakan framework Mesa untuk memodelkan dinamika penyebaran penyakit influenza dalam suatu populasi. Simulasi ini memberikan wawasan tentang bagaimana penyakit menyebar, dipengaruhi oleh faktor individu dan lingkungan.

Fitur Utama

	1.	Simulasi Penyebaran Penyakit:
	•	Model mengakomodasi individu dengan status kesehatan unik: sehat, terinfeksi, atau sembuh.
	•	Penyebaran dipengaruhi oleh faktor seperti resistensi tubuh, mobilitas, usia, vaksinasi, dan keparahan gejala.
	2.	Pengumpulan Data:
	•	Data jumlah individu dalam setiap status kesehatan dikumpulkan di setiap langkah simulasi.
	3.	Visualisasi Interaktif:
	•	Grafik Line: Perubahan jumlah individu sehat, terinfeksi, dan sembuh.
	•	Grafik Pie: Distribusi status kesehatan di akhir simulasi.
	•	Grafik Area: Tren kumulatif perubahan status kesehatan.

Persyaratan Sistem

	•	Python 3.8 atau lebih baru
	•	Library Python:
	•	mesa
	•	pandas
	•	numpy
	•	plotly

Cara Menjalankan

1. Instalasi

Pastikan semua dependensi telah diinstal:

pip install mesa pandas numpy plotly

2. Struktur Direktori

Letakkan file berikut di direktori proyek:
	•	simulation_parameters.csv (parameter simulasi)
	•	individual_data.csv (data individu)

3. Jalankan Simulasi

Eksekusi file Python di terminal atau Jupyter Notebook:

python influenza_simulation.py

Atau jalankan semua sel di Jupyter Notebook jika menggunakan notebook.

4. Hasil Simulasi

	•	Visualisasi interaktif akan ditampilkan, termasuk:
	•	Grafik perubahan status kesehatan
	•	Distribusi status di akhir simulasi
	•	Data hasil simulasi disimpan dalam file simulation_results.csv.

Struktur File

	•	influenza_simulation.py: Skrip utama untuk menjalankan simulasi.
	•	simulation_parameters.csv: Parameter simulasi, termasuk probabilitas infeksi, pemulihan, dan durasi infeksi.
	•	individual_data.csv: Data atribut individu seperti resistensi, mobilitas, usia, dan status awal.
	•	simulation_results.csv: Hasil simulasi berupa data jumlah individu dalam setiap status kesehatan di setiap langkah simulasi.

Visualisasi

Grafik 1: Line Chart

Tren jumlah individu dalam setiap status kesehatan dari waktu ke waktu.

Grafik 2: Pie Chart

Proporsi status kesehatan pada langkah terakhir simulasi.

Grafik 3: Area Chart

Perubahan kumulatif status kesehatan selama simulasi berlangsung.

Penjelasan Model

Model ini menggunakan pendekatan Agent-Based Modeling (ABM), di mana setiap individu dimodelkan sebagai agen yang:
	•	Memiliki atribut unik seperti resistensi tubuh, mobilitas, usia, dan status vaksinasi.
	•	Berinteraksi dengan agen lain dalam radius tertentu, memungkinkan penyebaran infeksi.
	•	Memiliki probabilitas untuk sembuh setelah terinfeksi.

Parameter utama model meliputi:
	•	Probabilitas Infeksi: Kemungkinan agen sehat tertular dari agen terinfeksi.
	•	Probabilitas Pemulihan: Kemungkinan agen terinfeksi menjadi sembuh.
	•	Durasi Infeksi: Jumlah langkah maksimum agen tetap terinfeksi.

Hasil dan Analisis

	1.	Dinamika Penyebaran:
	•	Penyebaran influenza lebih cepat dalam populasi dengan kepadatan tinggi dan mobilitas tinggi.
	2.	Faktor Risiko:
	•	Individu dengan resistensi tubuh rendah lebih rentan terhadap infeksi.
	•	Vaksinasi dapat membantu mengurangi risiko infeksi.
	3.	Efektivitas Mitigasi:
	•	Penerapan protokol kesehatan seperti menjaga jarak dapat memperlambat penyebaran.




