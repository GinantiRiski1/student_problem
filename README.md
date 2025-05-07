# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

## 🧠 Business Understanding

**Jaya Jaya Institut** merupakan institusi pendidikan tinggi yang telah berdiri sejak tahun 2000 dan telah mencetak banyak lulusan berkualitas. Namun, mereka menghadapi permasalahan serius berupa **tingginya angka siswa yang dropout** (tidak menyelesaikan studinya). Hal ini berdampak pada reputasi institusi dan efektivitas operasional pendidikan.

### ❗ Permasalahan Bisnis

- Tingginya angka **dropout mahasiswa** yang berpotensi merugikan institusi dari sisi reputasi, akreditasi, hingga kepercayaan publik.
- Tidak adanya sistem **deteksi dini** yang bisa membantu mengenali mahasiswa berisiko dropout.
- Kurangnya **dashboard** interaktif untuk memantau performa siswa secara real-time.

### 🔍 Cakupan Proyek

- Membangun sistem machine learning untuk **memprediksi status mahasiswa**: Dropout, Masih Studi, atau Lulus.
- Mengembangkan **dashboard bisnis** yang memvisualisasikan performa mahasiswa dan faktor-faktor yang memengaruhi dropout.
- Men-deploy prototype prediksi ke dalam **aplikasi web interaktif** menggunakan Streamlit.

---

## ⚙️ Persiapan

**Sumber data**:  
- Dataset performa mahasiswa disediakan oleh Jaya Jaya Institut (dengan berbagai fitur seperti nilai akademik, pekerjaan orang tua, GDP, dll).

**Setup environment**:
```bash
# Clone project (jika disimpan di repo)
git clone https://github.com/username/project-edutech.git
cd project-edutech

# Buat virtual environment
python -m venv env
source env/bin/activate  # Windows: .\env\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Jalankan aplikasi Streamlit
streamlit run app.py
```
## 📊 Business Dashboard

Dashboard yang dibuat bertujuan untuk memberikan **visualisasi performa mahasiswa** berdasarkan:

- 🎓 **Status akhir**: Graduate, Enrolled, Dropout
- 📌 **Faktor-faktor yang memengaruhi prediksi** (feature importance dari model machine learning)
- 📊 **Statistik umum** seperti jumlah mahasiswa, sebaran nilai, distribusi umur, latar belakang pendidikan orang tua, dsb.

Dashboard ini membantu pihak akademik untuk:
- Mengenali pola performa mahasiswa.
- Mengetahui variabel paling berpengaruh terhadap dropout.
- Mengambil tindakan preventif dengan data yang lebih informatif.

**Link Dashboard** (jika tersedia):  
🚧 *Contoh*: [https://streamlit-share.com/dashboard-edutech](https://streamlit-share.com/dashboard-edutech)  
_(Silakan ganti dengan link aslimu jika sudah dideploy)_

---

## 🤖 Menjalankan Sistem Machine Learning

Sistem machine learning dibangun menggunakan pendekatan **supervised classification** dengan model **Random Forest Classifier**.  
Model ini mampu memprediksi status mahasiswa berdasarkan berbagai input seperti:

- Nilai akademik semester 1 & 2
- Umur saat daftar
- Pekerjaan & pendidikan orang tua
- Faktor sosial ekonomi (GDP, pengangguran, inflasi, dll)

### 💻 Cara menjalankan prototype:
```bash
# Pastikan dependencies sudah terinstal
streamlit run app.py
```
## 🤖 Link Prototype yang Dapat Diakses

✅ [https://jaya-edutech-predictor.streamlit.app](https://jaya-edutech-predictor.streamlit.app)  
_(Ganti dengan URL asli jika sudah kamu hosting di Streamlit Cloud)_

---

## ✅ Conclusion

Melalui proyek ini, tim berhasil membangun:

- ✅ Sebuah **model prediksi status mahasiswa** dengan akurasi mencapai **94%**.
- ✅ Aplikasi **prototype interaktif** untuk deteksi dini risiko dropout.
- ✅ **Dashboard bisnis** untuk monitoring performa mahasiswa berdasarkan fitur-fitur penting.

Proyek ini diharapkan dapat membantu pihak akademik untuk:

- 🔻 **Mengurangi angka dropout** secara signifikan.
- 📌 **Memberikan intervensi personal lebih awal** berdasarkan prediksi sistem.
- 🎯 **Meningkatkan efisiensi sistem pendidikan dan kualitas lulusan.**

---

## 🚀 Rekomendasi Action Items

- 🧑‍🏫 **Bangun program bimbingan** untuk mahasiswa yang diprediksi dropout (misalnya mentoring atau konseling akademik).
- 🧾 **Integrasikan sistem ini ke SIAKAD** agar berjalan otomatis dan terhubung ke data mahasiswa secara real-time.
- 📈 **Pantau dan update model secara berkala** untuk mengikuti tren dan data terbaru.
- 💬 **Libatkan wali/orang tua siswa** sebagai bentuk komunikasi preventif untuk mendukung keberhasilan studi mahasiswa.
