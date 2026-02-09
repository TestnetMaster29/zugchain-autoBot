# Bot Tự Động Hóa Mạnh Mẽ Cho Hệ Sinh Thái ZugChain Airdrop

Một bot tự động hóa nâng cao dành cho hệ sinh thái ZugChain Airdrop, hỗ trợ đăng nhập tự động, điểm danh hằng ngày và hoàn thành nhiệm vụ đã được xác minh.

---

## 📋 Mục lục
- [Tính năng](#-tính-năng)
- [Yêu cầu](#-yêu-cầu)
- [Cài đặt (Hướng dẫn Setup)](#-cài-đặt-hướng-dẫn-setup)
- [Cấu hình (Thiết lập)](#-cấu-hình-thiết-lập)
- [Cách chạy](#-cách-chạy)

## ✨ Tính năng

| Tính năng | Mô tả | Trạng thái |
| :--- | :--- | :--- |
| **Đăng nhập tự động** | Đăng nhập bằng chữ ký ví an toàn (chuẩn Metamask) | ✅ |
| **Lập lịch thời gian** | Tự động chạy mỗi ngày lúc 00:00 UTC | ✅ |
| **Điểm danh hằng ngày** | Tự động nhận phần thưởng hằng ngày | ✅ |
| **Faucet** | Tự động claim faucet & giải captcha | ✅ |
| **Staking** | Tự động stake ZUG để nhận thêm điểm | ✅ |
| **Xác minh thông minh** | Cơ chế xác minh nhiệm vụ on-chain | ✅ |
| **Chế độ ẩn danh** | Xoay User-Agent thực tế & mô phỏng hành vi người dùng | ✅ |
| **Nhiều tài khoản** | Hỗ trợ không giới hạn số lượng tài khoản | ✅ |
| **Sipal Logging** | Log console rõ ràng, gọn gàng và dễ theo dõi | ✅ |

## 🛠 Yêu cầu

Trước khi bắt đầu, hãy đảm bảo bạn đã cài đặt các công cụ sau:

1. **Node.js** – Bắt buộc. Tải tại [nodejs.org](https://nodejs.org/) và chọn **phiên bản LTS (v18 trở lên)**.
2. **Git** – Bắt buộc. Tải tại [git-scm.com](https://git-scm.com/downloads).
3. **API Key 2Captcha** – Bắt buộc để giải captcha khi claim faucet (tài khoản phải có số dư).

## 📦 Cài đặt (Hướng dẫn Setup)

Thực hiện lần lượt các bước sau (phù hợp cho người mới):

### 1. Tải Bot
Mở Terminal (Command Prompt hoặc PowerShell) và chạy:

```bash
git https://github.com/TestnetMaster29/zugchain-autoBot
cd zugchain-autoBot
```

### 2. Cài đặt thư viện
Trong cùng cửa sổ terminal, chạy:

```bash
npm install
```

*Vui lòng đợi quá trình cài đặt hoàn tất. Có thể mất vài phút.*

## ⚙️ Cấu hình (Thiết lập)

### 1. Tạo file tài khoản (`accounts.json`)

Bạn cần tạo file để lưu thông tin tài khoản:

1. Tìm file `accounts_tmp.json` trong thư mục bot.
2. Đổi tên file thành `accounts.json`.
3. Mở file bằng Notepad hoặc bất kỳ trình soạn thảo văn bản nào.
4. Điền thông tin theo mẫu sau:

```json
{
  "twoCaptchaApiKey": "YOUR_2CAPTCHA_API_KEY",
  "accounts": [
    {
      "name": "Account 1",
      "privateKey": "YOUR_METAMASK_PRIVATE_KEY",
      "proxy": "http://user:pass@ip:port"
    }
  ]
}
```

> **Lưu ý:**
> - `privateKey`: Private key của ví Metamask (**tuyệt đối không chia sẻ!**).
> - `proxy`: Không bắt buộc. Có thể để trống nếu không dùng proxy.
> - `twoCaptchaApiKey`: Bắt buộc để vượt captcha khi claim faucet.

### 2. Cấu hình chung (`config.json`)

File `config.json` đã được cấu hình sẵn.

Bạn **không cần chỉnh sửa** trừ khi có thông báo cập nhật từ SipalDrop.

## 🚀 Cách chạy

Sau khi hoàn tất cài đặt và cấu hình, chạy bot bằng lệnh:

```bash
npm start
```

CHÚC BẠN FARM AIRDROP THÀNH CÔNG 🚀🔥

