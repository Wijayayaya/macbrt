# 🔐 macbrt — MAC Address Brute Force Tool for Winbox (Bash Script)

**macbrt** adalah tools brute-force sederhana yang dirancang untuk menargetkan login **Winbox MikroTik** menggunakan **MAC Address**. Tools ini dibuat dengan bahasa **Bash** sebagai bagian dari pembelajaran di bootcamp Cyber Security.

> ⚠️ **DISCLAIMER**: Tools ini dibuat **hanya untuk tujuan edukasi**. Dilarang menggunakan tools ini untuk menyerang perangkat atau sistem tanpa izin. Tindakan tersebut melanggar hukum.

---

## 🚀 Fitur

- Brute force kombinasi **username** dan **password**
- Input **MAC address** interaktif saat dijalankan
- Membaca daftar `user.txt` dan `pass.txt`
- Menampilkan hanya kombinasi yang berhasil
- Pesan khusus jika tidak ditemukan kombinasi yang benar
- 100% Bash tanpa dependensi eksternal

---

## 📁 Struktur File

├── macbrt <br>
├── user.txt <br>
└── pass.txt

---

## 📥 Contoh Isi File

**user.txt**
<br>admin
<br>user
<br>test

**pass.txt**
<br>admin
<br>1234
<br>toor

---

## ⚙️ Cara Menjalankan

1. Jadikan file `macbrt` executable:

   ```bash
   chmod +x macbrt
   ```

2. Jalankan:

   ```bash
   ./macbrt
   ```

3. Masukkan MAC Address saat diminta:
   ```bash
   Masukkan MAC Address target: 1A:2B:3C:AA:BB:CC
   ```

## 💡 Contoh Output

**Jika berhasil:**

```bash
[*] Starting MAC brute-force on 1A:2B:3C:AA:BB:CC...
[*] Trying...
[+] SUCCESS! Username: admin | Password: 1234
```

**Jika Gagal**

```bash
[*] Starting MAC brute-force on 4C:5E:0C:AA:BB:CC...
[*] Trying...
[!] Failed! Username and Password not found.
```
