# Tutorial MachineLearning-Development

# Sumber Dataset
https://www.kaggle.com/datasets/gunavenkatdoddi/eye-diseases-classification/data
# Langkah 1: Upload kaggle.json ke Google Colab
A. Dapatkan kaggle.json dari Kaggle:
  1. Masuk ke akun Kaggle .
  2. Klik pada ikon profil Anda di sudut kanan atas dan pilih "Account".
  3. Gulir ke bawah ke bagian "API" dan klik "Create New API Token".
  4. Sebuah file kaggle.json akan diunduh ke komputer .
B. Upload kaggle.json ke Google Colab:
  1. Buka Google Colab di browser.
  2. Buat notebook baru atau gunakan notebook yang ada.
  3. Klik tombol "Files" di sebelah kiri dan pilih "Upload".
  4. Pilih file kaggle.json dari komputer .
# Langkah 2: Instalasi Kaggle dan Unduh Dataset
Di dalam notebook Google Colab, kita akan menginstal paket Kaggle, mengimpor kaggle.json, dan mengunduh dataset dari Kaggle.
A. Instalasi Paket Kaggle:
Jalankan sel berikut di notebook Colab untuk menginstal kaggle:
python
Copy code
!pip install kaggle
B. Import kaggle.json:
Jalankan sel berikut untuk memindahkan file kaggle.json yang diunggah ke direktori tempat Kaggle mengharapkan untuk menemukannya.
python
Copy code
import os
# Mengunggah file kaggle.json
from google.colab import files
files.upload()
# Membuat direktori kaggle dan memindahkan kaggle.json ke dalamnya
!mkdir ~/.kaggle
!cp kaggle.json ~/.kaggle/
Pastikan file kaggle.json telah ter-upload dengan benar ke ~/.kaggle/.

C. Unduh Dataset dari Kaggle:
python
Copy code
!kaggle datasets download -d gunavenkatdoddi/eye-diseases-classification
