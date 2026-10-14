### Nhiệm vụ 1: Kiểm tra dữ liệu trước khi ước lượng

| Mã Story | Đủ rõ | Cần làm rõ | Thông tin/câu hỏi còn thiếu |
| :--- | :---: | :---: | :--- |
| **LS01** | [ ] | [X] | Trạng thái của phiên có cần tự động chuyển đổi sang trạng thái khác (như "Đang diễn ra") khi đến đúng thời gian bắt đầu hay không? |
| **LS03** | [ ] | [X] | Khi nhiều khách hàng cùng bấm đặt mua một mặt hàng có số lượng tồn kho cuối cùng, hệ thống xử lý tranh chấp (concurrency) và cơ chế giữ/trừ tồn như thế nào? |

---

### Nhiệm vụ 2: Phân tích Planning Poker và chốt Story Point

| Mã Story | Mức ưu tiên | Kết quả phiếu | SP cuối cùng | Lý do ngắn |
| :--- | :---: | :---: | :---: | :--- |
| **LS01** | 1 | 3 - 3 - 5 - 3 | **3** | Phiếu chênh lệch do Dev C hiểu nhầm việc phải tự động đổi trạng thái khi đến giờ phát; sau khi PO làm rõ chỉ cần gán mặc định 'Sắp diễn ra', độ phức tạp và nỗ lực chỉ ở mức CRUD cơ bản, tương đương với **LS02 (3 SP)**. |
| **LS02** | 2 | 3 - 3 - 3 - 3 | **3** | Reference Story; các phiếu đã trùng nhau. |
| **LS03** | 3 | 5 - 8 - 8 - 5 | **8** | Phiếu chênh lệch do lo ngại rủi ro tranh chấp khi nhiều người cùng đặt hàng đồng thời và luồng hoàn/giảm tồn kho; sau khi PO xác nhận logic tranh chấp, độ phức tạp kỹ thuật và rủi ro race condition này cao hơn hẳn so với **LS02 (3 SP)**. |

---

### Nhiệm vụ 3: Phát hiện cách hiểu sai

Đề xuất "1 Story Point = 4 giờ" là sai vì Story Point là đơn vị ước lượng tương đối, phản ánh tổng hòa giữa khối lượng công việc, độ phức tạp kỹ thuật và mức độ rủi ro/không chắc chắn, chứ không phải thời gian làm việc tuyến tính. Nhóm Scrum dùng **Velocity** (số Story Point trung bình hoàn thành qua các Sprint thực tế) để dự báo sức chứa cho Sprint kế tiếp dựa trên năng lực tổng thể, giúp duy trì tính linh hoạt mà không cần ép buộc quy đổi cơ học sang giờ.