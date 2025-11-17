Mini SOC Investigation Case

1. Summary

Trong quá trình phân tích log Windows Security trên Splunk SIEM, em phát hiện một số sự kiện 4625 (Failed Logon).
Các đăng nhập thất bại xuất hiện từ user guest và hung.
Dựa vào LogonType và Workstation, em đánh giá đây không phải brute force (chỉ xảy ra 1 lần mỗi user), mức độ sự cố thấp.
Tuy nhiên, EventID 4625 là nguồn quan trọng để SOC Analyst phát hiện tấn công dò mật khẩu (password guessing, brute force RDP).

2. Event Details
   | Trường | Giá trị |
   | ------------------------- | ---------------------------------- |
   | **EventID** | 4625 |
   | **Ý nghĩa** | Failed Logon |
   | **User bị ảnh hưởng** | guest, hung |
   | **Workstation** | DESKTOP-01, WIN-RDP01 |
   | **LogonType** | guest: 3 (Network), hung: 10 (RDP) |
   | **Số lần thất bại** | guest: 1, hung: 1 |
   | **Severity (SOC Tier 1)** | Low |
   | **Kết luận** | Không phải brute force |

3. SOC Analysis
   🔹 Vì sao không phải brute force?

- Không có sự lặp lại nhiều lần
- Không có pattern liên tục theo thời gian
- Mỗi user chỉ fail đúng 1 lần
- Không có tăng đột biến sự kiện
- Không có 4624 (logon thành công) sau chuỗi 4625
  🔹 LogonType quan trọng

- LogonType 3 → network login (ít nghi ngờ)
- LogonType 10 → RDP login (nguy cơ cao hơn)
  -> Nhưng vẫn chỉ 1 lần duy nhất.
