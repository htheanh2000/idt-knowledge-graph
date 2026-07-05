---
tags: [key-concept, chapter-9, security]
aliases: [Chữ ký số]
---
# Digital Signature

**Digital Signature (chữ ký số)** là **phương pháp định danh cá nhân hoặc doanh nghiệp bằng mã hoá khoá công khai (public-key encryption)**.

## Giải thích
- Người gửi ký bằng **private key**; người nhận xác minh bằng **public key** tương ứng → chứng minh danh tính người ký và tính toàn vẹn của thông điệp (không bị sửa sau khi ký).
- Khác chữ ký scan/ảnh: chữ ký số gắn toán học với nội dung tài liệu, sửa 1 ký tự là chữ ký vô hiệu.
- Cần [[Digital Certificate]] do CA cấp để ràng buộc public key với danh tính thực — tạo thành hạ tầng PKI.
- Ứng dụng e-commerce: xác thực hợp đồng điện tử (authenticating contracts) — một trong 8 lĩnh vực pháp lý ở [[CH04 - Key Issues in the Digital Environment]]; ký số hoá đơn, chứng từ B2B qua [[EDI]].

## Liên kết
- [[CH09 - Digital Experience and Service Design]]
- [[Digital Certificate]]
- [[SSL]]
- [[Privacy]]
