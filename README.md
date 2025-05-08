# 🛒 Discord Marketplace Bot

Bot Discord untuk marketplace dengan sistem pembayaran otomatis via **QRIS** (Xendit). Dibuat menggunakan Node.js dan Discord.js.


## 🚀 Fitur

- 💬 Perintah `!marketplace` untuk melihat daftar item
- 🛍️ Beli item dengan `!buy <item>`
- 📸 QRIS dibangkitkan otomatis (OVO, DANA, Gopay)
- 🔔 Bot mendeteksi pembayaran otomatis via webhook
- 📦 Produk dikirim otomatis via DM

## 📦 Struktur Project

```
.
├── index.js         # Main bot logic
├── keep_alive.js    # Keep-alive server (Replit)
├── package.json     # Dependencies
└── README.md        # Dokumentasi
```

## 🛠️ Cara Setup

1. Ganti `YOUR_DISCORD_BOT_TOKEN` dan `YOUR_XENDIT_API_KEY` di `index.js`
2. Deploy ke [Replit](https://replit.com) atau [Render](https://render.com)
3. Pastikan `callback_url` QRIS mengarah ke `/webhook` endpoint

## 🖼️ Demo Tampilan

```
!marketplace
🛒 Daftar item:
- Item1 - 1000 Coins
- Item2 - 2000 Coins

!buy item1
📲 Scan QR untuk bayar:
https://qr-code.xendit.co/...
```

## 🔐 Tips Keamanan

- Gunakan HTTPS untuk webhook
- Validasi signature dari Xendit (jika tersedia)
- Simpan data pembayaran ke database (opsional)

---

> Dibuat dengan ❤️ oleh Developer Bot Marketplace
