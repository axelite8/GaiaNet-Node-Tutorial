# GaiaNet-Node-Tutorial

## Spesifikasi VPS yang Dibutuhkan
- **CPU**: 4 Cores  
- **RAM**: 8 GB  
- **Disk**: 200 GB  
- **Bandwidth**: 10 MBit/s  
- **GPU (Opsional)**: Nvidia T4 (untuk performa AI lebih tinggi)  

## Langkah-Langkah Instalasi

### 1. Perbarui Sistem
```sh
sudo apt update && sudo apt upgrade -y
```

### 2. Pasang Dependensi
```sh
sudo apt install -y curl
```

### 3. Unduh dan Instal Gaia Node
```sh
curl -sSfL 'https://github.com/GaiaNet-AI/gaianet-node/releases/latest/download/install.sh' | bash
```

### 4. Tambahkan Path ke Lingkungan
```sh
source ~/.bashrc
```

### 5. Inisialisasi Node Gaia
```sh
gaianet init
```

### 6. Jalankan Node
```sh
gaianet start
```

### 7. Cek NodeID & DeviceID
```sh
gaianet info
```

## Setelah Node Aktif
Jika berhasil, terminal akan mencetak URL publik seperti:
```
https://0xxxxxxxxx.gaianet.xyz
```

### Langkah Selanjutnya:
1. Buka URL tersebut di browser untuk memverifikasi informasi node.
2. Di situs web, pilih:
   - **Profil > Node > Connect New Node**
3. Masukkan **NodeID** dan **DeviceID** yang diperoleh sebelumnya.
4. Verifikasi menggunakan **MetaMask**.
5. Kembali ke **Task XP** dan selesaikan proses verifikasi.

### Opsional: Mengubah Port Jika Diperlukan
Jika perlu mengubah port default (misalnya 8080), lakukan langkah berikut:
```sh
cd gaianet
nano config.json
```
Lalu cari port `8080` dan ubah ke port yang belum digunakan.

## Selesai! 🎉

Sekarang node Anda sudah aktif dan siap digunakan!
