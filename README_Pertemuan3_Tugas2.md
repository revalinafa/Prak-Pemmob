**File hasil running program = https://drive.google.com/file/d/1vRPCSrdaqhAWsMkhSDh5wgXEqkbtLwO4/view?usp=sharing**

# 📱 Praktikum Pemrograman Mobile – Pertemuan 2  
### **View Binding & Navigasi**

## 📖 Deskripsi
Project ini merupakan implementasi materi **View Binding** dan **Navigasi** pada pemrograman mobile berbasis **Kotlin** dan **Android Studio**.  
Tujuan utama dari praktikum ini adalah memahami cara:
- Mengakses komponen layout dengan **View Binding**.  
- Membuat **reusable layout** agar lebih efisien.  
- Menggunakan **Intent (explicit & implicit)** untuk navigasi antar activity.  

---

## 🛠️ Fitur yang Diimplementasikan
1. **Konfigurasi Resources**
   - Penambahan teks pada `strings.xml` (alamat, telepon, email, IG, dll).  
   - Import assets drawable (`ic_phone`, `ic_email`, `ic_location`, `ic_himpunan`, dll).  

2. **Reusable Layout**
   - Membuat layout `layout_menu.xml` dengan struktur **CardView** berisi `ImageView` dan `TextView`.  
   - Reusable layout ini dipanggil di activity lain menggunakan `<include>`.  

3. **Activity Baru**
   - `Halaman2Activity.kt` dengan layout `activity_halaman2.xml`.  
   - Menampilkan profil lulusan, gambar gedung, logo unsoed, dan informasi kontak.  

4. **Navigasi**
   - **Explicit Intent**: pindah dari `MainActivity` ke `Halaman2Activity`.  
   - **Implicit Intent**:  
     - Buka Google Maps (lokasi kampus).  
     - Buka email client.  
     - Buka aplikasi telepon (dialer).  
     - Buka Instagram HMIF.  

5. **Optimize Import**
   - Membersihkan import yang tidak terpakai untuk menjaga kerapihan kode.  

---

## 📂 Struktur Project
```
app/
 ├── java/com/example/ifunsoedmobile/
 │   ├── MainActivity.kt
 │   ├── Halaman2Activity.kt
 │
 ├── res/
 │   ├── layout/
 │   │   ├── activity_main.xml
 │   │   ├── activity_halaman2.xml
 │   │   └── layout_menu.xml
 │   ├── drawable/
 │   │   ├── ic_phone.xml
 │   │   ├── ic_email.xml
 │   │   ├── ic_location.xml
 │   │   ├── ic_himpunan.xml
 │   │   ├── teknik_unsoed_2.png
 │   │   └── lambang_unsoed.png
 │   ├── values/
 │   │   └── strings.xml
```

---

## ▶️ Cara Menjalankan
1. Clone repository:
   ```bash
   git clone https://github.com/revalinafa/Prak-Pemmob.git
   ```
2. Buka project di **Android Studio**.  
3. Pastikan **View Binding** sudah diaktifkan di `build.gradle.kts`:  
   ```kotlin
   android {
       buildFeatures {
           viewBinding = true
       }
   }
   ```
4. Sync project (`Sync Now`).  
5. Jalankan aplikasi di **emulator** atau **device Android**.  

---

## 📸 Screenshot Tampilan
- Halaman 1 (MainActivity): tombol navigasi ke halaman 2.  
- Halaman 2 (Halaman2Activity): menampilkan informasi profil lulusan dan menu (telepon, email, lokasi, IG).  

---

## 📚 Referensi
- [View Binding – Android Developer](https://developer.android.com/topic/libraries/view-binding?hl=id)  
- [ConstraintLayout – Android Developer](https://developer.android.com/develop/ui/views/layout/constraint-layout)  
- [Intents & Navigation – Android Developer](https://developer.android.com/guide/components/intents-common?hl=id)  
- Materi Praktikum Pemrograman Mobile – Universitas Jenderal Soedirman (2025)  
