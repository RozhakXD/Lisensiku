# Lisensiku - Server

Lisensiku adalah sebuah projek yang dibangunkan untuk mengelola API key pengguna. Lisensiku dibangun menggunakan Flask, HTML, CSS, dan SQLite. Projek ini bertujuan untuk memudahkan pengelolaan API key pengguna.

## Cara Menggunakan

### Installasi

1. Clone repository ini ke komputer anda menggunakan perintah `git clone https://github.com/RozhakXD/Lisensiku.git`
2. Install Flask menggunakan perintah `pip install flask`
3. Install Python User Agents menggunakan perintah `pip install user-agents`
4. Jalankan aplikasi menggunakan perintah `flask run`

## Contoh Penggunaan API

Untuk menggunakan API, anda dapat membuat permintaan HTTP POST ke `https://www.lisensiku.biz.id/api/v1/validasi/` dengan mengirimkan data dalam format JSON. Berikut adalah contoh menggunakan Python:
```python
import requests
import json

platform = "nama_platform"
apikey = "apikey_pengguna"

response = requests.post(
    "https://www.lisensiku.biz.id/api/v1/validasi/", json = {"platform": platform, "apikey": apikey}
)
```

## Struktur Direktori

* `templates/`: Direktori untuk file HTML, berisi template untuk halaman web Anda.
* `static/`: Direktori untuk file CSS dan JavaScript, berisi aset statis untuk aplikasi web Anda.
* `database/`: Direktori untuk file pangkalan data SQLite, berisi konfigurasi dan data untuk basis data Anda.

## Kontribusi

Anda boleh membantu projek Lisensiku dengan membuat pull request atau membuka isu di GitHub.

## Lisensi

Projek Lisensiku dilisensikan di bawah lisensi MIT.
