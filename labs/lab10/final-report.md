# 🏦 ATM Mini Project – Final Report

## 1. Giới thiệu
Dự án này được phát triển trong môn **Nhập môn Công nghệ Phần mềm**, với mục tiêu xây dựng một hệ thống ATM mô phỏng.  
Các chức năng chính:  
- Đăng nhập (Login)  
- Rút tiền (Withdraw)  
- Kiểm tra số dư  
- Đăng xuất  

Quá trình phát triển được chia thành 10 lab: từ phân tích yêu cầu, thiết kế UML, xây dựng database, code module, kiểm thử và quản lý tiến độ bằng Jira.

---

## 2. Artifacts Tổng Hợp
- **Lab 02 – Use Case Diagram** → [link](../lab02-uc/)  
- **Lab 03 – Sequence Diagram** → [link](../lab03-sequence/)  
- **Lab 04 – Form Login** → [link](../lab04-form-login/)  
- **Lab 05 – ERD + Database** → [link](../lab05-erd/)  
- **Lab 06 – Class Diagram** → [link](../lab06-class/)  
- **Lab 07 – Withdraw Module** → [link](../lab07-withdraw/)  
- **Lab 08 – Unit Test & Integration Test** → [link](../lab08-test/)  
- **Lab 09 – Jira Report** → [link](../lab09-jira/)  

(Ảnh UML, ERD, test screenshot có thể đặt trong thư mục `/labs/lab10/artifacts/`)

---

## 3. UML Models
Hệ thống ATM gồm các actor: **User**, **ATM System**, với các ca sử dụng chính:  
- Đăng nhập  
- Rút tiền  
- Kiểm tra số dư  

👉 (Chèn hình Use Case, Sequence, Class Diagram tại đây)

---

## 4. Database & Code Minh Hoạ
- Cấu trúc bảng chính: **User, Account, Transaction**  
- Ví dụ code kết nối DB + chức năng `withdraw`  

```sql
CREATE TABLE Account (
    account_id INT PRIMARY KEY,
    user_id INT,
    balance DECIMAL(12,2)
);
