# Repotin Companion — GitHub Pages Deploy Guide

Web App Mobile & Desktop untuk Admin Repot.in (Generate Kunci Aktivasi & Monitoring Perangkat Supabase).

---

## 🚀 Mengapa GitHub Pages?
- **Zero-Blocker**: Tidak dibungkus sandbox iframe Google, sehingga bebas dari isu blokir pihak ketiga (*Third-Party Cookies*) pada Safari iOS dan Chrome Android.
- **Direct HTTPS**: Langsung terhubung ke Supabase REST API dengan latensi rendah melalui global CDN.
- **Universal**: Dapat diakses langsung dari HP (Android/iPhone), tablet, maupun PC manapun.

---

## 📌 Cara Deploy Cepat (Paling Mudah via GitHub Web - 2 Menit)

1. **Buka GitHub** dan buat repository baru:
   - Nama repo: `repotin-companion` (atau sesuai keinginan).
   - Visibility: **Public** (atau **Private** jika akun Anda mendukung GitHub Pages pada repo private).
   - Jangan centang "Add a README file" jika ingin upload langsung.
   - Klik **Create repository**.

2. **Upload File**:
   - Pada halaman repository yang baru dibuat, klik link **"uploading an existing file"**.
   - Tarik (drag & drop) 2 file dari folder ini:
     - `index.html`
     - `.nojekyll`
   - Klik **Commit changes**.

3. **Aktifkan GitHub Pages**:
   - Masuk ke tab **Settings** di repo Anda.
   - Di menu sebelah kiri, klik **Pages** (di bawah bagian "Code and automation").
   - Pada bagian **Build and deployment** -> **Branch**:
     - Pilih branch: **`main`**
     - Pilih folder: **`/ (root)`**
     - Klik tombol **Save**.

4. **Selesai!**:
   - Tunggu sekitar 30–60 detik hingga GitHub selesai mem-publish.
   - Refresh halaman **Settings -> Pages**.
   - Link Web App Anda akan muncul di bagian atas:
     👉 `https://<username-github>.github.io/repotin-companion/`
   - Buka link tersebut di browser HP atau simpan ke layar utama (*Add to Home Screen*) sebagai PWA.

---

## 💻 Cara Deploy via Git Terminal / Command Prompt

Jika Anda memiliki `git` di komputer:

```bash
cd repotin-companion
git init
git add .
git commit -m "Deploy Repotin Companion to GitHub Pages"
git branch -M main
git remote add origin https://github.com/<username-github>/repotin-companion.git
git push -u origin main --force
```

Setelah itu, aktifkan GitHub Pages di **Settings -> Pages** (Branch: `main`, Folder: `/ (root)`).

