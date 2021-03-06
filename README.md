# Data Sekolah Negeri Indonesia APi 
---

## Dibuat menggunakan :

[![Express Logo](https://i.cloudup.com/zfY6lL7eFa-3000x3000.png)](http://expressjs.com/)

  Fast, unopinionated, minimalist web framework for [node](http://nodejs.org).

  [![NPM Version][npm-image]][npm-url]
  [![NPM Downloads][downloads-image]][downloads-url]
  [![Linux Build][travis-image]][travis-url]
  [![Windows Build][appveyor-image]][appveyor-url]
  [![Test Coverage][coveralls-image]][coveralls-url]

---
## Semua data saya ambil dari data referensi pendidikan [link](https://referensi.data.kemdikbud.go.id/)
---
Status : Pending karena banyak kegiatan

## Dokumentasi

### Base URL : https://datasekolahapi.herokuapp.com/api/data

### Data yang sudah ada saat ini : 

#### SD

| Provinsi | Kecamatan atau Kabupaten |
| --- | --- | 
| Jakarta  | Kepulauan Seribu |
| Jakarta | Cilandak |
| Jakarta | Jagakarsa | 
| Jakarta | Kebayoran Baru |
| Jakarta | Kebayoran Lama |
| Jakarta | Pasar Minggu |
| Jakarta | Pesanggrahan |
| Jakarta | Setia Budi |
| Jakarta | Tebet |
| Jakarta | Jakarta Pusat |
| Jakarta | Pulo Gadung |
| Jakarta | Cipayung |
---

### Mendapatkan data berdasarkan jenjang : https://datasekolahapi.herokuapp.com/api/data/jenjanghurufkecil

### Contoh mendapatkan semua data berdasarkan jenjang
```Javascript
fetch('https://datasekolahapi.herokuapp.com/api/data/sd')
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(err => console.log(err));
```
Hasil request contoh di atas :

![yes](https://user-images.githubusercontent.com/78361430/107293546-61049780-6a9e-11eb-9243-646713905f9e.PNG)

---
### Mendapatkan data berdasarkan jenjang dan provinsi : https://datasekolahapi.herokuapp.com/api/data/jenjanghurufkecil/namaprovinsihurufkecil

### Contoh mendapatkan semua data berdasarkan jenjang dan daerah
```Javascript
fetch('https://datasekolahapi.herokuapp.com/api/data/sd/jakarta')
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(err => console.log(err));
```
Hasil request contoh di atas :

![okegas](https://user-images.githubusercontent.com/78361430/107293742-c48ec500-6a9e-11eb-9c34-ce8559615838.PNG)

---
### Mendapatkan data berdasarkan jenjang, provinsi dan kecamatan / kabupaten : https://datasekolahapi.herokuapp.com/api/data/jenjanghurufkecil/namaprovinsihurufkecil/namapanjangkecamatanhurufkecil
> Untuk yg nama kecamatan nya panjang bisa menggunakan _ contoh : kebayoran_baru

### Contoh mendapatkan semua data berdasarkan jenjang, provinsi dan kecamatan / kabupaten
```Javascript
fetch('https://datasekolahapi.herokuapp.com/api/data/sd/jakarta/cilandak')
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
> Untuk mencoba nya anda bisa menggunakan browser Google Chrome, Microsoft Edge, Firefox dll.

[npm-image]: https://img.shields.io/npm/v/express.svg
[npm-url]: https://npmjs.org/package/express
[downloads-image]: https://img.shields.io/npm/dm/express.svg
[downloads-url]: https://npmcharts.com/compare/express?minimal=true
[travis-image]: https://img.shields.io/travis/expressjs/express/master.svg?label=linux
[travis-url]: https://travis-ci.org/expressjs/express
[appveyor-image]: https://img.shields.io/appveyor/ci/dougwilson/express/master.svg?label=windows
[appveyor-url]: https://ci.appveyor.com/project/dougwilson/express
[coveralls-image]: https://img.shields.io/coveralls/expressjs/express/master.svg
[coveralls-url]: https://coveralls.io/r/expressjs/express?branch=master

Terimakasihh.
