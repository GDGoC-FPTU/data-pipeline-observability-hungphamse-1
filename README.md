[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=23574259&assignment_repo_type=AssignmentRepo)
# Day 10 Lab: Data Pipeline & Data Observability

**Student Email:** 26ai.hungpq@vinuni.eddu.vn
**Name:** Phạm Quang Hưng

---

## Mo ta

Bài Lab này mô phỏng quy trình ETL từ trích xuất -> xử lý -> sử dụng cho model AI

---

## Cach chay (How to Run)

### Prerequisites
Trước khi bắt đầu, bạn nên tạo môi trường ảo để quản lý các thư viện:

1. **Khởi tạo và kích hoạt Virtual Environment (venv):**
   - **Trên Windows:**
     ```powershell
     python -m venv venv
     .\venv\Scripts\activate
     ```
   - **Trên macOS/Linux:**
     ```bash
     python3 -m venv venv
     source venv/bin/activate
     ```

2. **Cài đặt thư viện cần thiết:**
   ```bash
   pip install pandas pytest
   ```

### Chay ETL Pipeline
```bash
python solution.py
```

### Chay Agent Simulation (Stress Test)
```bash
python agent_simulation.py
```

---

## Cau truc thu muc

```readme
├── agent_simulation.py      # Agent simulation / stress test
├── experiment_report.md     # Báo cáo thí nghiệm
├── generate_garbage.py      # Script tạo dữ liệu giả
├── garbage_data.csv         # Dữ liệu rác (generated)
├── raw_data.json            # Dữ liệu thô đầu vào
├── processed_data.csv       # Output của pipeline
├── solution.py              # ETL pipeline script
├── README.md                # Tệp hướng dẫn này
└── tests/
    └── test_autograder.py     # Test autograder
```

---

## Ket qua

Trong 6 record ở `raw_data.json`, có 4 record là "sạch", còn lại 2 record là "bẩn" và đã bị loại
