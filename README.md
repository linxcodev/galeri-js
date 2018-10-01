# Membuat galeri dengan javascript

### Inisialisasi variable
```javascript
var nomor = 0
```

### Ganti gambar menggunakan Javascript
```javascript
function ganti(angka) {
   nomor = angka  
   var lokasi = 'gambar/' + angka + '.png'
   document.getElementById('galeri').src = lokasi
    
   // untuk mematikan fungsi asli dari element html
   return false
}
```

### Tombol sebelum dan sesudah (Next and Previous)
```javascript
function sebelum() {
   nomor -= 1
      
   if (nomor < 0)
     nomor = 4

   var lokasi = 'gambar/' + nomor + '.png'
   document.getElementById('galeri').src = lokasi
      
   return false
}

function sesudah() {
   nomor += 1
      
   if (nomor > 4)
   nomor = 0

   var lokasi = 'gambar/' + nomor + '.png'
   document.getElementById('galeri').src = lokasi
      
   return false
}
```
