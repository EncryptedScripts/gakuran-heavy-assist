# Encrypted Scripts — Gakuran

Script combat all-in-one buat **Gakuran** (Roblox): counter assist Wing Chun, auto parry, reach, lock target, HUD & nameplate musuh gaya RPG, animation changer & emote yang **keliatan pemain lain**, teleport, basket always green, autoplay alat musik, exploiter scanner, plus sistem config — dengan menu sidebar (switch, slider, kotak cari).

## Cara pakai

Paste ke executor lu (Potassium / executor lain yang support `getgenv`, `writefile`, `getloadedmodules`, `VirtualInputManager`):

```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/EncryptedScripts/gakuran-heavy-assist/main/GakuranHeavyAssist.lua"))()
```

Execute ulang = versi lama otomatis di-unload dulu (setting lu kebawa).

## Keybind default

| Tombol | Fungsi |
|---|---|
| `RightShift` | Munculin / sembunyiin menu |
| `J` / `K` / `L` | Mode counter Wing Chun: Normal Attack Only / All Attack / Heavy Attack Only |
| `U` | Auto parry on / off |
| `Y` | Face target on / off |
| `Z` | Lock ke musuh terdekat / unlock |
| `P` | Auto parry hub Interium on / off |

Reach & 4 slot emote belum ada tombol default — set sendiri di tab **Keybind** (atau tab **Emote**). Satu tombol cuma buat satu fungsi, `Backspace` = kosongin.

## Fitur

**Assist (counter Wing Chun)**
- Counter heavy (R) otomatis pas pukulan musuh mau kena — timing dihitung pake rumus game (tinggi badan, style, combo, ping lu).
- 3 mode: pukulan biasa aja / semua / heavy aja. Slider kepastian kena, penyesuaian jangkauan, jangkauan dinamis (ikut gerak musuh), lingkaran jangkauan di tanah.
- **M1 Guard** — auto swing lu ditahan pas counter / parry mau jalan (biar R / block gak ketolak). **Prioritas Counter**, **Fix R nyangkut**, pause auto parry hub lain pas counter siap.

**Combat**
- **Auto Parry** — preset Full Parry / Pro / Like Human / Santai / Custom, rotation cone, timing, tahan block, parry heavy.
  - Koreksi timing otomatis (belajar dari hasil parry lu sendiri), cadangan detik terakhir (block pas hitbox udah nyentuh), auto equip (T) kalau belum combat stance.
  - Anti reach: pemain yang ketauan pake reach tetep di-parry walau posisinya jauh.
  - Lawan nge-spam: block ditahan kalau gak sempet perfect lagi (kecuali stamina mepet).
- **Face Target** — badan (+ kamera) ngadep penyerang, ada smoothing.
- **No Slowdown / No Stun Slow / No Delay** — gak dipelanin pas nyerang / kena stun, swing M1 nyambung tanpa jeda.
- **Reach** — pukulan nyampe dari jauh, **di layar lu badan tetep diem**.
  - Target: **Nearest**, **Player pilihan** (daftar pemain + cari), atau **Aim** (paling deket kursor).
  - Jarak bisa diketik bebas atau **Unlimited**. Prediksi gerak musuh (ping + delay posisi) biar tetep kena pas musuh lari.
  - **Mode cepet** — di layar orang lain lu keliatan di samping target sesingkat mungkin.
  - Highlight target + penanda jarak di atas kepala (merah kalau lewat batas).
- **Lock Target** — lock ke terdekat atau pilih pemain, kamera & badan ngadep target.

**Visual**
- HUD sendiri (HP, stamina asli, cooldown heavy) & nameplate musuh pake **nama Gakuran** mereka (HP, perkiraan stamina, cooldown heavy) — cuma pemain di sekitar, ringan.
- Tanda hasil exploiter scanner di nameplate, sembunyiin tulisan "IN COMBAT" game.

**Anim** — semua keliatan pemain lain
- Animation changer per gerakan: M1 1–4, heavy, idle & jalan combat, block — pake animasi style lain. Set lengkap dari 1 style & preset mix.
- Animasi pas perfect parry.
- Gerak di luar combat: idle, jalan, lari, lompat, jatuh, mendarat, dash — pake animasi Gakuran (stance / jalan style lain, pose, dance) atau **animation pack marketplace**.
- Kotak cari di tiap daftar. Daftar style & animasi dibaca langsung dari game (update game = otomatis muncul).
- Cuma visual: timing, jangkauan & damage tetep style asli lu.

**Emote** — semua keliatan pemain lain
- 4 slot emote + keybind, **emote di mana aja** (combat stance, di udara, abis mukul). **Backflip** = efek VFX-nya muncul di layar semua orang.
- Daftar semua emote Gakuran (klik = main) + kotak cari.
- **Marketplace Roblox**: cari emote & animation pack live (urut relevan / populer / terbaru / terlaris) atau tempel ID / link, terus pasang ke slot, taunt, AFK, parry, idle / jalan / lari / lompat.
- **Auto taunt** abis musuh yang lu pukul KO, **pose AFK** pas lu diem.

**World**
- Teleport ke area & ruangan (mendarat di lantainya, termasuk area yang "disegel" game).
- Basket **always green** (+ persen sengaja meleset biar natural).
- Autoplay alat musik rhythm (+ persen PERFECT).

**Scan** — exploiter scanner
- Tombol scan (5 detik): speed, fly, noclip, teleport, high jump, walkspeed, lari tanpa izin, no slowdown / no stun, animation changer, dll.
- Statistik pasif: auto parry / auto counter (persentase & konsistensi timing), reach, stamina tanpa abis.

**Config**
- Save pakai nama, load, delete, **autoload** config pilihan tiap script dijalanin.
- Setting sesi terakhir otomatis kesimpen tiap 5 detik — tetep ada walau rejoin / game crash.
- Disimpen di folder executor: `EncryptedHeavyAssist/`.

## Catatan

- Damage, block, stamina & safe zone tetep diputusin server — script gak bisa bikin kebal.
- Reach: di layar pemain lain lu keliatan pindah ke samping target sebentar pas mukul.
- Animasi / emote marketplace cuma keliatan orang lain kalau asset-nya boleh dipake publik (animation pack & emote yang dijual di marketplace).
- Pakai dengan risiko sendiri.
