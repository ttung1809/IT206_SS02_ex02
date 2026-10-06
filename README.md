# THIẾT KẾ MÔ HÌNH VẬN HÀNH AGILE CHO TOÀN MẢNG RIKKEIGO

## Phần 1. Kiến trúc mô hình

### 1. Các module vận hành

| Module                                | Trách nhiệm chính                                                                                                              |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| **1. Product Backlog**                | Product Owner quản lý, sắp xếp và điều chỉnh ưu tiên theo giá trị người dùng và mục tiêu sản phẩm.                             |
| **2. Sprint Planning**                | Product Owner, Scrum Master và Developers xác định Sprint Goal, lựa chọn công việc phù hợp và lập Sprint Backlog.              |
| **3. Development & Daily Scrum**      | Developers tự tổ chức thực hiện Sprint Backlog và đồng bộ tiến độ, phát hiện vướng mắc hằng ngày.                              |
| **4. Increment & Definition of Done** | Developers tạo Increment đạt Definition of Done; chỉ phần hoàn thành đúng tiêu chuẩn mới được coi là sản phẩm có thể kiểm tra. |
| **5. Sprint Review**                  | Scrum Team và các bên liên quan kiểm tra Increment, thu thập phản hồi và điều chỉnh Product Backlog khi cần.                   |
| **6. Sprint Retrospective**           | Scrum Team kiểm tra cách làm việc, xác định vấn đề và thống nhất các cải tiến cho Sprint tiếp theo.                            |
| **7. Cải tiến liên tục**              | Các cải tiến được đưa trở lại cách làm việc và Sprint tiếp theo, tạo thành vòng lặp Agile liên tục.                            |

### 2. Phân công cho 3 đội

* **Đội Đặt xe:** áp dụng Scrum, Sprint cố định 2 tuần vì yêu cầu thay đổi liên tục theo nhu cầu thị trường.
* **Đội Thanh toán:** áp dụng Scrum, Sprint cố định 2 tuần vì cần phản hồi thường xuyên và có khả năng thay đổi phương thức thanh toán.
* **Đội Đối soát:** **không bắt buộc áp dụng toàn bộ nhịp Scrum giống hai đội trên**. Đội này ưu tiên mô hình tuần tự và kiểm soát tuân thủ do yêu cầu ổn định, liên quan đến quy định thuế; tuy nhiên vẫn áp dụng các nguyên tắc Agile phù hợp như phản hồi sớm, kiểm tra và cải tiến khi quy định thay đổi.

### 3. Luồng giá trị

**Nhu cầu người dùng / Business**

↓

**Product Backlog**

↓

**Ưu tiên theo giá trị – Product Owner**

↓

**Sprint Planning**

↓

**Sprint 2 tuần – Developers tự tổ chức + Daily Scrum**

↓

**Increment đạt Definition of Done**

↓

**Sprint Review – Kiểm tra + nhận phản hồi**

↓

**Cập nhật Product Backlog**

↓

**Sprint Retrospective – Cải tiến cách làm việc**

↺ **Quay lại Sprint tiếp theo**

Luồng trên thể hiện 3 trụ cột Scrum:

> **Minh bạch → Thanh tra → Thích nghi**

và phản ánh 4 giá trị Agile, trong đó đặc biệt nhấn mạnh **phản hồi với thay đổi** và **phần mềm chạy được**.

---

## Phần 2. Xử lý tình huống ngoài dự kiến

### Tình huống 1: Sprint Review không có hạng mục nào đạt tiêu chuẩn "Done"

| Nội dung                     | Cách xử lý                                                                                                                                                               |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Mô hình phát hiện ở đâu?** | Phát hiện tại **Sprint Review** khi kiểm tra Increment theo Definition of Done.                                                                                          |
| **Ai xử lý?**                | **Developers** chịu trách nhiệm về chất lượng Increment; Product Owner và các bên liên quan cung cấp phản hồi; Scrum Master hỗ trợ Scrum Team xử lý vấn đề.              |
| **Xử lý thế nào?**           | Không coi phần chưa đạt là Increment "Done". Đội phân tích nguyên nhân, đưa công việc cần thiết trở lại Product Backlog và cải tiến cách làm trong Sprint Retrospective. |

### Tình huống 2: Đội Thanh toán muốn kéo dài Sprint thêm 1 tuần

| Nội dung                     | Cách xử lý                                                                                                                                                                                                         |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Mô hình phát hiện ở đâu?** | Phát hiện khi đội Thanh toán đề xuất thay đổi độ dài Sprint đang diễn ra.                                                                                                                                          |
| **Ai xử lý?**                | **Scrum Master** bảo vệ nguyên tắc Scrum và hỗ trợ đội xử lý vấn đề; Developers điều chỉnh phạm vi công việc nếu cần.                                                                                              |
| **Xử lý thế nào?**           | Không kéo dài Sprint đang chạy. Giữ nguyên Sprint 2 tuần, hoàn thành phần đạt được và đưa phần chưa xong về Product Backlog để ưu tiên cho Sprint tiếp theo. Các đội tiếp tục giữ chung nhịp Sprint đã thống nhất. |

### Kết luận

Mô hình RikkeiGo sử dụng **Scrum làm khung vận hành chung cho các đội có yêu cầu biến động**, trong khi cho phép Đội Đối soát áp dụng cách làm phù hợp với đặc thù tuân thủ. Mô hình vẫn giữ được vòng lặp **Nhu cầu → Ưu tiên → Sprint → Increment → Phản hồi → Cải tiến**, nhờ đó có thể thích nghi mà không phá vỡ nhịp vận hành chung.
