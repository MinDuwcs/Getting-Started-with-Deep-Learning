# Tổng Quan & Tóm Tắt Bài Báo Khoa Học - Deep Learning

> **Môn học:** Học Sâu  
> **Giảng viên hướng dẫn:** TS. Đỗ Như Tài  
> **Sinh viên thực hiện:** Đường Minh Đức  
> **MSSV:** 3123580010  
> **Lớp:** DDU1231  
> **Khoa:** Toán - Ứng Dụng, Trường Đại Học Sài Gòn  

---

## 📌 Tổng Quan

Repository này lưu trữ tài liệu tóm tắt và nghiên cứu các bài báo khoa học nền tảng trong lĩnh vực **Học Sâu (Deep Learning)** cũng như các công trình đặt nền móng cho **Mạng Thần Kinh Nhân Tạo (ANN)** được vinh danh tại **Giải Nobel Vật Lý 2024**.

---

## 📚 Nội Dung Tóm Tắt Chi Tiết

### 📄 Bài 1: Deep Learning
* **Tác giả:** Yann LeCun, Yoshua Bengio, Geoffrey Hinton
* **Nguồn:** Nature, Tập 521, 2015

1. **Học biểu diễn (Representation Learning) & Bản chất Học sâu:**
   * Khác với học máy nông (traditional machine learning) dựa vào trích xuất đặc trưng thủ công, học sâu tự động học các biểu diễn phân cấp từ dữ liệu thô thông qua nhiều tầng phi tuyến (từ đường nét, họa tiết đến bộ phận và đối tượng hoàn chỉnh).
2. **Cơ chế Huấn luyện:**
   * Thuật toán Lan truyền ngược (Backpropagation) áp dụng quy tắc chuỗi để tính gradient độ lỗi, kết hợp SGD (Stochastic Gradient Descent) để tinh chỉnh trọng số.
   * Việc áp dụng hàm kích hoạt ReLU giúp huấn luyện mạng sâu nhanh hơn nhiều so với các hàm Sigmoid/Tanh truyền thống.
   * Bài báo chứng minh không gian tối ưu hóa nhiều chiều bị chi phối bởi các điểm yên ngựa (saddle points) chứ không phải cực tiểu địa phương (local minima).
3. **Hai kiến trúc cốt lõi:**
   * **Mạng thần kinh cuộn (CNN):** Dành cho dữ liệu mảng (hình ảnh, video), dựa trên 4 nguyên lý: kết nối cục bộ, chia sẻ trọng số, gom tụ (pooling) và kết hợp nhiều tầng.
   * **Mạng thần kinh hồi quy (RNN) & LSTM:** Dành cho dữ liệu chuỗi (văn bản, tiếng nói) nhờ lưu trữ vector trạng thái bộ nhớ. Cấu trúc LSTM giải quyết triệt để bài toán triệt tiêu gradient (vanishing gradient).
4. **Biểu diễn phân tán & Định hướng:**
   * Ngôn ngữ được mã hóa thành các vector biểu diễn phân tán (word embeddings) trong không gian liên tục.
   * Tương lai học sâu tập trung vào Học không giám sát (Unsupervised Learning), kết hợp Học tăng cường (Reinforcement Learning) và khả năng biểu diễn lập luận phức tạp.

---

### 📄 Bài 2: Giải Nobel Vật lý 2024 (Popular Science)
* **Nguồn:** The Royal Swedish Academy of Sciences (nobelprize.org)

1. **Giao thoa giữa Vật lý và Học máy:**
   * Giải Nobel Vật lý 2024 vinh danh John J. Hopfield và Geoffrey E. Hinton vì đã vận dụng các nguyên lý toán học và mô hình vật lý (spin từ tính, cơ học thống kê Boltzmann) để xây dựng nền móng cho Mạng thần kinh nhân tạo (ANN).
2. **Mạng Hopfield & Bộ nhớ liên tưởng (1982):**
   * Sử dụng mô hình spin từ tính để tạo lập một "bản đồ năng lượng" (Energy Landscape).
   * Khi nạp vào một mẫu dữ liệu nhiễu hoặc thiếu sót, hệ thống tự động đưa trạng thái về đáy thung lũng năng lượng thấp nhất để tái tạo chính xác mẫu gốc.
3. **Máy Boltzmann & Đột phá RBM (1985–2006):**
   * Ứng dụng phương trình xác suất Boltzmann cùng các nút ẩn (hidden nodes) để phát hiện đặc trưng dữ liệu.
   * Việc rút gọn thành Restricted Boltzmann Machine (RBM) và kỹ thuật tiền huấn luyện xếp chồng tầng (pretraining) năm 2006 đã khởi đầu cho cuộc cách mạng Học sâu (Deep Learning).
4. **Tác động hai chiều:**
   * Vật lý cung cấp công cụ toán học xây dựng AI, và ngược lại, ANN trở thành công cụ phân tích đắc lực cho vật lý (tìm kiếm hạt Higgs, sóng hấp dẫn, lỗ đen, dự đoán cấu trúc 3D protein AlphaFold và phát triển vật liệu mới).

---

### 📄 Bài 3: Giải Nobel Vật lý 2024 (Scientific Background)
* **Nguồn:** The Royal Swedish Academy of Sciences (nobelprize.org)

1. **Bối cảnh Lịch sử & Khủng hoảng Perceptron:**
   * Từ mô hình nơ-ron nhị phân McCulloch-Pitts (1943) và quy tắc Hebb (1949), Perceptron của Rosenblatt (1957) ra đời nhưng bị Minsky & Papert (1969) chứng minh hạn chế ở các bài toán phi tuyến (như bài toán XOR), dẫn đến sự đóng băng của nghiên cứu ANN ("Mùa đông AI").
2. **Mạng Hopfield & Hàm Năng lượng Spin (1982):**
   * John Hopfield ứng dụng lý thuyết vật lý từ tính (mô hình Ising, spin glass) thiết lập mạng hồi quy có hàm năng lượng:
     $$E = -\sum_{i < j} w_{ij} s_i s_j$$
   * Hàm năng lượng giảm đơn điệu, giúp các ký ức hội tụ về các cực tiểu địa phương (thung lũng năng lượng) để khôi phục dữ liệu nhiễu.
3. **Máy Boltzmann, RBM & Bước ngoặt Học sâu (1985–2006):**
   * Geoffrey Hinton tích hợp phân bố xác suất Boltzmann $P(s) \propto e^{-E/T}$ và các nút ẩn.
   * Đột phá Restricted Boltzmann Machine (RBM) loại bỏ kết nối nội tầng kết hợp thuật toán Contrastive Divergence (2002) và tiền huấn luyện từng tầng (2006) đã giải quyết bài toán khởi tạo trọng số cho các mạng sâu.
4. **Đóng góp Hai chiều cho Khoa học:**
   * ANN trở lại làm công cụ phân tích đắc lực cho vật lý và khoa học tự nhiên: phát hiện hạt Higgs (CERN), chụp ảnh lỗ đen (EHT), phân tích Neutrino (IceCube), dự đoán cấu trúc 3D protein (AlphaFold), chẩn đoán y tế và mô phỏng vật liệu mới.

---

## 🛠️ Tech Stack & Môi Trường

* **Ngôn ngữ & Thư viện:** Python 3.x, PyTorch / TensorFlow, NumPy, Matplotlib
* **Quản lý mã nguồn & Đóng gói:** Git, GitHub, Docker
* **Công cụ soạn thảo & Quản lý tri thức:** Obsidian, Markdown
