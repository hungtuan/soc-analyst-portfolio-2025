# Playbook: Windows Failed Logon (EventID 4625)

## 1. Xác định sự kiện

- EventID = 4625
- Kiểu đăng nhập (LogonType)
- Tài khoản bị ảnh hưởng (AccountName)

## 2. Kiểm tra nguồn đăng nhập

- Workstation
- IP / Machine name
- LogonType 10 = RDP (nghi hơn)

## 3. Phân tích số lượng đăng nhập thất bại

- > 5 lần / 5 phút = nghi ngờ brute force

## 4. Tìm sự kiện 4624 tiếp theo

- Nếu có login thành công sau 4625 → nghi compromise

## 5. Tạo ticket hoặc escalate

- Low / Medium / High theo số lần và nguồn
