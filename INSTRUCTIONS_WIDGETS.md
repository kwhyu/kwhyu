# ⚙️ Panduan Mengaktifkan Widget Tambahan

Saya telah memasangkan widget **WakaTime** (statistik coding) dan **3D City** (animasi kontribusi). Agar semuanya bekerja, ada beberapa hal yang harus Anda "nyalakan" karena ini membutuhkan data pribadi Anda.

## 1. 🧱 Mengaktifkan 3D Contribution City
Widget ini akan membuat tampilan kota isometrik dari kontribusi Anda. Bagian ini **sudah siap** dan akan otomatis muncul besok pagi (jadwal otomatis). Tapi jika Anda ingin memunculkannya SEKARANG:

1. Buka tab **Actions** di GitHub Anda.
2. Cari workflow bernama **GitHub-Profile-3D-Contrib**.
3. Klik **Run workflow**.
4. Tunggu sampai selesai (hijau).
5. Refresh profil Anda, dan kotanya akan muncul di bawah Stats.

---

## 2. ⏳ Mengaktifkan WakaTime (Statistik Coding)
Ini adalah widget yang paling keren karena bisa melacak berapa jam Anda coding per minggu.
**Langkah-langkah:**

1. **Daftar/Login ke WakaTime**: Buka [https://wakatime.com/](https://wakatime.com/) dan login dengan GitHub.
2. **Dapatkan API Key**: Masuk ke [https://wakatime.com/settings/api-key](https://wakatime.com/settings/api-key), lalu copy "Secret Agent Key" Anda.
3. **Masukkan ke GitHub Secrets**:
   - Buka Repo Anda > **Settings**.
   - Menu kiri > **Secrets and variables** > **Actions**.
   - Klik **New repository secret**.
   - **Name**: `WAKATIME_API_KEY` (harus persis sama).
   - **Secret**: (Paste API Key dari WakaTime tadi).
   - Klik **Add secret**.
4. **Jalankan Workflow**:
   - Pergi ke tab **Actions**.
   - Klik **Waka Readme**.
   - Klik **Run workflow**.

Jika berhasil, bagian "Weekly Coding Status" di profil Anda akan terisi dengan grafik batang coding habit Anda!

---
*Catatan: Jika Anda tidak ingin menggunakan WakaTime, Anda bisa menghapus bagian <!--START_SECTION:waka--> di file README.md.*
