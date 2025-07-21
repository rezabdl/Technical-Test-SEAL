# 🧹 Technical Test – Data Cleansing & Standardization Wilayah Indonesia

Repositori ini berisi solusi technical test yang berfokus pada proses **data cleansing**, **standardisasi penamaan wilayah**, dan **penggabungan data** untuk menciptakan dataset wilayah Indonesia yang bersih dan konsisten.

## 📌 Deskripsi Singkat

Data awal terdiri dari beberapa sumber berbeda terkait informasi wilayah administrasi (kabupaten, kecamatan, kelurahan/desa). Terdapat banyak inkonsistensi dalam penamaan wilayah yang menyebabkan kegagalan saat proses merging antar tabel.

Melalui proses cleansing dan standardisasi, semua nama wilayah berhasil diselaraskan dan seluruh data berhasil digabungkan tanpa missing value.

## ⚙️ Tahapan Pengerjaan

1. **Pemeriksaan Awal**
   - Memastikan tidak ada missing value di masing-masing sumber data.
   - Mengidentifikasi ketidaksesuaian penamaan wilayah antar tabel.

2. **Proses Cleansing**
   - Hilangkan spasi berlebih, karakter asing, dan ubah ke format huruf kapital (upper case).
   - Normalisasi nama-nama wilayah (misalnya: "Kec. Sukorejo" menjadi "SUKOREJO").

3. **Penggabungan Data**
   - Melakukan merging berdasarkan kolom `kabupaten`, `kecamatan`, dan `kelurahan`.
   - Menggunakan metode `left join` untuk mempertahankan struktur data utama.

4. **Evaluasi Hasil**
   - Seluruh data berhasil di-merge secara konsisten.
   - Tidak ada nilai yang hilang di atribut utama (`kabupaten`, `kecamatan`, `kelurahan`, `kode wilayah`).
   - Inconsistency awal berhasil diminimalisir secara signifikan.

## 🖥️ Tools & Library

- Python (pandas, numpy)
- Google Colab / VS Code
- GitHub untuk dokumentasi

## 📎 File Penting

- `technical_test.ipynb`: Notebook utama berisi seluruh proses.
- `masterdesa - masterdesa`: Data master desa, kumpulan informasi desa-desa berdasarkan data BPS dan KEMENDAGRI
- `Data Dinas Sosial - Data Dinas Sosial` : Data sebagai penerima bantu sosial berdasarkan Data Dinas Sosial Provinsi Jawa Timur
- `data_final.csv`: Hasil akhir data yang sudah bersih dan lengkap.

## 📬 Kontak & Media Sosial

Jika ada pertanyaan atau ingin terkoneksi:

- 📧 Email: reza.irwansyah.aryanto@gmail.com  
- 💼 LinkedIn: [linkedin.com/in/reza-irwansyah-aryanto](https://www.linkedin.com/in/reza-irwansyah-aryanto)
- 📸 Instagram: [@rez_irw](https://www.instagram.com/rez_irw)

---

🙏 Terima kasih telah mengunjungi repositori ini!
