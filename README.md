# Assignment-3-Computer-Vision-Natural-Language-Processing

## Deskripsi Proyek
Proyek ini mencakup empat kasus berbeda yang menerapkan teknik Machine Learning dan Deep Learning untuk pemrosesan gambar, deteksi objek, dan analisis teks. Setiap tugas dikerjakan menggunakan Python di Jupyter Notebook, dengan langkah-langkah yang terstruktur untuk setiap kasus.

---

## Rincian Tugas

### 1. Assignment Chapter 3 - Case 1: Peningkatan Kualitas Gambar
**Deskripsi**: Tugas ini mereplikasi teknik peningkatan gambar pada kamera smartphone untuk menghasilkan foto berkualitas tinggi meskipun dalam kondisi minim cahaya, menggunakan teknik Max Pooling dan CLAHE.

**Langkah Pengerjaan**:
1. Konversi gambar ke grayscale dan visualisasi histogram.
2. Penerapan Max Pooling menggunakan Scikit-Image dan PyTorch, serta eksplorasi Min Pooling dan Average Pooling.
3. Penerapan CLAHE untuk meningkatkan kontras gambar.
4. Menyimpan hasil gambar akhir dengan kualitas yang ditingkatkan.

**Hasil dan Kesimpulan**:
- Teknik CLAHE menghasilkan kualitas visual yang optimal untuk gambar gelap tanpa mengorbankan detail, lebih efektif dibanding Max Pooling yang menghasilkan gambar lebih terang dan Min Pooling yang lebih gelap.

### 2. Assignment Chapter 3 - Case 2: Klasifikasi Angka Tulisan Tangan dengan Transfer Learning
**Deskripsi**: Membangun model klasifikasi angka tulisan tangan dengan dataset MNIST menggunakan Transfer Learning melalui DenseNet, ResNet18, dan Vision Transformer (ViT).

**Langkah Pengerjaan**:
1. Modifikasi DenseNet untuk menyesuaikan input dan output sesuai dataset MNIST.
2. Menentukan hyperparameter batch size dan learning rate.
3. Pelatihan dan evaluasi model dengan visualisasi akurasi dan loss.
4. Eksperimen pembekuan layer DenseNet, serta uji coba pada ResNet18 dan ViT sebagai model tambahan.

**Hasil dan Kesimpulan**:
- Pembekuan layer meningkatkan kecepatan pelatihan tetapi mengurangi akurasi. Transfer learning terbukti memberi efisiensi dengan hasil cukup baik pada dataset MNIST.

### 3. Assignment Chapter 3 - Case 3: Deteksi Objek pada Video Real-Time
**Deskripsi**: Implementasi deteksi objek secara real-time menggunakan YOLOv5 pada video YouTube, dengan bounding box untuk objek yang terdeteksi.

**Langkah Pengerjaan**:
1. Instalasi library yang dibutuhkan, termasuk cap-from-youtube.
2. Panggil model YOLOv5 yang telah dilatih menggunakan PyTorch Hub.
3. Deteksi objek frame-by-frame pada video dan evaluasi kinerja deteksi dengan FPS.
4. Eksperimen deteksi objek pada video-video yang berbeda.

**Hasil dan Kesimpulan**:
- YOLOv5 akurat mendeteksi objek di video realistis, tetapi kurang akurat pada video animasi karena perbedaan data latar pelatihan.

### 4. Assignment Chapter 3 - Case 4: Klasifikasi Tweet Bencana dengan BERT
**Deskripsi**: Menggunakan model pre-trained BERT untuk mengklasifikasikan tweet sebagai informasi terkait bencana atau tidak, dengan tujuan mendukung sistem peringatan dini berbasis media sosial.

**Langkah Pengerjaan**:
1. Pembersihan data teks: menghilangkan URL, tanda baca, dan emoji.
2. Tokenisasi teks dengan BERT Tokenizer.
3. Membagi dataset menjadi train dan validation set.
4. Fine-tuning BERT pada dataset dan evaluasi hasil akurasi pada data uji.

**Hasil dan Kesimpulan**:
- Fine-tuning BERT menghasilkan akurasi tinggi (>80%) untuk klasifikasi tweet terkait bencana, menunjukkan potensi sebagai sistem peringatan dini.

---

## Menjalankan Notebook
1. Buka Google Colab.
2. Unggah dataset yang diperlukan dan ikuti petunjuk dalam setiap notebook untuk dependencies tambahan.
3. Jalankan sel-sel secara berurutan untuk analisis terstruktur dan proses pelatihan model.
