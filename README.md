# 🎬 Netflix Data Analysis

🎯 ## Objective

Phân tích dữ liệu Netflix nhằm tìm hiểu đặc điểm của các thể loại phim và TV Show, từ đó xác định xu hướng phát triển nội dung trên nền tảng Netflix.

---

## 📂 Dataset

Nguồn: Netflix Titles Dataset

Bao gồm các thông tin:
- Title
- Type (Movie / TV Show)
- Country
- Release Year
- Rating
- Duration
- Listed_in (Category)
- Director
- Cast
- ...

---

## ⚙️ Data Cleaning

Các bước xử lý dữ liệu:

- Xóa các giá trị thiếu (`dropna`)
- Kiểm tra dữ liệu null theo từng cột
- Làm sạch cột `duration`
- Chuyển đổi kiểu dữ liệu
- Tách riêng dữ liệu Movie và TV Show
- Xử lý dữ liệu thời lượng:
  - Movie → phút
  - TV Show → số mùa

---

## 🔍 Analysis

### 1. Phân tích tổng quan nội dung
- So sánh số lượng Movie và TV Show
- Tính tỷ lệ phần trăm từng loại nội dung

### 2. Phân tích theo năm phát hành
- Số lượng Movie và TV Show theo từng năm
- Xu hướng tăng trưởng nội dung trên Netflix

### 3. Phân tích thời lượng
- Thời lượng trung bình của Movie theo năm
- Số mùa trung bình của TV Show theo năm

### 4. Phân tích theo Category
Sử dụng `groupby` để:
- Tính số lượng nội dung theo category
- So sánh xu hướng giữa các nhóm nội dung

---

## 📊 Visualization

- Bar chart:
  - So sánh Movie và TV Show
  - Top category phổ biến

- Line chart:
  - Xu hướng số lượng nội dung theo năm
  - Thời lượng trung bình theo năm

---

## 💡 Main Insights

- Movie chiếm phần lớn nội dung trên Netflix (~70%)
- Giai đoạn 2016–2019 là thời kỳ bùng nổ của Movie
- TV Show tăng trưởng chậm hơn nhưng ổn định
- Sau đại dịch Covid-19, số lượng nội dung phát hành giảm đáng kể
- Xu hướng hiện tại tập trung vào Movie có thời lượng dài hơn

---

## 📖 Data Storytelling

Mục tiêu của phân tích là tìm hiểu đặc điểm của các thể loại phim trên Netflix.

Phân tích cho thấy phần lớn nội dung trên nền tảng này là Movie (chiếm ~70%), phản ánh chiến lược phát triển của Netflix và xu hướng hiện tại của người xem.

Trước năm 2016 cho thấy sự cân bằng giữa 2 thể loại Movie và TV Show, nhưng từ 2016 đến 2019 là sự bùng nổ mạnh của thị trường phim điện ảnh với đỉnh điểm là hơn 1400 bộ phim được ra mắt trên nền tảng này. Song song đó TV Show vẫn có sự tăng trưởng nhất định.

Từ năm 2019 trở về sau, dưới ảnh hưởng của đại dịch Covid-19, số lượng nội dung được phát hành trên Netflix giảm đáng kể. Tuy vậy Movie vẫn duy trì khoảng hơn 1000 nội dung mỗi năm, trong khi TV Show cũng giảm nhẹ ở giai đoạn 2021.

Thời lượng trung bình qua các năm của các thể loại phim có sự khác biệt rõ rệt.

Trước năm 2014, thời lượng trung bình của TV Show khá cao và tăng lên đến khoảng 4.5 mùa, cho thấy Netflix từng tập trung phát triển nhiều nội dung thuộc thể loại này. Trong khi đó Movie lại có sự dao động mạnh và chưa ổn định.

Từ 2014 đến 2016 lại cho thấy xu hướng đối lập khi thời lượng trung bình của TV Show giảm đáng kể xuống còn khoảng 1.5 mùa, trong khi Movie bắt đầu ổn định hơn với thời lượng dao động khoảng 75–85 phút mỗi bộ.

Từ năm 2016 trở đi là giai đoạn phát triển mạnh của Movie khi thời lượng tăng dần và ổn định hơn ở các năm sau. Bên cạnh đó, dù phát triển chậm hơn nhưng TV Show cũng bắt đầu tăng trở lại về thời lượng của các series phim.

Từ các phân tích trên có thể thấy xu hướng phát triển chủ đạo hiện tại trên Netflix là Movie với thời lượng dài. Đồng thời TV Show với thời lượng dưới 3 mùa cũng đang xuất hiện ngày càng nhiều trên nền tảng.

---

## 🛠️ Technologies Used

- Python
- Pandas
- Matplotlib
- Jupyter Notebook

---

## 🚀 Project Structure

```text
project/
│
├── analysis.ipynb      # notebook chính
├── README.md           # mô tả project
└── netflix_titles.csv  # dữ liệu
```

---

## 📌 Conclusion

Dữ liệu cho thấy Netflix hiện đang tập trung mạnh vào Movie với số lượng và thời lượng ngày càng tăng.

Tuy TV Show không phát triển nhanh bằng Movie nhưng vẫn duy trì được sự ổn định và tiếp tục là một phần quan trọng của nền tảng.

Việc kết hợp phân tích dữ liệu, visualization và storytelling giúp hiểu rõ hơn về xu hướng phát triển nội dung của Netflix qua từng giai đoạn.

---
