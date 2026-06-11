#  Re-Implementasi Algoritma Depth First Search (DFS) untuk Penyelesaian Lintasan dan Sirkuit Euler

Proyek ini merupakan implementasi ulang dari algoritma **Depth First Search (DFS)** untuk menyelesaikan permasalahan pencarian **Lintasan Euler (Euler Path)** dan **Sirkuit Euler (Euler Circuit)** pada sebuah graf. Proyek ini dikembangkan dengan mengacu pada penelitian yang dipublikasikan dalam *Jurnal Komtika (Komputasi dan Informatika)*.

##  Deskripsi
Permasalahan menggambarkan ulang lintasan dan sirkuit Euler tanpa melewati sisi (edge) yang telah dilalui merupakan masalah yang rumit dan memakan waktu jika diselesaikan secara manual. Penelitian ini menyelesaikan masalah tersebut dengan mengimplementasikan algoritma DFS sebagai pencari solusi, sehingga semua jalur dalam graf dapat dilalui tepat satu kali. 

Khusus untuk **Sirkuit Euler**, pencarian akan berakhir kembali ke titik asal keberangkatan. Algoritma ini dipilih karena membutuhkan memori yang relatif kecil dan efektif dalam menelusuri ruang keadaan.

##  Fitur Utama
- **Deteksi Otomatis:** Mampu mengidentifikasi apakah sebuah graf merupakan Sirkuit Euler, Lintasan Euler, atau Bukan Euler berdasarkan derajat simpulnya.
- **Pencarian Jalur DFS:** Menelusuri graf secara rekursif untuk menemukan urutan lintasan/sirkuit yang valid tanpa mengulang sisi.
- **Visualisasi Graf:** Menampilkan representasi visual dari graf beserta bobot jarak antar simpul menggunakan `networkx` dan `matplotlib`.
- **Dua Mode Pengujian:** 
  1. Pengujian dengan data nyata (Jarak antar fakultas di UNESA Lidah Wetan).
  2. Pengujian dengan input manual dari pengguna (CLI).

##  Prasyarat
Pastikan Anda telah menginstal Python 3.x di sistem Anda. Proyek ini membutuhkan pustaka pihak ketiga berikut:
- `networkx`: Untuk pembuatan dan manajemen struktur data graf.
- `matplotlib`: Untuk visualisasi/rendering graf.

Instalasi dependensi dapat dilakukan melalui terminal/command prompt:
```bash
pip install networkx matplotlib
