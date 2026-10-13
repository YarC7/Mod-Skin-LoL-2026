# 🎮 Mod Skin LoL

Ứng dụng desktop giúp áp Mod Skin cho Liên Minh Huyền Thoại chỉ với một click.

## ✨ Điểm nổi bật

- **Áp skin 1 click** — chọn tướng, chọn skin, bấm Apply là chơi.
- **2 chế độ:**
  - *LTK Manager* — đưa mod vào thư viện LTK, mở LTK bấm Start (ổn định, quen thuộc).
  - *Auto (engine)* — tự dựng overlay + chạy patcher, **không cần mở LTK** (cần `ltk_patcher_host.exe` + dll từ bản cài LTK).
- **Kho skin online** — hơn 9,000 skin & chroma tải khi cần qua CDN, máy nhẹ, luôn mới.
- **Tìm kiếm song ngữ** Việt – Anh, lọc theo lane và hệ, xem trước chroma.

## 🚀 Bắt đầu

1. Tải bản mới nhất ở mục [Releases](../../releases), mở app.
2. Mode *LTK Manager*: cài thêm [LTK Manager](https://github.com/LeagueToolkit/ltk-manager/releases/latest). Mode *Auto*: chỉ cần 2 file patcher của LTK.
3. Chọn tướng → chọn skin → **Apply**.
   - LTK Manager: mở LTK bấm **Start** rồi vào game.
   - Auto: mở game từ Client và vào trận thẳng.
4. Đổi skin có hiệu lực từ **trận sau** (giới hạn của engine game, tool nào cũng vậy).

## 🧱 Công nghệ

Electron + React + TypeScript · LTK patcher · mod-tools (cslol-manager, GPL-3.0 — xem `tools/README.md`) · Cloudflare R2 CDN · Riot DDragon

Skin assets: [Rose / LeagueSkins](https://github.com/Alban1911/LeagueSkins)

## ⚖️ Disclaimer

Không liên kết với Riot Games. Dùng mod skin có rủi ro theo chính sách nhà phát hành — bạn tự chịu trách nhiệm.

---
*Phát triển bởi [YarC7](https://github.com/YarC7)*

![Downloads](https://img.shields.io/github/downloads/YarC7/Mod-Skin-LoL-2026/total)
