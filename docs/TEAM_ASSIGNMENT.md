# Phân công FreshLens — Quản lý dự án phần mềm

Học phần: **Quản lý dự án phần mềm**. Bảng dưới ghi nhận phân công kỹ thuật đang được kế thừa của bốn thành viên. Vai trò quản lý, khối lượng, lịch thực hiện và tiêu chí nghiệm thu cần được nhóm thống nhất trong kế hoạch của học phần này.

| Thành viên | Vai trò kỹ thuật | Module chính |
| --- | --- | --- |
| Lương Thị Như Huỳnh — N23DCCN096 | TV1 dữ liệu và xử lý ảnh | freshlens_ai/data, inference/quality.py, PREPARE_CAMERA_MANIFEST.py |
| Võ Văn Đạt — N23DCCN078 | TV2 huấn luyện CNN | models, training, TRAIN_CNN_V2.py, BENCHMARK_MODELS.py |
| Hứa Như Quỳnh — N23DCCN118 | TV3 suy luận và đánh giá | inference, evaluation, EVALUATE_TV3.py, Grad-CAM |
| Nguyễn Thị Yến Nhi — N23DCCN112 | TV4 giao diện và tích hợp | ui, APP_CNN_V2.py, launcher, cài đặt, QA và tài liệu |

SVM trong legacy/svm chỉ là lịch sử/baseline.
Phân công là trách nhiệm kiểm tra và bàn giao, không tự chứng nhận thí nghiệm đã hoàn thành.

## Bàn giao

- Huỳnh: nhãn ảnh camera, group theo quả vật lý, nguồn ảnh, báo cáo trùng, ảnh trước/sau tiền xử lý; tách dev/calibration/final.
- Đạt: cấu hình, seed, checkpoint/hash, learning curves; chỉ công bố nâng cấp tốt hơn sau khi so cùng protocol. Candidate multi-task và resolution mới là thí nghiệm, chưa là production.
- Quỳnh: JSON/CSV/CM, error gallery, coverage/FAR, quality và latency. External V2 đã calibration không phải final test độc lập.
- Nhi: bốn trang chạy được, đổi ảnh xóa kết quả và heatmap, ảnh lỗi không crash, CPU fallback, cài mới, demo upload và camera thật.

Mỗi người kiểm tra yêu cầu, tiến độ, chất lượng và bằng chứng bàn giao thuộc phần mình. Nhi tổng hợp tài liệu theo phân công hiện có; cả nhóm xác nhận kết quả. Các thay đổi về phạm vi, người phụ trách hoặc thời hạn cần được ghi nhận trong kế hoạch và theo dõi công việc của học phần Quản lý dự án phần mềm. Xem [SUBMISSION.md](SUBMISSION.md) để chạy lại công cụ.
