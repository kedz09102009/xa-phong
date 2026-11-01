# Báo cáo thực hành xà phòng handmade — Slidev Kawaii

Dự án vẫn sử dụng Slidev, không chuyển sang HTML độc lập.

## Chạy trên Windows PowerShell

```powershell
npm.cmd run dev
```

## Rà soát bố cục

- Chuẩn hóa `box-sizing: border-box` cho toàn bộ phần tử bên trong slide để padding và border không làm tăng kích thước ngoài dự kiến.
- Thu gọn slide 06 (Vì sao xà phòng có thể làm sạch?): khung phân tử, SVG, ba thẻ giải thích và kết luận được bố trí lại để giảm nguy cơ tràn cạnh dưới.
- Vẽ lại sơ đồ SVG: gốc hydrocarbon `R`, nhóm carboxylate `C(=O)O⁻` và ion đối `Na⁺` được thể hiện rõ ràng.
- Rà lại khoảng trống cho các slide mục tiêu, nguyên liệu, lý thuyết, quy trình, quan sát ảnh, đánh giá, rút kinh nghiệm và kết thúc.
- Bỏ cache npm khỏi GitHub Actions vì dự án không kèm `package-lock.json`.

## 5 vị trí ảnh thực nghiệm

1. Nguyên liệu và dụng cụ — slide 04.
2. Quá trình thực hành — slide 07.
3. Hỗn hợp sau khi nhũ hóa — slide 08.
4. Xà phòng sau khi tạo hình — slide 08.
5. Thành phẩm hoàn chỉnh — slide 08.

Các vị trí trên hiện là khung chờ để thay bằng ảnh thật của nhóm.

## Kiểm tra đã thực hiện

- Frontmatter YAML: có cặp phân cách mở/đóng.
- Số slide: 11; tổng số dòng phân cách là 12 (2 dòng frontmatter + 10 dòng ngăn cách slide).
- 11 slide có một root `.k-slide` và một tiêu đề chính.
- Các đường dẫn sticker trong Markdown đều tồn tại.
- Đủ 5 khung ảnh thực nghiệm.
- CSS phân tích không có lỗi cú pháp; SVG hợp lệ XML; ZIP đã kiểm tra toàn vẹn.

**Giới hạn kiểm thử:** cài đặt npm trong môi trường đóng gói bị hết thời gian, vì vậy chưa chạy được `slidev build` hoặc kiểm tra end-to-end trên trình duyệt. Các kết quả trên là kiểm tra tĩnh, không phải xác nhận bản dựng trực tiếp.
