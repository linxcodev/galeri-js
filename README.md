# Membuat galeri dengan javascript

### Inisialisasi variable
```javascript
var nomor = 0
```

### Ganti gambar menggunakan Javascript
```javascript
function ganti(angka) {
   nomor = angka  
   gantiGambar(nomor)
}
```

### Tombol sebelum dan sesudah (Next and Previous)
```javascript
function sebelum() {
  nomor--
  if (nomor < 0) nomor = 4
  gantiGambar(nomor)
}

function sesudah() {
  nomor++
  if (nomor > 4) nomor = 0
  gantiGambar(nomor)
}
```

### Function gantiGambar()
```javascript
function gantiGambar(angka) {
  var lokasi = 'gambar/' + angka + '.png'
  document.getElementById('galeri').src = lokasi

  // untuk mematikan fungsi asli dari element html
  return false
}
