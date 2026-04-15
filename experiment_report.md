# Experiment Report: Data Quality Impact on AI Agent

**Student ID:** AI20K-2A202600266
**Name:** Phạm Quang Hưng
**Date:** 15/04/2026

---

## 1. Ket qua thi nghiem

Chay `agent_simulation.py` voi 2 bo du lieu va ghi lai ket qua:

| Scenario | Agent Response | Accuracy (1-10) | Notes |
|----------|----------------|-----------------|-------|
| Clean Data (`processed_data.csv`) | Based on my data, the best choice is Laptop at $1200. | 10 | |
| Garbage Data (`garbage_data.csv`) | Based on my data, the best choice is Nuclear Reactor at $999999. | 1 | |

---

## 2. Phan tich & nhan xet

### Tai sao Agent tra loi sai khi dung Garbage Data?

Agent chỉ quan tâm đến giá trị dữ liệu, chứ không đảm bảo rằng dữ liệu đầu vào hợp lý. Ví dụ, agent trả về Nuclear Reactor với giá $999999 (không ai đăng bán Nuclear Reactor ngoài đời hết!).

---

## 3. Ket luan

**Quality Data > Quality Prompt?** (Dong y hay khong? Giai thich ngan gon.)

*Garbage in, garbage out.*
Nếu dữ liệu đã không chuẩn từ ban đầu, mô hình AI dù có mạnh đến mấy cũng không giảỉ quyết được được. Dữ liệu vẫn đóng vai trò lớn trong với hệ thống, một mô hình AI chỉ mạnh khi dữ liệu có chất lượng
