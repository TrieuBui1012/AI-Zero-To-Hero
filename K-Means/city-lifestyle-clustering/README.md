# 🌆 Bộ dữ liệu Phân khúc Lối sống Đô thị

## 📋 Tổng quan

Bộ dữ liệu này mô phỏng **các hồ sơ thành phố trên toàn cầu** nhằm khám phá lối sống đô thị thông qua các kỹ thuật học máy không giám sát. Dữ liệu phản ánh cách thu nhập, ô nhiễm, hạ tầng số và các yếu tố môi trường ảnh hưởng đến chất lượng sống — từ các siêu đô thị đông đúc đến các thành phố nhỏ thân thiện với môi trường.

---

## 🎯 Yêu cầu: Chia dữ liệu đầu vào thành các cụm kỳ vọng sau:

### 1. Trung tâm Công nghệ Đô thị
- Thu nhập cao, mật độ cao, chi phí thuê nhà lớn
- Ví dụ: trung tâm tài chính, thành phố công nghệ

### 2. Thành phố Đang Phát triển
- Thu nhập trung bình, Internet tăng nhanh, ô nhiễm cao

### 3. Thành phố Ngoại ô Thu nhập Thấp
- Hạ tầng yếu, Internet thấp, mật độ dân số thấp

### 4. Thành phố Nhỏ Thân thiện Môi trường
- Không khí sạch, nhiều cây xanh, mức độ hạnh phúc cao

### 5. Siêu Đô thị Công nghiệp
- Mật độ rất cao, ô nhiễm nặng, chất lượng sống thấp

---

## 🎯 Đặc điểm chính

- 300 **thành phố tổng hợp** thuộc 6 khu vực địa lý
- 10 **đặc trưng có tương quan thực tế**, đại diện cho kinh tế – môi trường – xã hội
- **Không có dữ liệu thiếu**
- Phân phối dữ liệu mô phỏng sát dữ liệu đô thị thực tế
- Tự nhiên hình thành **4–5 nhóm lối sống đô thị**

---

## 📊 Cấu trúc bộ dữ liệu

### Mô tả các cột

| Cột | Kiểu | Khoảng | Mô tả |
|---|---|---|---|
| city_name | string | – | Tên thành phố (tổng hợp) |
| country | string | 6 khu vực | Châu Âu, Châu Á, Bắc Mỹ, Nam Mỹ, Châu Phi, Châu Đại Dương |
| population_density | int | 100–25.000 | Mật độ dân số (người/km²) |
| avg_income | float | 300–7.000 | Thu nhập hộ gia đình TB/tháng (USD) |
| internet_penetration | float | 30–100 | % hộ gia đình có Internet |
| avg_rent | float | 150–3.000 | Tiền thuê nhà TB/tháng (USD) |
| air_quality_index | int | 20–180 | Chỉ số AQI (thấp = sạch) |
| public_transport_score | float | 10–95 | Điểm giao thông công cộng |
| happiness_score | float | 2–9 | Mức độ hài lòng cuộc sống |
| green_space_ratio | float | 2–60 | % diện tích không gian xanh |

### Thông tin file
- Tên file: `city_lifestyle_dataset.csv`
- Kích thước: ~300 dòng × 10 cột
- Định dạng: CSV UTF-8
- Giá trị thiếu: Không có

---

## 🌍 Đặc điểm theo khu vực

| Khu vực | Số TP | Thu nhập TB | Mật độ | Internet | AQI |
|---|---|---|---|---|---|
| Châu Âu | 60 | $3.500 | Trung bình | 88% | Tốt |
| Châu Á | 80 | $2.500 | Cao | 72% | Trung bình |
| Bắc Mỹ | 50 | $4.200 | Trung bình | 90% | Tốt |
| Nam Mỹ | 40 | $1.800 | Trung–Cao | 65% | Trung bình |
| Châu Phi | 35 | $900 | Thấp–Trung | 45% | Kém |
| Châu Đại Dương | 35 | $3.800 | Thấp | 92% | Rất tốt |