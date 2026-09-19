# 🚀 LỘ TRÌNH & CHECKLIST CHINH PHỤC LAB ANALOG IC DESIGN ĐÀI LOAN

> **Hồ sơ ứng viên:**
> * **Học vấn:** Kỹ sư Cơ điện tử – Đại học Bách Khoa Hà Nội (CPA: 2.8/4.0)
> * **Kinh nghiệm:** 4 năm Java Backend Developer (Tư duy logic, thuật toán, kỷ luật công sở)
> * **Đã tích lũy:** FPT Jetking (Verilog, Basys 3 FPGA), ICTC Physical Design
> * **Ngoại ngữ:** Đang học tiếng Trung Phồn thể (Mục tiêu: Đạt TOCFL A2 vào Tháng 7/2027 sau khóa 250h) + Tiếng Anh kỹ thuật
> * **Chiến lược:** Săn **Học bổng INTENSE Bán dẫn toàn phần** (hoặc Tự túc kinh phí), dùng **Portfolio Dự án Analog thực tế + Chứng chỉ Synopsys PSTC** để vượt qua rào cản CPA.

---

## 🎯 MỤC TIÊU CUỐI CÙNG (THE NORTH STAR)
* Nhận được **Letter of Acceptance** và **Học bổng INTENSE toàn phần** vào một **Lab Analog / Mixed-Signal IC Design** tại các trường đại học hàng đầu Đài Loan (NYCU, NTUST, NCKU, NCHU, CCU, NSYSU).
* Kỳ nhập học mục tiêu: **KỲ THU (THÁNG 9/2028)** — Đảm bảo thời gian chuẩn bị vững chắc, không bị vội vã, tích lũy tối đa tài chính và kỹ năng thực chiến.

---

## GIAI ĐOẠN 1: NỀN TẢNG LÝ THUYẾT CỐT LÕI (2 THÁNG)
*Tài liệu chính: Sách & Chuỗi bài giảng YouTube của **GS. Behzad Razavi** (Design of Analog CMOS Integrated Circuits).*
* 📺 **Kênh YouTube chính thức của Thầy Razavi:** [Behzad Razavi (@b_razavi)](https://www.youtube.com/@b_razavi)
* 🔗 **Playlist Electronics 1 (MOSFET, CS/CD/CG, Small-Signal):** [Razavi Electronics 1 Playlist (YouTube)](https://www.youtube.com/playlist?list=PLyYrySVqmyVPzvVlPW-TTzHhNWg1J_0LU)
* 🔗 **Playlist Electronics 2 (Vi sai, Đáp ứng tần số, Hồi tiếp, Op-Amp):** [Razavi Electronics 2 Playlist (YouTube)](https://www.youtube.com/results?search_query=Razavi+Electronics+2+playlist)
* 📚 **2 cuốn sách kinh điển cần có:**
  1. *Fundamentals of Microelectronics* – Behzad Razavi (Bám sát từng bài giảng Electronics 1 & 2, cực kỳ trực quan).
  2. *Design of Analog CMOS Integrated Circuits (2nd Edition)* – Behzad Razavi (Sách chuyên sâu về thiết kế vi mạch CMOS).
* 📖 **Cẩm nang hướng dẫn đọc sách chi tiết (80/20):** [razavi_analog_study_guide.md](file:///c:/Users/ddao20/Documents/analog/razavi_analog_study_guide.md)



### 1.1. Mô hình Transistor MOSFET *(Chặng 1: Razavi Elec 1 - Lec 29 đến 34 \| Sách CMOS Ch. 2)*
- [ ] Hiểu rõ 3 vùng hoạt động của MOSFET: Cut-off, Triode (Linear), và Saturation (Bão hòa).
- [ ] Nắm vững điều kiện bão hòa: $V_{DS} \ge V_{GS} - V_{th}$ và ý nghĩa điện áp vượt ngưỡng (Overdrive Voltage: $V_{OV} = V_{GS} - V_{th}$).
- [ ] Hiểu bản chất và công thức tính Độ hỗ dẫn: $g_m = \frac{\partial I_D}{\partial V_{GS}} = \sqrt{2 \mu C_{ox} \frac{W}{L} I_D}$.
- [ ] Hiểu hiệu ứng điều chế độ dài kênh (Channel-Length Modulation - $\lambda$) và trở kháng ra $r_o = \frac{1}{\lambda I_D}$.
- [ ] Nắm chắc Mô hình tín hiệu nhỏ (Small-Signal Model) cho MOS transistor tần số thấp.

### 1.2. Các khối khuếch đại 1 tầng cơ bản *(Chặng 2: Razavi Elec 1 - Lec 35 đến 39 \| Sách CMOS Ch. 3)*
- [ ] Mạch cực phát chung (Common-Source - CS): Tải điện trở, tải diode-connected, và **tải nguồn dòng (Current Source Load)**.
- [ ] Công thức vàng: $\text{Gain } A_v = -g_m \cdot R_{out}$.
- [ ] Mạch cực máng chung (Source Follower / Common-Drain - CD): Dùng làm tầng đệm (Buffer), trở kháng vào lớn, trở kháng ra nhỏ.
- [ ] Mạch cực cổng chung (Common-Gate - CG): Dùng cho ứng dụng tần số cao / phối hợp trở kháng.
- [ ] Kỹ thuật Cascode: Cách tăng trở kháng ra và độ lợi $A_v$ lên hàng chục lần.

### 1.3. Gương dòng điện & Cặp vi sai *(Chặng 3: Razavi Elec 2 - Lec 05-07, 12-16 \| Sách CMOS Ch. 4 & 5)*
- [ ] Hiểu nguyên lý sao chép dòng điện của Basic Current Mirror (tỷ lệ $W/L$).
- [ ] Hiểu Cascode Current Mirror để tăng độ chính xác của dòng điện.
- [ ] Mạch cặp khuếch đại vi sai (MOS Differential Pair): Tại sao chip luôn dùng tín hiệu vi sai (triệt tiêu nhiễu Common-Mode)?
- [ ] Cặp vi sai có tải gương dòng tích cực (Active Current Mirror Load) $\rightarrow$ Tầng 1 của Op-Amp.
- [ ] Tính toán Common-Mode Rejection Ratio (CMRR).

### 1.4. Kiến trúc Op-Amp & Bù tần số *(Chặng 4: Razavi Elec 2 - Lec 42 đến 45 \| Sách CMOS Ch. 6, 9 & 10)*
- [ ] Hiểu cấu trúc tổng thể của **Two-Stage Miller Op-Amp** (Tầng 1 vi sai + Tầng 2 CS).
- [ ] Ôn lại trực giác: $Z_C = \frac{1}{j\omega C}$ (Tụ hở mạch ở DC, ngắn mạch ở tần số cao).
- [ ] Hiểu bản chất Điểm cực (Pole) và Điểm không (Zero).
- [ ] Thành thạo cách đọc & phác thảo Biểu đồ Bode (Bode Plot: Biên độ và Pha).
- [ ] Nắm vững khái niệm Băng thông đơn vị (Unity-Gain Bandwidth - UGBW).
- [ ] Nắm vững Độ dự trữ pha (Phase Margin - PM): Tại sao PM phải $> 60^\circ$ để mạch không tự biến thành máy phát dao động?
- [ ] Kỹ thuật bù tần số Miller (Miller Compensation): Hiệu ứng tách cực (Pole Splitting) bằng tụ $C_c$ và triệt RHP Zero bằng điện trở $R_z$.

---

## GIAI ĐOẠN 2: THỰC HÀNH TẠI PHENIKAA VỚI CÔNG CỤ SYNOPSYS (2 THÁNG)
*Mục tiêu: Chuyển toàn bộ lý thuyết thành kỹ năng thực hành công cụ chuẩn công nghiệp.*

### 2.1. Làm chủ bộ công cụ Synopsys Custom Design
- [ ] Làm quen giao diện **Synopsys Custom Compiler** (Vẽ sơ đồ nguyên lý - Schematic).
- [ ] Thuộc lòng các phím tắt cốt lõi: `i` (lấy linh kiện), `w` (nối dây), `q` (chỉnh W/L), `m` (di chuyển).
- [ ] Thiết lập môi trường mô phỏng với **HSPICE / PrimeSim**.
- [ ] Thành thạo công cụ xem dạng sóng **Custom WaveView**.

### 2.2. Kỹ năng thiết lập mô phỏng cốt lõi
- [ ] **Mô phỏng DC (.dc):** Tìm điểm làm việc tĩnh (Q-point), kiểm tra các transistor có nằm trong vùng bão hòa (Saturation) hay không.
- [ ] **Mô phỏng AC (.ac):** Quét dải tần số từ 1 Hz đến 10 GHz để vẽ đồ thị Bode, đo Gain (dB) và Phase Margin.
- [ ] **Mô phỏng thời gian (.tran - Transient):** Đưa tín hiệu xung vuông / sóng sin vào để đo độ méo, độ trễ và tốc độ đáp ứng (Slew Rate).
- [ ] Đo công suất tiêu thụ của mạch ở trạng thái tĩnh.

---

## GIAI ĐOẠN 3: XÂY DỰNG DỰ ÁN PORTFOLIO CHUẨN ĐẦU RA (1 THÁNG)
*Mục tiêu: Tạo ra một sản phẩm hoàn chỉnh để gửi cho Giáo sư Đài Loan.*

### 3.1. Dự án cốt lõi: Two-Stage Miller CMOS Operational Amplifier
*Thiết kế trên tiến trình có sẵn tại Phenikaa hoặc mã nguồn mở SkyWater 130nm.*

- [ ] **Tầng 1 (Input Stage):** Thiết kế cặp vi sai (Differential Pair) có tải là gương dòng điện.
- [ ] **Tầng 2 (Output Stage):** Thiết kế tầng Common-Source để khuếch đại điện áp đầu ra (High Output Swing).
- [ ] **Mạch bù tần số:** Tính toán và cấy tụ Miller $C_c$ kèm điện trở $R_z$ để triệt tiêu Right-Half-Plane (RHP) Zero.
- [ ] **Đạt các chỉ tiêu kỹ thuật (Specs):**
  - [ ] Nguồn cấp $V_{DD} = 1.8V$ (hoặc $1.2V$).
  - [ ] DC Open-Loop Gain: $\ge 60\text{ dB}$ (Khuếch đại trên 1.000 lần).
  - [ ] Unity Gain Bandwidth (UGBW): $\ge 20 - 50\text{ MHz}$.
  - [ ] Phase Margin (PM): $\ge 60^\circ$ với tải dung $C_L = 2 - 5\text{ pF}$.
  - [ ] Slew Rate (SR): $\ge 20\text{ V/}\mu\text{s}$.
  - [ ] Công suất tiêu thụ: $\le 1\text{ mW}$.

### 3.2. Kiểm chứng nâng cao (Advanced Verification)
- [ ] **Chạy mô phỏng quét nhiệt độ:** Chạy từ $-40^\circ\text{C} \rightarrow 27^\circ\text{C} \rightarrow 125^\circ\text{C}$, chứng minh mạch vẫn ổn định.
- [ ] **Chạy mô phỏng quét góc chế tạo (Process Corners):** Kiểm tra các corner TT (Typical-Typical), SS (Slow-Slow), FF (Fast-Fast), SF, FS.
- [ ] **Kiểm tra biến thiên nguồn:** Thử nghiệm khi $V_{DD}$ sụt giảm $\pm 10\%$.

### 3.3. Đóng gói Báo cáo Kỹ thuật (Design Report)
- [ ] Viết một tài liệu PDF từ 10–15 trang hoàn toàn bằng **Tiếng Anh**:
  - [ ] Trang bìa: Tên dự án, họ tên, liên hệ, link GitHub / LinkedIn.
  - [ ] Mục 1: Mục tiêu & Bảng tóm tắt chỉ tiêu thiết kế (Specs Table).
  - [ ] Mục 2: Sơ đồ khối và tính toán lý thuyết bằng tay ($W/L$, dòng $I_D$, giá trị $C_c$).
  - [ ] Mục 3: Ảnh chụp sơ đồ Schematic chi tiết trên Synopsys Custom Compiler.
  - [ ] Mục 4: Ảnh chụp kết quả mô phỏng đồ thị Bode, Transient, Slew Rate từ WaveView.
  - [ ] Mục 5: Bảng tổng kết so sánh giữa **Tính toán lý thuyết** vs **Mô phỏng thực tế** vs **Kết quả quét PVT**.
  - [ ] Mục 6: Kết luận và hướng phát triển (ví dụ: Layout, mạch Bandgap Reference tích hợp).
- [ ] Tạo một GitHub Repository: Đẩy toàn bộ schematic, netlist, script mô phỏng và file PDF báo cáo lên (kèm file `README.md` trình bày chuyên nghiệp).

---

## GIAI ĐOẠN 4: NGOẠI NGỮ & BỘ HỒ SƠ DU HỌC (SONG SONG)

### 4.1. Ngoại ngữ
- [ ] Học tiếng Trung Phồn thể 3 buổi/tuần (Khóa 250 giờ *Modern Chinese 1 & 2*).
- [ ] Đăng ký thi chứng chỉ **TOCFL A2** (Dự kiến thi vào **Tháng 7/2027** sau khi kết thúc khóa 250 giờ; có thể thi thử sớm vào Tháng 3–4/2027).
- [ ] Đạt chứng chỉ TOCFL A2 chính thức.
- [ ] Chuẩn bị Tiếng Anh: Luyện tập nói trôi chảy phần giới thiệu bản thân và thuyết trình về dự án Op-Amp bằng tiếng Anh (10–15 phút).

### 4.2. Bộ hồ sơ học thuật (Application Package)
- [ ] **Curriculum Vitae (CV) chuẩn học thuật (1-2 trang):**
  - Nổi bật: Tốt nghiệp Bách Khoa Hà Nội (Kỹ sư Cơ điện tử).
  - Điểm nhấn: 4 năm kinh nghiệm Kỹ sư Phần mềm Java Backend (chứng minh tính tự lập, tư duy logic, kỹ năng lập trình).
  - Phần trọng tâm nhất: Mục **IC Design Projects** đặt lên hàng đầu, mô tả chi tiết dự án Op-Amp/LDO và chứng chỉ Synopsys.
- [ ] **Statement of Purpose (SOP) / Study Plan:**
  - Kể câu chuyện thuyết phục: Vì sao từ Cơ điện tử $\rightarrow$ làm Java Backend $\rightarrow$ quyết định theo đuổi Analog IC Design (yêu thích bản chất nguyên lý, muốn cống hiến lâu dài).
  - Nêu rõ định hướng nghiên cứu tại Đài Loan và lý do chọn Lab của Giáo sư.
- [ ] Dịch công chứng Bằng tốt nghiệp & Bảng điểm ĐHBK Hà Nội sang Tiếng Anh.
- [ ] Xin 2 Thư giới thiệu (Recommendation Letters) từ thầy cô cũ ở Bách Khoa hoặc sếp tại công ty làm việc.

---

## GIAI ĐOẠN 5: CHIẾN DỊCH "SĂN LAB" & NỘP HỌC BỔNG INTENSE (KỲ THU 2028)

### 5.1. Lập danh sách Giáo sư mục tiêu (Target Professors)
*Lập bảng Excel theo dõi 15 – 20 Giáo sư chuyên ngành Analog / Mixed-Signal / Power Management IC:*
- [ ] **NYCU (Dương Minh Giao Thông - Hsinchu):** Thánh địa vi mạch số 1, nhắm vào các Phó giáo sư trẻ hoặc trường ICST.
- [ ] **NTUST (Đài Khoa - Taipei):** Cực kỳ chuộng ứng viên đã có kinh nghiệm thực chiến đi làm, có học bổng INTENSE mạnh.
- [ ] **NCKU (Thành Công - Tainan):** Lò đào tạo kỹ thuật số 1 miền Nam, đối tác mật thiết của TSMC và MediaTek.
- [ ] **NCHU (Trung Hưng - Taichung):** Trường quốc lập số 1 miền Trung (cách Asia University 8km), có chương trình INTENSE bán dẫn.
- [ ] **NSYSU (Tôn Trung Sơn - Kaohsiung) & CCU (Trung Chính - Chiayi):** Tỷ lệ nhận rất cao, cơ sở vật chất bán dẫn tốt.

### 5.2. Gửi Cold Email & Phỏng vấn (Tháng 10 – 12/2027)
- [ ] Soạn mẫu email cá nhân hóa cho từng Giáo sư:
  - Đọc 1–2 bài báo nghiên cứu gần nhất của Giáo sư để nhắc tới trong email.
  - Tuyên bố rõ ràng: *Ứng tuyển diện Học bổng INTENSE Bán dẫn toàn phần (hoặc Tự túc kinh phí).*
  - Đính kèm: **CV + PDF Design Report dự án Op-Amp/LDO + Chứng chỉ Synopsys PSTC + Bằng TOCFL A2**.
- [ ] Theo dõi phản hồi, gửi follow-up email sau 7–10 ngày nếu chưa nhận được trả lời.
- [ ] Phỏng vấn online với Giáo sư:
  - Tự tin trình bày Slide dự án Op-Amp/LDO đã làm.
  - Trả lời các câu hỏi kỹ thuật về nguyên lý mạch và mô phỏng PVT/Post-sim.
- [ ] **Nhận được cái gật đầu của Giáo sư (Acceptance to join the Lab).**
- [ ] Hoàn tất thủ tục nộp hồ sơ chính thức qua cổng trường (Tháng 1 – 4/2028) để nhận giấy báo nhập học và Học bổng INTENSE.

---

## ⏰ THỜI KHÓA BIỂU THỰC TẾ CHO NGƯỜI ĐI LÀM FULL-TIME (TIME-BLOCKING)
*Nguyên tắc sống còn: "Tách bạch tuyệt đối" – Không học tiếng Trung và Vi mạch cùng một buổi tối để tránh kiệt sức.*

| Thứ | Khung giờ | Nội dung ưu tiên | Số giờ |
| :--- | :---: | :--- | :---: |
| **Thứ 2, 4, 6** | 19:30 – 22:00 | **Deep Work:** Học lý thuyết Analog / Thực hành mô phỏng | 2.5h / tối (Tổng 7.5h) |
| **Thứ 3, 5, 7** | 18:00 – 20:00 | Học Tiếng Trung trên lớp | 2h / tối |
| | 20:30 – 21:30 | Làm bài tập & Ôn từ vựng Tiếng Trung (Sau đó nghỉ ngơi) | 1h / tối |
| **Thứ 7 (Chiều)**| 14:00 – 17:00 | **Thực hành Analog:** Chạy mô phỏng / Xem bài giảng Razavi | 3h |
| **Chủ Nhật** | 08:30 – 12:00 | **Dự án Analog:** Tính toán, sửa lỗi mạch, vẽ Schematic | 3.5h |
| | Chiều & Tối | Nghỉ ngơi, sạc lại năng lượng, chuẩn bị cho tuần làm việc mới | Buffer / Relax |
| **TỔNG CỘNG** | | **Analog: ~14 giờ/tuần** \| **Tiếng Trung: ~9 giờ/tuần** | **Bền vững & Khả thi** |

---

## 📅 BẢNG THEO DÕI TIẾN ĐỘ THEO TUẦN (CHẶNG 1 – 4 LÝ THUYẾT & LTSPICE TẠI NHÀ)
| Giai đoạn | Tuần | Mục tiêu trọng tâm | Quỹ thời gian | Đánh giá |
| :---: | :---: | :--- | :---: | :---: |
| **GĐ 1** | **Tuần 1-2** | **Chặng 1:** Razavi Elec 1 (Lec 29-34) & Ch. 2 (Vật lý MOS, Saturation, $g_m, r_o$, Small-Signal) | 14h / tuần | [ ] |
| **GĐ 1** | **Tuần 3-4** | **Chặng 2:** Razavi Elec 1 (Lec 35-39) & Ch. 3 (Khuếch đại CS tải nguồn dòng, Biasing, Tầng 2 Op-Amp) | 14h / tuần | [ ] |
| **GĐ 1** | **Tuần 5-6** | **Chặng 3:** Razavi Elec 2 (Lec 05-07, 12-16) & Ch. 4, 5 (Gương dòng, Cặp vi sai tải tích cực, CMRR) | 14h / tuần | [ ] |
| **GĐ 1** | **Tuần 7-8** | **Chặng 4:** Razavi Elec 2 (Lec 42-45) & Ch. 9, 10 (Two-Stage Op-Amp, Phase Margin $>60^\circ$, Bù Miller $C_c, R_z$) | 14h / tuần | [ ] |

---

## 🗓️ DÒNG THỜI GIAN TỔNG THỂ HƯỚNG TỚI KỲ THU 2028 (MASTER MILESTONES)

| Mốc thời gian | Mục tiêu trọng tâm | Trạng thái đạt được | Check |
| :--- | :--- | :--- | :---: |
| **Cuối 2026 – Tháng 6/2027** | • Tự học lý thuyết Razavi Ch. 2–10 & Mô phỏng Two-Stage Op-Amp trên LTspice tại nhà.<br>• Học đều đặn lớp tiếng Trung Phồn thể 250 giờ (Tối T3, T5, T7).<br>• Duy trì công việc Java Backend, tích lũy tiền tiết kiệm. | Nắm chắc bản chất mạch tương tự, hoàn thành 2 quyển *Modern Chinese*. | [ ] |
| **Tháng 7/2027** | • **Thi chứng chỉ TOCFL A2** (Hà Nội).<br>• Thi test đầu vào để vào thẳng **Module 2 Phenikaa (18 triệu)**. | Cầm chắc bằng TOCFL A2, tiết kiệm 12 triệu Module 1. | [ ] |
| **Tháng 8 – Tháng 12/2027** | • Học thực hành Module 2 Phenikaa: Layout vi mạch, DRC/LVS, trích xuất PEX, Post-sim trên Synopsys Custom Compiler.<br>• Hoàn thiện tập **Design Report Op-Amp/LDO (15 trang tiếng Anh)**.<br>• Nhận **Chứng chỉ do Synopsys & PSTC đồng cấp**.<br>• Gửi **Cold Email** làm quen với 15–20 Giáo sư mục tiêu (NYCU, NCKU, NTUST, NCHU). | Bộ hồ sơ R&D hoàn hảo 100%, có sự đồng ý của Giáo sư. | [ ] |
| **Tháng 1 – Tháng 4/2028** | • Mở cổng nộp hồ sơ **KỲ THU 2028** chính thức trên hệ thống các trường.<br>• Nộp đơn xin **Học bổng INTENSE Bán dẫn toàn phần**. | Đã nộp đầy đủ hồ sơ sớm, không bị cập rập deadline. | [ ] |
| **Tháng 5 – Tháng 6/2028** | • Nhận **Letter of Acceptance** và Quyết định cấp **Học bổng INTENSE** (Miễn 100% học phí + trợ cấp sinh hoạt phí hàng tháng). | Cầm chắc vé nhập học trong tay. | [ ] |
| **Tháng 7 – Tháng 8/2028** | • Xin Visa du học, dịch thuật tư pháp, bàn giao công việc tại công ty Java, nghỉ ngơi bên gia đình. | Sẵn sàng tâm lý và hành lý. | [ ] |
| **Tháng 9/2028** | 🛫 **CHÍNH THỨC BAY SANG ĐÀI LOAN NHẬP HỌC THẠC SĨ BÁN DẪN!** | Bắt đầu hành trình chinh phục mức lương 1,7 tỷ/năm! | [ ] |

