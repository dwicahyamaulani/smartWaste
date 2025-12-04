# **SMARTWASTE CLASSIFIER**

Klasifikasi Sampah Organik vs Anorganik

## **Project Structure**

```
SMARTWASTE/
│
├── DATASET/
│   ├── ANORGANIK/
│   └── ORGANIK/
│
├── projekakhir.ipynb      ← Notebook utama
├── R_101.jpg              ← Sample test image
├── O_12582.jpg            ← Sample test image
```

> **Catatan:**
> Untuk menjalankan notebook, *wajib* memiliki folder **DATASET/** dengan dua subfolder **ANORGANIK/** dan **ORGANIK/** di direktori yang sama dengan notebook.

## **Deskripsi Singkat**

Project ini membangun sistem klasifikasi sampah menjadi **organik** dan **anorganik** menggunakan:

* **PCD Preprocessing**
  (Remove background/GrabCut, HSV conversion, smoothing)
* **Feature Extraction**
  (Color, texture/GLCM, shape)
* **CNN Classification**
  (3× Conv2D + MaxPooling + GAP + Dense)
* **Evaluation**
  (Confusion matrix + accuracy, precision, recall, F1)

Tujuan project adalah membuat sistem klasifikasi otomatis yang stabil untuk mendukung pemilahan sampah.

## **Cara Menjalankan**

1. **Clone repository**

   ```bash
   git clone <repo-link-kamu>
   cd SMARTWASTE
   ```

2. **Pastikan dataset berada di struktur berikut:**

   ```
   SMARTWASTE/
   └── DATASET/
       ├── ANORGANIK/
       └── ORGANIK/
   ```

   *Jika folder tidak sesuai, notebook tidak dapat membaca dataset.*

3. **Install dependencies minimal**

   ```bash
   pip install tensorflow opencv-python numpy matplotlib seaborn scikit-learn scikit-image
   ```

4. **Buka dan jalankan notebook**

   ```
   projekakhir.ipynb
   ```

   Jalankan semua cell mulai dari preprocessing → feature extraction → training CNN → evaluasi → prediksi.

## **Hasil Utama**

* **Accuracy:** ~0.84
* **Precision (Macro):** ~0.84
* **Recall (Macro):** ~0.84
* Confusion matrix menunjukkan performa stabil dengan beberapa misclassification.

## **Pengembangan Lanjutan**

Model dapat ditingkatkan dengan menambah variasi dataset, memperkuat preprocessing, dan menguji arsitektur CNN yang lebih robust.
Sistem ini juga berpotensi diintegrasikan ke perangkat pemilah sampah otomatis untuk klasifikasi real-time.


## **Contributors**

* **Aufii Fathin Nabila - 23515020111002 - Teknik Informatika**
* **Dwi Cahya Maulani - 23515020111002 - Teknik Informatika**
