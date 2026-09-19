# ⚡ Analog IC Design Roadmap & Study Guide

Repository lưu trữ lộ trình học tập, cẩm nang nghiên cứu và tài liệu thực hành thiết kế vi mạch tương tự (**Analog / Mixed-Signal IC Design**), hướng tới mục tiêu xin học bổng và gia nhập Lab Vi mạch tại các trường Đại học hàng đầu Đài Loan (NYCU, NCKU, NTUST, NCHU,...).

---

## 📌 Nội dung chính trong Repository

| Tài liệu | Mô tả chi tiết |
| :--- | :--- |
| 📋 [taiwan_analog_lab_roadmap_checklist.md](./taiwan_analog_lab_roadmap_checklist.md) | **Lộ trình toàn diện & Checklist chi tiết:** Chiến lược hồ sơ, thời khóa biểu thực tế, danh sách Lab mục tiêu, các mốc thời gian và kế hoạch săn học bổng INTENSE. |
| 📖 [razavi_analog_study_guide.md](./razavi_analog_study_guide.md) | **Cẩm nang học 80/20 giáo trình GS. Behzad Razavi:** Bản đồ chương (đọc gì, bỏ gì), lộ trình 4 chặng bám sát chuỗi bài giảng *Electronics 1 & 2* và sách *Design of Analog CMOS Integrated Circuits*. |

---

## 🎯 Dự án mục tiêu (Core Portfolio)
* **Two-Stage Miller CMOS Operational Amplifier**
  * Tầng 1: Cặp vi sai (Differential Pair) có tải gương dòng tích cực (Active Current Mirror Load).
  * Tầng 2: Tầng Common-Source có tải nguồn dòng (Current Source Load).
  * Mạch bù tần số: Tụ bù Miller $C_c$ và điện trở triệt RHP zero $R_z$ (Pole splitting).
  * Kiểm chứng nâng cao: Mô phỏng PVT (Process Corners SS/TT/FF, Điện áp $\pm 10\%$, Nhiệt độ $-40^\circ\text{C} \to 125^\circ\text{C}$).

---

## 🛠️ Công cụ & Nền tảng
* **Lý thuyết:** Sách & Bài giảng GS. Behzad Razavi (UCLA).
* **EDA Tools:** Synopsys Custom Compiler, HSPICE / PrimeSim, Custom WaveView.
* **Tiến trình:** Synopsys EDA Lab / SkyWater 130nm PDK.
