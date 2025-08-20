### **Hướng Dẫn Sử Dụng Whisk Automation Tool**

**Whisk Automation Tool** là một tiện ích mở rộng giúp bạn tự động hóa toàn bộ quá trình gửi prompt và tải hàng loạt ảnh từ trang Google Whisk.

#### **1. Cài Đặt**

1.  Giải nén thư mục chứa code của extension.
2.  Mở trình duyệt Chrome, truy cập vào địa chỉ `chrome://extensions`.
3.  Bật **"Chế độ dành cho nhà phát triển"** (Developer mode) ở góc trên bên phải.
4.  Nhấn vào nút **"Tải tiện ích đã giải nén"** (Load unpacked) và chọn thư mục bạn vừa giải nén.
5.  Ghim extension lên thanh công cụ để dễ dàng sử dụng.

#### **2. Giao Diện Chính**

Khi bạn truy cập đúng trang Google Whisk, biểu tượng của tool trên thanh công cụ sẽ sáng lên. Nhấn vào đó để mở bảng điều khiển.

* **📝 Danh sách prompt:** Nơi bạn nhập hoặc dán danh sách các prompt, mỗi prompt nằm trên một dòng.
    * **Nút "Nhập từ file (.txt)":** Cho phép bạn tải lên một file văn bản chứa danh sách prompt.
* **▶️ Nút điều khiển:**
    * **Bắt đầu:** Chạy chu trình tự động hóa. Nút sẽ chuyển thành **Tạm dừng**.
    * **Tạm dừng/Tiếp tục:** Tạm dừng hoặc tiếp tục chu trình đang chạy.
    * **Dừng:** Hủy bỏ hoàn toàn chu trình hiện tại.
* **Thanh Trạng thái:** Hiển thị tiến trình (%), số lượng prompt đã xử lý và các thông báo trạng thái trực tiếp.
* **☕️ Ủng hộ tác giả:** Một icon ly cà phê nhỏ ở góc trên bên phải. Nếu thấy tool hữu ích, bạn có thể nhấn vào đây để mời tác giả một ly cà phê!

#### **3. Hướng Dẫn Sử Dụng**

**Bước 1: Chuẩn bị Prompt**
* Mở bảng điều khiển của tool.
* Nhập danh sách prompt vào ô **"Danh sách prompt"** hoặc nhấn nút **"Nhập từ file (.txt)"**.

**Bước 2: Tinh chỉnh Cài đặt (Không bắt buộc)**
* Mở mục **⚙️ Cài đặt**.
* **Thời gian chờ (giây):** Đây là khoảng thời gian tool sẽ chờ trước khi chuyển sang prompt tiếp theo nếu không phát hiện ảnh mới được tạo. Mặc định là `10` giây.
* **Tự động lưu log:** Nếu được chọn, tool sẽ tự động tải về một file `.txt` chứa toàn bộ nhật ký hoạt động khi chu trình hoàn tất.

**Bước 3: Bắt đầu**
* Nhấn nút **▶️ Bắt đầu**.
* **Lần chạy đầu tiên:** Tool có thể hiện một popup khuyên bạn nên tắt cài đặt "Hỏi vị trí lưu file" của trình duyệt để quá trình tải ảnh không bị gián đoạn.
* Tool sẽ tự động làm mới trang, gửi từng prompt, quét tìm ảnh mới và tự động tải chúng về.

**Bước 4: Theo dõi và Hoàn tất**
* Bạn có thể theo dõi toàn bộ quá trình qua mục **📄 Log chi tiết**. Các màu sắc và biểu tượng sẽ cho bạn biết chính xác điều gì đang diễn ra.
* Bạn có thể thoải mái **chuyển sang tab khác để làm việc**, tool sẽ tiếp tục chạy ngầm trên tab Whisk.
* Khi hoàn tất, tool sẽ hiển thị thông báo "✅ ĐÃ HOÀN THÀNH!".

#### **4. Xử lý Lỗi**

* Nếu một prompt nào đó bị lỗi (do nội dung không phù hợp hoặc lỗi từ Google), nó sẽ được ghi lại trong mục **⚠️ Prompt lỗi**.
* Bạn có thể nhấn nút **"Sao chép các prompt lỗi"** để lưu lại và thử lại sau. Tool sẽ không dừng lại mà tự động bỏ qua prompt lỗi và tiếp tục với các prompt còn lại.
