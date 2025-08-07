Hệ thống Gợi ý Phim (Movie Recommendation System)
Một hệ thống gợi ý phim cá nhân hóa, đề xuất các bộ phim phù hợp với người dùng dựa trên lịch sử tương tác và sở thích của họ.

Tính năng chính
Gợi ý dựa trên người dùng hoặc sản phẩm (Collaborative Filtering)
Hỗ trợ Graph Neural Networks (LightGCN) để học vector đặc trưng người dùng và phim
Huấn luyện mô hình và đánh giá bằng các chỉ số như MSE, Recall
Hỗ trợ dữ liệu MovieLens 100K
Gợi ý Top-K phim phù hợp cho từng người dùng

Công nghệ sử dụng
Ngôn ngữ: Python
Thư viện: NumPy, Pandas, PyTorch hoặc TensorFlow
Mô hình: Matrix Factorization / GNN (LightGCN)
Dữ liệu: MovieLens 100K

Link drive: bao gồm báo cáo, slide, data, ảnh 
https://drive.google.com/drive/folders/1x2AooDSPe0sgNZIoRBAmYdIiFSk_x3AH?usp=sharing

Bắt đầu
1. Clone dự án
git clone https://github.com/ten-cua-ban/movie-recommendation-system.git
cd movie-recommendation-system

2. Cài đặt thư viện phụ thuộc
pip install -r requirements.txt

3. Chuẩn bị dữ liệu
Tải tập dữ liệu MovieLens 100K và giải nén vào thư mục data/:
Trong folder data trong link drive

5. Huấn luyện mô hình
python 'movie recommendation.py'

6. Gợi ý phim cho người dùng
recommend_movies(user_id=1, top_k=10)

Đánh giá mô hình
Hệ thống hỗ trợ đánh giá chất lượng gợi ý bằng các chỉ số như MSE, Recall@K, Precision@K


Có thể mở rộng để đánh giá với tập kiểm tra và hiển thị kết quả trực quan
