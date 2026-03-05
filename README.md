# Computer Vision Assignment 2
**Gradient Domain Editing & Biến Đổi Hình Học**

> **Môn học:** Xử lý Ảnh Số và Thị Giác Máy Tính  
> **Giảng viên:** TS. Võ Thanh Hùng  

---

## 📋 Nội dung

### Phần 1: Gradient Domain Editing
- Ghép ảnh bằng Naive Copy-Paste
- Ghép ảnh bằng Gradient Domain Editing (`seamlessClone`)
- So sánh chất lượng giữa hai phương pháp

### Phần 2: Biến đổi hình học
- **Cơ bản:** Translation, Rotation, Scaling
- **Nâng cao:** Affine Transformation, Projective Transformation (Homography)
- So sánh Affine vs Projective

### Thử nghiệm mở rộng: Image Warping
- Dán ảnh lên mặt phẳng đích bằng Projective Transformation
- Xác định điểm tương ứng thủ công (hardcode)

---

## 🛠️ Công nghệ
- Python 3.8+
- OpenCV 4.x
- NumPy, SciPy, Matplotlib, Pillow

---

## 🚀 Chạy code

```bash
# Cài đặt
pip install opencv-python numpy scipy matplotlib pillow jupyter

# Chạy notebook
jupyter notebook BTL_2_full_v3.ipynb
```
## 📊 Kết quả chính

**Gradient Domain Editing:**  
`seamlessClone` cho kết quả tự nhiên hơn Naive Copy-Paste nhờ hòa trộn gradient tại vùng biên

**Geometric Transformations:**  
- Affine bảo toàn tính song song, Projective mô hình hóa phối cảnh đầy đủ
- Projective cần 4 điểm, Affine chỉ cần 3 điểm

**Image Warping:**  
Projective Transformation ánh xạ ảnh chính xác theo góc nhìn camera, kể cả khi mặt phẳng đích bị nghiêng

---

## 📚 Tài liệu tham khảo

1. Võ Thanh Hùng, *Slide bài giảng CV*, HCMUT, 2024-2025
2. Pérez et al., *Poisson Image Editing*, SIGGRAPH 2003
3. [OpenCV Documentation](https://docs.opencv.org/4.x/)
4. Hartley & Zisserman, *Multiple View Geometry in Computer Vision*, 2nd Ed., 2004
