# Machine-Learning

# Deskripsi

Aplikasi ini menggunakan Flask sebagai backend untuk melayani model machine learning berbasis deep learning yang dilatih menggunakan MobileNetV2, NasNetMobile, dan VGG16 untuk pengenalan gambar. Aplikasi ini juga mendukung integrasi dengan library tambahan seperti Roboflow.

# Instalasi

1. Persyaratan Sistem

Pastikan sistem Anda telah memiliki:

Python 3.7 atau lebih baru

Virtual environment (opsional, tetapi direkomendasikan)

2. Instalasi Library yang Dibutuhkan

Gunakan pip untuk menginstal semua library berikut:

pip install flask keras tensorflow scikit-image pillow matplotlib roboflow flask-cors numpy opencv-python

Jika Anda menggunakan file requirements.txt, buat file tersebut dengan daftar library di atas, lalu jalankan:

pip install -r requirements.txt

# Langkah Menjalankan Aplikasi

Jalankan Skrip Pengolahan Dataset
Buka file save_dataset.py untuk mempersiapkan dataset. Jalankan file ini menggunakan perintah:

python save_dataset.py

Latih Model Machine Learning
Gunakan file Jupyter Notebook yang tersedia untuk melatih model machine learning. Langkah-langkah:

Jalankan mobilenetv2.ipynb untuk model MobileNetV2.

Jalankan nasnetmobile.ipynb untuk model NasNetMobile.

Jalankan vgg16.ipynb untuk model VGG16.

Jalankan exception.ipynb untuk model Xception (jika digunakan).

Jalankan Aplikasi Flask
Setelah model selesai dilatih, jalankan aplikasi Flask dengan perintah berikut di terminal (di folder proyek):

python apps.py

Akses Aplikasi
Aplikasi akan tersedia di browser pada alamat:

http://127.0.0.1:5000

# Struktur Folder Proyek

save_dataset.py – Skrip untuk menyimpan dataset.

mobilenetv2.ipynb – Notebook untuk melatih model MobileNetV2.

nasnetmobile.ipynb – Notebook untuk melatih model NasNetMobile.

vgg16.ipynb – Notebook untuk melatih model VGG16.

exception.ipynb – Notebook untuk melatih model Xception.

apps.py – File utama untuk menjalankan server Flask.

# Library yang Digunakan

Flask: Framework untuk membangun aplikasi web.

Keras: Library untuk deep learning.

TensorFlow: Backend untuk model deep learning.

Roboflow: Integrasi untuk manajemen dataset.

OpenCV: Prosesing gambar.

Pillow: Pemrosesan gambar berbasis Python.

Matplotlib: Visualisasi data.

Flask-CORS: Mendukung akses lintas domain pada API Flask.

NumPy: Pemrosesan numerik untuk array.

# Catatan Tambahan

Pastikan semua model dilatih dan disimpan sebelum menjalankan aplikasi Flask.

Jika menghadapi error, cek versi library yang digunakan, atau sesuaikan dependensi pada file requirements.txt.
