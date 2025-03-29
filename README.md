# Bookshelf API

Proyek ini adalah implementasi RESTful API untuk mengelola data buku.

## Fitur Utama
- **Manajemen Buku**
  - Tambah, ubah, hapus, dan ambil data buku.
- **Filter Buku**
  - Filter buku berdasarkan status baca.

## Teknologi yang Digunakan
- **Node.js** + **Hapi.js**

## Instalasi
1. Instal dependensi
```bash
npm install
```

2. Jalankan server
```bash
npm start
```

## Endpoint API

### Buku (Books)
| Method | Endpoint             | Deskripsi                    |
|---------|----------------------|------------------------------|
| `POST`   | `/books`              | Tambah buku baru             |
| `GET`    | `/books`              | Ambil daftar buku            |
| `GET`    | `/books/{bookId}`     | Ambil detail buku            |
| `PUT`    | `/books/{bookId}`     | Ubah data buku               |
| `DELETE` | `/books/{bookId}`     | Hapus buku                   |

### Filter Buku
| Method | Endpoint             | Deskripsi                    |
|---------|----------------------|------------------------------|
| `GET`    | `/books?reading=1`   | Filter buku yang sedang dibaca|
| `GET`    | `/books?finished=1`  | Filter buku yang telah selesai|

