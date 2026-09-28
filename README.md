# Amigos OJT Countdown

Static site, siap deploy ke Vercel. Ada 4 halaman, dihubungkan lewat pill switcher di bagian atas:

- `index.html` — **OJT COUNTDOWN**: hitung mundur ke 14 November 2026, background `bg.jpg`.
- `time.html` — **TIME IS**: jam real-time WIB, layout sama seperti halaman 1, background `bg-time.jpg`.
- `timer.html` — **TIMER**: preset 15m/30m/45m/1j/1.5j/2j + input manual menit, background navy polos. Ikon ⛶ = fullscreen (cuma angka). Waktu habis → layar terang + bel bunyi terus sampai "Stop Bel" / Reset.
- `absen.html` — **ABSEN!**: full gambar `absen.jpg`, tanpa teks.

## Deploy
```bash
npm i -g vercel
vercel
```
Atau upload ke GitHub lalu import di vercel.com (framework preset: **Other**, tanpa build command).

## Ganti tanggal target (index.html)
```js
const target = new Date("2026-11-14T00:00:00+07:00");
```

## Ganti foto
`bg.jpg` (OJT Countdown), `bg-time.jpg` (TIME IS), `absen.jpg` (ABSEN!). Nama file harus tetap sama.
