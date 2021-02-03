# Data Sekolah Negeri Indonesia APi 
---

Dibuat menggunakan Express JS
---
---
## Semua data saya ambil dari data referensi pendidikan [link](https://referensi.data.kemdikbud.go.id/)
---
Status : On Progress

## Dokumentasi

### Base URL : https://datasekolahapi.herokuapp.com/api/data
> Saat ini baru tersedia data sekolah sd negeri di dua daerah provinsi jakarta, yaitu kepulauan seribu dan cilandak
---

### Mendapatkan data berdasarkan jenjang : https://datasekolahapi.herokuapp.com/api/data/jenjanghurufkecil

### Contoh mendapatkan semua data berdasarkan jenjang
```Javascript
fetch('https://datasekolahapi.herokuapp.com/api/data/sd')
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(err => console.log(err));
```

### Mendapatkan data berdasarkan jenjang dan daerah : https://datasekolahapi.herokuapp.com/api/data/jenjanghurufkecil/namadaerahhurufkecil

### Contoh mendapatkan semua data berdasarkan jenjang dan daerah
```Javascript
fetch('https://datasekolahapi.herokuapp.com/api/data/sd/jakarta')
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(err => console.log(err));
```
---
### Contoh mendapatkan semua data di Javascript
```Javascript
fetch('https://datasekolahapi.herokuapp.com/api/data')
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(err => console.error(err));
```
> Untuk mencoba nya anda bisa menggunakan browser Microsoft Edge, Firefox dll, untuk google chrome saat ini masih kena cors.

Terimakasihh.
