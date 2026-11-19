# Daily GitHub Activity

Repository ini memperbarui `activity.txt` secara otomatis setiap hari menggunakan GitHub Actions.

## Setup

1. Buat repository GitHub bernama `daily-github-activity`.
2. Upload seluruh isi folder ini ke branch default (biasanya `main`).
3. Buka **Settings → Secrets and variables → Actions → New repository secret**.
4. Buat secret bernama `GH_USER_EMAIL`, isi dengan alamat email yang sudah terverifikasi di akun GitHub kamu.
5. Buka tab **Actions**, lalu izinkan Actions jika diminta.
6. Workflow berjalan setiap hari sekitar pukul 08.00 WIB. Kamu juga bisa menjalankannya manual melalui **Actions → Daily Activity → Run workflow**.

## Catatan

- GitHub Actions terjadwal dapat berjalan terlambat beberapa menit atau lebih.
- Kontribusi hanya akan muncul jika commit memenuhi aturan GitHub Contributions, termasuk email commit yang terhubung ke akunmu dan repository berada dalam kondisi yang memenuhi syarat.
- Workflow menggunakan `GITHUB_TOKEN` bawaan; tidak perlu membuat Personal Access Token.
