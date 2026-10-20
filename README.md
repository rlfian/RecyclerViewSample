# RecyclerViewSample - Modul 1 (PAM)

Proyek implementasi `RecyclerView` pada aplikasi Android sederhana sesuai panduan praktikum Materi 6: RecyclerView (Pemrograman Aplikasi Mobile).

## Spesifikasi Proyek
- **Nama Proyek:** RecyclerViewSample
- **Package Name:** `lat.pam.recyclerviewsample`
- **Min SDK:** API 27 (Android 8.1 Oreo)
- **Target / Compile SDK:** API 35 / 36
- **Bahasa Pemrograman:** Kotlin

## Struktur & Komponen Utama
- `activity_main.xml`: Menggunakan `androidx.constraintlayout.widget.ConstraintLayout` yang menampung `RecyclerView` (`@+id/recyclerview`).
- `card_view_design.xml`: Layout untuk tiap item list menggunakan `androidx.cardview.widget.CardView` dan `TextView` bold berukuran 20sp.
- `ItemsViewModel.kt`: Data class model penampung data teks item list.
- `CustomAdapter.kt`: Adapter turunan `RecyclerView.Adapter<CustomAdapter.ViewHolder>` untuk memetakan item data ke tampilan `card_view_design`.
- `MainActivity.kt`: Menyiapkan `LinearLayoutManager`, membuat dataset 20 item (`Item 1` s/d `Item 20`), dan memasang adapter ke `RecyclerView`.
