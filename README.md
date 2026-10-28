# Ứng dụng Thời tiết 8 Thành phố Việt Nam

Ứng dụng React + TypeScript hiển thị thời tiết hiện tại và dự báo 7 ngày cho 8 thành phố tại Việt Nam, sử dụng API Open-Meteo miễn phí, không yêu cầu API key.

## Chức năng

- Hiển thị danh sách 8 thành phố:
  - Hà Nội
  - Hải Phòng
  - Huế
  - Đà Nẵng
  - Nha Trang
  - Đà Lạt
  - TP. Hồ Chí Minh
  - Cần Thơ
- Làm nổi bật thành phố đang được chọn.
- Hiển thị thời tiết hiện tại:
  - Biểu tượng và mô tả thời tiết
  - Nhiệt độ
  - Độ ẩm
  - Tốc độ gió
  - Thời điểm cập nhật
- Hiển thị dự báo 7 ngày: thứ/ngày, biểu tượng, nhiệt độ cao nhất và thấp nhất.
- Có trạng thái chưa chọn thành phố, đang tải và lỗi kèm nút **Thử lại**.
- Đổi đơn vị nhiệt độ giữa °C và °F mà không gọi lại API.
- Giao diện responsive:
  - Từ 768px: bố cục hai cột.
  - Dưới 768px: bố cục xếp dọc.
- Nền giao diện đổi theo tình trạng thời tiết, có animation nhẹ.

## Công nghệ sử dụng

- React
- TypeScript
- Vite
- Oxlint
- Open-Meteo API

## Cấu trúc thư mục
  src/
  ├── components/
  │   └── Forecast.tsx
  ├── data/
  │   └── cities.ts
  ├── services/
  │   └── weatherApi.ts
  ├── types/
  │   └── weather.ts
  ├── utils/
  │   ├── temperature.ts
  │   └── weatherCode.ts
  ├── App.tsx
  ├── App.css
  ├── index.css
  └── main.tsx

## Yêu cầu cài đặt

Cần cài đặt trước:

- Node.js phiên bản 20 trở lên
- npm

Kiểm tra phiên bản:

```bash
node -v
npm -v
