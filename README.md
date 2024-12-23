# Deteksi_uang
 1. Membuat Virtual Environment
Buka terminal di VS Code:
Klik Terminal > New Terminal di menu atas.
Navigasi ke folder project Anda menggunakan perintah:
cd path/to/project/folder

Buat virtual environment dengan perintah:
python -m venv venv

Ini akan membuat folder bernama venv di dalam folder project Anda.
Aktifkan virtual environment:
.\venv\Scripts\activate

2. Install Dependencies
Buat file bernama requirements.txt di dalam folder project Anda dan tambahkan daftar library yang dibutuhkan:
opencv-python
pygame
numpy
tensorflow
scikit-learn
matplotlib

Jalankan perintah berikut di terminal untuk menginstal semua dependensi:
pip install -r requirements.txt


3. Siapkan Dataset
Buat folder dataset di dalam folder project Anda.
Tambahkan dua subfolder:
train: berisi subfolder dengan nama kelas (misalnya, "10000", "20000") yang berisi gambar uang sebagai data latih.
test: folder ini akan digunakan untuk menyimpan gambar yang ditangkap dari kamera.


5. Siapkan File Audio
Buat folder audio_files di dalam folder project.
Tambahkan file audio MP3 untuk setiap kelas uang dengan format nama file sesuai nama kelas. Misalnya:
10000.mp3
20000.mp3


6. Jalankan Program
Jalankan terminal di VS Code dengan virtual environment aktif.
Eksekusi program dengan perintah:
python main.py


8. Fungsi Utama yang Akan Berjalan
Training Model: Program akan melatih model menggunakan data di folder train dan menyimpan model ke file money_detector.keras.
Capture dan Prediksi: Setelah model selesai dilatih, Anda bisa menangkap gambar dari kamera untuk memprediksi nominal uang.
Tekan Space untuk menangkap gambar.
Tekan Esc untuk keluar dari mode prediksi.

