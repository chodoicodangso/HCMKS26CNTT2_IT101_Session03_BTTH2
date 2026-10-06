## **3\. Yêu cầu đầu ra**

### **Báo cáo phân tích:**

Giải thích tại sao đường dẫn tuyệt đối gây lỗi khi đổi máy. Phân tích luồng IPO của ứng dụng từ lúc nạp từ Storage vào RAM.  
**Lỗi đường dẫn tuyệt đối:** Đường dẫn tuyệt đối bị **cố định theo cấu trúc máy cũ** Khi sang máy mới, tên user hoặc cấu trúc thư mục thay đổi khiến Python không tìm thấy file   
**IPO:**  
**I (Input \- Nhập):** **CPU** ra lệnh lấy code và ảnh logo từ **Ổ cứng** truyền vào **RAM**.  
**P (Process \- Xử lý):** **CPU** đọc dữ liệu trên **RAM** để chạy ứng dụng. Do ảnh quá nặng hoặc code nạp ảnh bị lặp vô hạn, dữ liệu tràn ngập làm **RAM đầy 98%**, CPU bị quá tải gây treo máy.  
**O (Output \- Xuất):** Máy bị đứng hình, không hiển thị được giao diện Shopee-Lite.  
**Giải pháp kỹ thuật:**  
Viết lại cấu trúc đường dẫn tương đối sử dụng ký hiệu . và .. .Đề xuất 3 bước xử lý để giảm lag cho máy bạn thân dựa trên Task Manager.  
**Đường dẫn tương đối:**  
Dấu . : Đại diện thư mục hiện tại  
Dấu .. : Lùi lại một thư mục cha phía ngoài.  
**3 bước xử lý để giảm lag**  
Mở Task Manager, bấm vào cột Memory (RAM)   
Xem ai ngốn nhiều tài ngyên thì xóa  
Tắt bớt các ứng dụng chạy ngầm để giải phóng RAM cho máy. 

