# Bản đồ số cơ sở lưu trú – dữ liệu Nhóm 4

## Thành phần
- `index.html`: giao diện bản đồ tương tác Leaflet, bộ lọc, tìm kiếm, chi tiết cơ sở, thư viện ảnh, nút Google Maps.
- `du_lieu.js`: 22 bản ghi lấy từ workbook `NHOM4_MAU_THU_THAP_DU_LIEU_TEN_FILE_ANH(3).xlsx`.
- `anh/`: 66 ảnh lấy từ ZIP ảnh do Nhóm 4 cung cấp (3 ảnh cho mỗi mã điểm).

## Cách chạy
1. Giải nén toàn bộ thư mục.
2. Giữ nguyên `index.html`, `du_lieu.js` và thư mục `anh/` cùng cấp.
3. Mở `index.html` bằng Chrome hoặc Edge. Cần Internet để tải Leaflet và bản đồ nền.
4. Khi đưa lên GitHub Pages, tải lên cả ba tệp và thư mục `anh/`.

## Nguồn và cách giữ dữ liệu
- Dữ liệu cơ sở lấy từ sheet `DANH_SACH_22_CSLT`, các dòng dữ liệu 5–26.
- Chi tiết lấy từ sheet `KHAO_SAT_CHI_TIET`, ghép theo `Mã điểm`.
- Ảnh hiển thị lấy từ các tệp ảnh có tên tương ứng trong ZIP ảnh Nhóm 4. Các trường tên ảnh ban đầu từ Excel được giữ trong `photoRefs`.
- Tên, nhóm yêu cầu, loại hình thực tế, hạng sao, tọa độ, liên kết Google Maps, mô tả và giá được giữ theo dữ liệu nguồn; không tự sửa hoặc xác minh thay cho nhóm.

## Cần kiểm tra trước khi nộp
- **Workbook hiện cung cấp dữ liệu Đà Nẵng, không phải Hội An.** Vì vậy tiêu đề bản đồ đã đổi thành bản đồ cơ sở lưu trú Nhóm 4, tránh gắn nhãn sai địa điểm.
- Một số dòng được xếp vào nhóm yêu cầu `Homestay` nhưng cột `Loại hình thực tế` ghi `Resort`; website hiển thị riêng cả hai trường, không tự điều chỉnh.
- Tọa độ của mã `5S01` trong Excel là latitude `16.074809`, longitude `106.219579`; kinh độ này có vẻ không đồng nhất với địa chỉ ở Đà Nẵng. Website giữ nguyên dữ liệu Excel theo yêu cầu, nên cần kiểm tra tọa độ trước khi công bố. Nếu điểm này làm bản đồ thu nhỏ quá rộng, đó là do tọa độ nguồn.
- Các mức giá, mô tả, hạng sao và liên kết được xem là dữ liệu do nhóm cung cấp, không phải xác nhận độc lập hay giá hiện hành.
- Ảnh trong ZIP là ảnh do nhóm cung cấp; cần tự kiểm tra quyền sử dụng, nguồn ảnh và sự tương ứng với từng cơ sở trước khi công khai.

## Công nghệ
- [Leaflet](https://leafletjs.com/)
- [OpenStreetMap](https://www.openstreetmap.org/) / CARTO tiles
- [GitHub Pages](https://docs.github.com/en/pages)
