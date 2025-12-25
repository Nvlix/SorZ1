# ⚔️ Roblox Auto Attack (Tween Fly Prone)

Script **Auto Attack Roblox** menggunakan **TweenService** dengan sistem **fly di atas mob** (menghadap ke bawah / prone) dan **auto attack terus menerus** tanpa animasi.

Karakter akan:
- Terbang ke atas mob
- Menghadap ke bawah (prone-style)
- Menyerang otomatis
- Langsung pindah ke mob berikutnya saat target mati (tanpa jeda)

---

## ✨ Fitur Utama

- 🚀 **Tween-based Movement** (smooth & stabil)
- 🛸 **Fly di atas mob** (tanpa physics fly)
- 🔄 **Auto Attack Loop** (continuous)
- 🎯 **Auto switch target** saat mob mati
- ❌ **Tanpa animasi** (pure CFrame control)
- ⚡ **Speed configurable** lewat `ATTACK_SPEED`
- 🧱 **Noclip support** (opsional)

---

## 📌 Cara Kerja

1. Script mencari target mob
2. Karakter tween ke posisi **di atas mob**
3. Karakter menghadap **ke bawah (prone)**
4. Auto attack dipanggil terus
5. Jika mob mati → lanjut ke mob berikutnya

---

## 🧩 Requirements

Pastikan script kamu memiliki:
- `LocalPlayer`
- `ATTACK_SPEED`
- `callAttackRemotes()`
- `NOCLIP_ENABLED` (opsional)
- `enableNoclip()` / `disableNoclip()` (opsional)

---

## ⚙️ Konfigurasi

```lua
ATTACK_SPEED = 50      -- Kecepatan tween (semakin besar semakin cepat)
FLY_HEIGHT = 8         -- Tinggi posisi di atas mob
