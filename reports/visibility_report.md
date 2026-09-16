# Visibility report

- Thư mục nhãn: `dataset\labels\train`
- 20 ảnh, 28 skeleton, trung bình 15.75 khớp có v > 0 mỗi người
- Tổng: v=2 326 | v=1 115 | v=0 35

| # | Khớp | v=2 | v=1 | v=0 | %v=1 |
| ---: | --- | ---: | ---: | ---: | ---: |
| 0 | nose | 22 | 6 | 0 | 21% |
| 1 | left_eye | 20 | 8 | 0 | 29% |
| 2 | right_eye | 21 | 7 | 0 | 25% |
| 3 | left_ear | 10 | 18 | 0 | 64% |
| 4 | right_ear | 13 | 15 | 0 | 54% |
| 5 | left_shoulder | 25 | 3 | 0 | 11% |
| 6 | right_shoulder | 27 | 1 | 0 | 4% |
| 7 | left_elbow | 23 | 4 | 1 | 14% |
| 8 | right_elbow | 26 | 2 | 0 | 7% |
| 9 | left_wrist | 19 | 8 | 1 | 29% |
| 10 | right_wrist | 20 | 7 | 1 | 25% |
| 11 | left_hip | 19 | 8 | 1 | 29% |
| 12 | right_hip | 22 | 5 | 1 | 18% |
| 13 | left_knee | 14 | 8 | 6 | 29% |
| 14 | right_knee | 17 | 5 | 6 | 18% |
| 15 | left_ankle | 14 | 5 | 9 | 18% |
| 16 | right_ankle | 14 | 5 | 9 | 18% |

## Đọc bảng này thế nào

1. Khớp nào có **%v=1 cao**: khớp hay bị che. Cổ tay và hông thường là hai vị trí cần xem lại guideline trước khi kết luận.
2. Khớp nào có **v=0 cao bất thường**: mọi người đang dùng Outside ở chỗ đáng lẽ là Occluded. Đó là lỗi số 3 của slide 46, và nó xoá thẳng khớp đó khỏi bảng điểm OKS.
3. Khi so hai người: **lệch lớn = bất đồng về guideline**, không phải về bức ảnh. Sửa guideline trước, sửa nhãn sau.
