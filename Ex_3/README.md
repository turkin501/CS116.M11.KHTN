Bước 1: Cài đặt các thư viện cần thiết
!pip install osmnet
!pip install matplotlib==3.1.3
!pip install osmnet
!pip install pandana
!pip install folium

Bước 2: clone data từ https://github.com/CityScope/CSL_HCMC

Bước 3: Load ranh giới quận huyện và dân số quận huyện từ: Data\GIS\Population\population_HCMC\population_shapefile\Population_District_Level.shp

Bước 4: Lọc ra 5 quận huyện có tốc độ tăng dân số nhanh nhất (Pop2019/Pop2017)

Bước 5: Dùng spatial join (from geopandas.tools import sjoin) để lọc ra các điểm click của người dùng trong 5 quận/huyện hot nhất

Bước 6: chạy KMean cho top 5 quận huyện này. Lấy K = 30

Bước 7: Lưu cụm điểm nhiều nhất của mỗi quận

Bước 8: show lên bản đồ các cụm đông nhất theo từng quận theo dạng HEATMAP

Bước 0: tiền xử lý bằng Hough Transform để loại bỏ các click mà do máy tính crawl về
