---
tags: [key-concept, chapter-9, security]
aliases: [Chứng chỉ số, Certificate]
---
# Digital Certificate

**Digital Certificate (chứng chỉ số)** là **bản sao hợp lệ của public key của một cá nhân/tổ chức kèm thông tin định danh, do một bên thứ ba tin cậy — Certificate Authority (CA) — cấp phát**.

## Giải thích
- Là nền tảng của **public-key infrastructure (PKI)**: xác thực rằng public key thực sự thuộc về chủ thể được ghi trong chứng chỉ.
- CA (vd Verisign/DigiCert, Let's Encrypt) ký số lên chứng chỉ; trình duyệt tin CA → tin website.
- Dùng trong [[SSL]]/TLS để mã hoá phiên giao dịch e-commerce và hiển thị HTTPS/ổ khoá — yếu tố [[Trust Signals]] quan trọng với người mua.
- Kết hợp với [[Digital Signature]] để xác thực danh tính người ký và tính toàn vẹn thông điệp trong hợp đồng điện tử.
- Thuộc nhóm "current approaches to e-commerce security" trong thiết kế bảo mật của Chaffey.

## Liên kết
- [[CH09 - Digital Experience and Service Design]]
- [[SSL]]
- [[Digital Signature]]
- [[Trust Signals]]
