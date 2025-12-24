# 🎄 Cây Thông Noel 3D Tương Tác với AI

> Một ứng dụng web 3D cao cấp được xây dựng với **React**, **Three.js (R3F)** và **nhận diện cử chỉ AI**.

🌐 **[Xem Demo Trực Tiếp](https://christmas-tree-gamma-silk.vercel.app/)**

Đây không chỉ là một cây thông - mà là một **bộ sưu tập kỷ niệm tương tác**. Hàng ngàn hạt phát sáng, đèn lấp lánh và những tấm ảnh polaroid lơ lửng cùng nhau tạo nên một cây thông Giáng sinh lung linh. Người dùng có thể điều khiển cây bằng **cử chỉ tay** thông qua camera!

---

## ✨ Tính Năng Chính

- 🌟 **Trải nghiệm hình ảnh tuyệt đẹp**: 15,000+ hạt phát sáng tạo thành tán cây, hiệu ứng Bloom và ánh sáng lung linh
- 📸 **Bộ sưu tập kỷ niệm**: Ảnh được hiển thị theo phong cách "polaroid" lơ lửng trên cây
- 🤖 **Điều khiển bằng cử chỉ AI**: Không cần chuột - dùng tay để điều khiển!
- 🎁 **Chi tiết phong phú**: Đèn nhấp nháy, tuyết rơi, quà và kẹo trang trí
- ⚙️ **Dễ tùy chỉnh**: Thay thế ảnh và điều chỉnh số lượng dễ dàng

---

## 🖐️ Hướng Dẫn Cử Chỉ Tay

| Cử chỉ | Chức năng | Mô tả |
|--------|-----------|-------|
| 🖐 **Xòe bàn tay** | Phân tán | Cây thông tan ra thành các hạt bay lơ lửng |
| ✊ **Nắm tay** | Tập hợp | Tất cả phần tử tụ lại thành cây thông hoàn chỉnh |
| 🤟 **ILoveYou** | Xem ảnh chi tiết | Mở/đóng chế độ xem ảnh lớn |
| 👍 **Thích (Thumb Up)** | Ảnh tiếp theo | Chuyển sang ảnh kế tiếp |
| 👎 **Không thích (Thumb Down)** | Ảnh trước đó | Quay lại ảnh trước |
| 👋 **Di chuyển tay trái/phải** | Xoay cây | Xoay góc nhìn cây thông |

> 💡 **Mẹo**: Bấm nút **DEBUG** ở góc phải dưới để xem camera và cử chỉ đang được nhận diện!

---

## 🛠️ Công Nghệ Sử Dụng

- **Framework**: React 18, Vite
- **3D Engine**: React Three Fiber (Three.js)
- **Thư viện hỗ trợ**: @react-three/drei, Maath
- **Hiệu ứng**: @react-three/postprocessing
- **AI Vision**: MediaPipe Tasks Vision (Google)

---

## 🚀 Cài Đặt & Chạy

### 1. Yêu cầu hệ thống
- [Node.js](https://nodejs.org/) phiên bản 18 trở lên
- Camera (webcam) cho chức năng nhận diện cử chỉ

### 2. Cài đặt
```bash
# Clone repo
git clone https://github.com/imhnam/christmas-tree.git
cd christmas-tree

# Cài đặt dependencies
npm install
```

### 3. Chạy ứng dụng
```bash
npm run dev
```

Truy cập: `http://localhost:5173`

---

## 🖼️ Tùy Chỉnh Ảnh

### Thay thế ảnh của bạn

1. Tìm thư mục `public/photos/`
2. Thay thế các file ảnh với tên:
   - `top.jpg` - Ảnh đỉnh cây (tùy chọn)
   - `1.jpg`, `2.jpg`, `3.jpg`... - Các ảnh trên cây

### Thêm/bớt số lượng ảnh

Mở file `src/App.tsx`, tìm dòng ~19:
```javascript
const TOTAL_NUMBERED_PHOTOS = 31; // Thay đổi số này
```

> 💡 **Gợi ý**: Dùng ảnh vuông hoặc tỷ lệ 4:3, kích thước < 500KB để đảm bảo hiệu suất.

---

## ⚙️ Cấu Hình Nâng Cao

Trong `src/App.tsx`, bạn có thể điều chỉnh tại object `CONFIG`:

```javascript
const CONFIG = {
  colors: { ... },     // Màu sắc cây, đèn, viền ảnh
  counts: {
    foliage: 15000,    // Số hạt lá cây
    ornaments: 300,    // Số ảnh polaroid
    lights: 400        // Số đèn nhấp nháy
  },
  tree: { 
    height: 22,        // Chiều cao cây
    radius: 9          // Bán kính cây
  }
};
```

---

## 📄 Giấy Phép

MIT License - Tự do sử dụng và chỉnh sửa cho mục đích cá nhân!

---

## 🎄 Chúc Mừng Giáng Sinh! 

Made with ❤️ for the holiday season ✨
