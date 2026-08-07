# Cẩm nang CẤM "AI Slop" khi thiết kế Website / Landing Page

> Tổng hợp từ **Impeccable** (59 rule detector: 32 dấu hiệu "đậm chất AI" + 27 lỗi chất lượng) và bộ "lệnh cấm tuyệt đối" của skill.
> Mục đích: dán vào công cụ AI (Claude, GPT, v0, Lovable, Cursor...) làm quy tắc "KHÔNG được thiết kế kiểu này".

---

## 🟢 Cách dùng file này

**Cách 1 — Dán đoạn ngắn này vào đầu prompt thiết kế:**

```
Khi thiết kế UI, TUYỆT ĐỐI TRÁNH các dấu hiệu "AI slop" sau:
- KHÔNG dùng font Inter/Roboto/system default. Chọn font có cá tính, tự host.
- KHÔNG gradient tím→xanh, KHÔNG cyan-trên-nền-tối, KHÔNG nền kem "tasteful".
- KHÔNG chữ gradient. Nhấn mạnh bằng độ đậm/cỡ chữ.
- KHÔNG border màu dày một bên card (side-tab). KHÔNG glow/halo tròn phát sáng.
- KHÔNG ô icon bo góc phía trên tiêu đề (feature-card template).
- KHÔNG eyebrow/kicker (nhãn chữ hoa nhỏ) phía trên headline.
- KHÔNG card lồng card, KHÔNG mọi thứ đều là card cùng cỡ.
- KHÔNG bounce/elastic easing. KHÔNG chấm nhấp nháy, con trỏ nhấp nháy, marquee.
- KHÔNG buzzword SaaS: streamline, empower, supercharge, world-class, seamless...
- KHÔNG dùng emoji thay icon. Icon phải vẽ, cùng nét cùng weight.
- KHÔNG chữ xám trên nền màu. Tint theo màu nền.
```

**Cách 2:** Đọc phần dưới để hiểu từng loại và tự soi thiết kế của mình.

---

## 🔴 5 LỆNH CẤM TUYỆT ĐỐI (không lý do nào gỡ được)

Đây là những thứ Impeccable coi là "costume" — mặc vào cho ra vẻ, không phải thiết kế thật:

1. **Eyebrow / Kicker** — nhãn chữ HOA nhỏ, giãn ký tự, đứng ngay trên tiêu đề lớn. Tiêu đề tự đủ sức nặng → xóa nhãn đi.
2. **Chữ gradient** (gradient text) — nhấn mạnh bằng weight/size, không phải màu chuyển.
3. **Border màu dày một bên** (>1px) trên card/list/alert — dấu hiệu AI dễ nhận nhất.
4. **Đổ bóng cứng lệch** (`box-shadow: 4px 4px 0`) ngoài thế giới neobrutalist thật sự.
5. **Emoji / ký tự Unicode thay icon** — icon phải được vẽ từ thư viện thật hoặc SVG, một nét một weight thống nhất.

---

## 🎨 NHÓM 1 — Màu sắc "AI"

| Dấu hiệu | Mô tả | Rule |
|---|---|---|
| Gradient tím/violet | Gradient tím→xanh là dấu hiệu AI dễ nhận nhất | `ai-color-palette` |
| Cyan trên nền tối | Xanh cyan phát sáng trên nền đen/tối | `ai-color-palette` |
| Nền kem "tasteful" | Nền kem ấm đã thành mặc định "sang" của AI | `cream-palette` |
| Chữ gradient | Chữ tô gradient trang trí, vô nghĩa | `gradient-text` |
| Glow tối màu | Bóng đổ phát sáng màu — vẻ "cool" mặc định của AI | `dark-glow` |
| Halo tròn tỏa sáng | Vệt radial-gradient đậm giữa, mờ dần ra rìa | `radial-halo` |
| Spotlight mờ | Radial gradient màu nhấn opacity thấp làm nền | `radial-spotlight-glow` |

**Thay bằng:** Bảng màu có POV rõ ràng, lấy từ brand. Bóng đổ phải có offset + blur mềm (bóng thật), không phải halo phát sáng.

---

## 🔤 NHÓM 2 — Typography "AI"

| Dấu hiệu | Mô tả | Rule |
|---|---|---|
| Font bị lạm dụng | Inter, Roboto, Fraunces... nhàm, mất cá tính | `overused-font` |
| Serif nghiêng làm hero | Tiêu đề hero serif in nghiêng = "startup AI" điển hình | `italic-serif-display` |
| Thứ bậc chữ phẳng | Các cỡ chữ quá gần nhau, không phân cấp | `flat-type-hierarchy` |
| H1 quá khổ | Headline cả câu set cỡ display, chiếm hết màn hình | `oversized-h1` |
| Giãn ký tự âm cực đoan | Letter-spacing âm tới mức chữ mất hình dạng | `extreme-negative-tracking` |
| Giãn ký tự rộng | Tracking >0.05em trên body phá nhóm chữ tự nhiên | `wide-tracking` |
| Monospace làm màu | Dùng monospace để "ra vẻ kỹ thuật" chứ không phải cho code/data | (craft-floor) |
| Font hệ thống làm display | Impact/Arial Black/system sans làm giọng chính | (craft-floor) |

**Thay bằng:** Tự host một font có cá tính khớp brand. Body 65–75 ký tự/dòng, display tối đa ~6rem, các bước cỡ/weight rõ ràng.

---

## 🧱 NHÓM 3 — Cấu trúc & Layout "AI"

| Dấu hiệu | Mô tả | Rule |
|---|---|---|
| Ô icon bo góc trên tiêu đề | Template feature-card phổ biến nhất của AI | `icon-tile-stack` |
| Card lồng card | Card trong card tạo nhiễu, chiều sâu thừa | `nested-cards` |
| Toàn card cùng cỡ | "Icon + tiêu đề + text" lặp lại làm cấu trúc trang | (craft-floor) |
| Eyebrow chip hero | Nhãn chữ hoa nhỏ ngay trên headline khổng lồ | `hero-eyebrow-chip` |
| Kicker trên tiêu đề | Nhãn tracked uppercase/small-caps đứng riêng trên heading | `kicker-above-heading` |
| Đánh số section 01/02/03 | Nhãn số cạnh heading — "scaffolding biên tập" của AI | `numbered-section-labels` |
| Template hero-metric | Số to + nhãn nhỏ + vài stat phụ + màu nhấn | (craft-floor) |
| Spacing đều đều | Một giá trị spacing dùng khắp nơi, không nhịp điệu | `monotonous-spacing` |
| Modal thừa | Modal cho việc không cần ngắt quãng | (craft-floor) |

**Thay bằng:** Bố cục có nhịp điệu (nhóm chặt, tách thoáng, khoảng trên heading > dưới). Chỉ đánh số khi thứ tự thật sự mang thông tin.

---

## 🖼️ NHÓM 4 — Viền, bóng & nền trang trí "AI"

| Dấu hiệu | Mô tả | Rule |
|---|---|---|
| Side-tab | Viền màu dày một bên card — **tell dễ nhận nhất** | `side-tab` |
| Viền nhấn trên card bo góc | Viền dày đâm nhau với góc bo | `border-accent-on-rounded` |
| Viền mảnh + bóng rộng | Border hairline + shadow khuếch tán rộng | `gpt-thin-border-wide-shadow` |
| Nền lưới / line-field | Nền kẻ ô/lưới trang trí | `codex-grid-background` |
| Sọc gradient lặp | Repeating-gradient làm nền trang trí | `repeating-stripes-gradient` |
| Glass/blur trang trí | Kính mờ dùng làm màu chứ không cho hiệu ứng cụ thể | (craft-floor) |
| Minh họa ghép hình | SVG ghép từ hình cơ bản = clip art placeholder | `shape-assembled-illustration` |
| Sparkline/progress ring giả | Biểu đồ mini, vòng tiến trình thay cho nội dung thật | (craft-floor) |

---

## 🎬 NHÓM 5 — Chuyển động "AI"

| Dấu hiệu | Mô tả | Rule |
|---|---|---|
| Bounce/elastic easing | Cảm giác lỗi thời, sến | `bounce-easing` |
| Chấm nhấp nháy | Chấm trạng thái pulsing giả "đang sống" | `pulsing-dot` |
| Con trỏ nhấp nháy | Cursor gõ chữ giả trong hero (không có input thật) | `blinking-cursor` |
| Marquee | Nội dung tự cuộn vô tận đòi chú ý không xứng đáng | `marquee` |
| Ảnh phóng/xoay khi hover | Scale/rotate ảnh lúc hover — chữ ký UI generated | `image-hover-transform` |
| Animate width/height | Animate kích thước/padding gây giật layout | `layout-transition` |

**Thay bằng:** MỘT khoảnh khắc chuyển động có chủ đích, ease-out mũ. Vượt ra ngoài transform/opacity: blur, backdrop-filter, clip-path, mask, shadow — miễn mượt.

---

## ✍️ NHÓM 6 — Copy / Nội dung "AI"

| Dấu hiệu | Mô tả | Rule |
|---|---|---|
| Buzzword SaaS | streamline / empower / supercharge / world-class / enterprise-grade / seamless | `marketing-buzzword` |
| Lạm dụng em-dash | Rải em-dash (—) trong body là nhịp AI | `em-dash-overuse` |
| Nhịp cách ngôn | ≥3 section kết bằng câu phản đề ngắn = giọng AI, không phải giọng người | `aphoristic-cadence` |
| Chê "theater" | Gọi cái gì đó là "theater" — tic viết của AI | `theater-slop-phrase` |

**Thay bằng:** Ngôn ngữ riêng của sản phẩm. Nút gọi tên hành động; lỗi nêu vấn đề + cách khắc phục.

---

## ⚠️ LỖI CHẤT LƯỢNG THƯỜNG GẶP (không phải "AI" nhưng vẫn phải fix)

- **Tương phản thấp** — body/placeholder phải ≥4.5:1, chữ lớn ≥3:1 (`low-contrast`, `gray-on-color`)
- **Dòng quá dài** — >80 ký tự/dòng khó đọc (`line-length`)
- **Padding chật** — chữ sát mép container (`cramped-padding`, `body-text-viewport-edge`)
- **Leading chật** — line-height <1.3 (`tight-leading`)
- **Chữ quá nhỏ** — body <12px, UI text <11px (`tiny-text`, `undersized-ui-text`)
- **Chữ HOA cả đoạn dài** — khó đọc (`all-caps-body`)
- **Căn đều không ngắt từ** — khoảng cách chữ lệch (`justified-text`)
- **Nhảy cấp heading** — h1→h3 phá cấu trúc (`skipped-heading`)
- **Ảnh vỡ** — `<img>` thiếu/rỗng src (`broken-image`)
- **Chữ ẩn lúc nghỉ** — nhiều text ở opacity 0 (`content-hidden-at-rest`)
- **Chữ bị che** — text nằm dưới lớp mờ đục (`text-occlusion`)
- **Tràn container** — nội dung rộng hơn khung (`text-overflow`, `first-viewport-column-overflow`)
- **Lặp text 3+ lần** — nội dung trùng thừa (`repeated-container-text`)

---

## ✅ 8 điều NÊN làm (mặt tích cực)

1. **Brief thắng tất cả** — tôn trọng font/màu/thời kỳ đã chốt, kể cả khi trái với cảnh báo trên.
2. **Bóng đổ thật** — có offset + blur mềm, không phải halo phát sáng.
3. **Nhịp spacing** — nhóm chặt, tách thoáng, khoảng trên heading nhiều hơn dưới.
4. **Font tự host có cá tính** khớp brand, không dùng font mặc định.
5. **Icon vẽ thật** — cùng nét, cùng weight; không emoji.
6. **Đủ trạng thái** — hover, disabled, loading, error, empty + responsive + focus bàn phím.
7. **Màu có POV** — bảng màu lấy từ brand, không mặc định tím/cyan.
8. **Sáng/tối theo bối cảnh dùng** (ai, ở đâu, ánh sáng nào), không theo thói quen category.

---

## 🛠️ Kiểm tra tự động (bonus)

Impeccable có CLI quét 59 lỗi này **không cần AI, không cần API key**:

```bash
npx impeccable detect index.html          # quét 1 file
npx impeccable detect src/                # quét cả thư mục
npx impeccable detect https://example.com # quét 1 URL đang chạy
npx impeccable detect --json .            # xuất JSON cho CI
```

Hoặc trong Claude Code: `/impeccable audit` (kỹ thuật) và `/impeccable critique` (thẩm mỹ/UX).

---

*Nguồn: [Impeccable](https://impeccable.style) — Apache 2.0, tác giả Paul Bakaus. Tổng hợp cho mục đích nội bộ Leandigi.*
