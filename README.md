### **Hướng Dẫn Sử Dụng WhiskFlow Chi Tiết**

WhiskFlow được thiết kế để giúp bạn tự động hóa công việc trên Whisk một cách dễ dàng nhất. Hãy làm theo các bước dưới đây để tận dụng tối đa sức mạnh của công cụ này.

---

#### **Bước 1: Cài Đặt và Mở Giao Diện**

1.  **Cài đặt:** Thêm WhiskFlow vào trình duyệt của bạn từ [Chrome Web Store](https://chromewebstore.google.com/detail/gedfnhdibkfgacmkbjgpfjihacalnlpn).
2.  **Mở Whisk:** Truy cập vào trang làm việc của [Whisk Project](https://labs.google/fx/vi/tools/whisk/project).
3.  **Mở Giao Diện WhiskFlow:** Nhấp vào biểu tượng WhiskFlow trên thanh công cụ của trình duyệt để mở bảng điều khiển.

    > **Lưu ý:** WhiskFlow chỉ hoạt động khi bạn đang mở đúng trang Whisk. Nếu bạn ở trang khác, một thông báo sẽ hiện ra để nhắc nhở bạn.

---

#### **Bước 2: Nhập Danh Sách Prompt**

Đây là trái tim của WhiskFlow. Bạn có hai cách để nhập danh sách các ý tưởng của mình:

* **Cách 1: Dán trực tiếp:** Sao chép danh sách prompt từ bất cứ đâu (Notepad, Google Docs,...) và dán vào ô văn bản lớn có ghi "📝 Danh sách prompt". Hãy chắc chắn rằng mỗi prompt nằm trên một dòng riêng biệt.
* **Cách 2: Nhập từ file:**
    1.  Nhấp vào nút **"Nhập từ file (.txt)"**.
    2.  Chọn một file văn bản (`.txt`) từ máy tính của bạn. Nội dung của file sẽ tự động được đưa vào ô nhập liệu.

---

#### **Bước 3: Tùy Chỉnh Cài Đặt (Rất Quan Trọng!)**

Trong mục **"⚙️ Cài đặt"**, bạn có thể tinh chỉnh cách WhiskFlow hoạt động cho phù hợp với nhu cầu của mình:

* **Ngôn Ngữ (Language):** Lựa chọn giao diện hiển thị là Tiếng Việt hoặc Tiếng Anh.
* **Thời Gian Chờ (Wait Time):**
    * **Công dụng:** Đây là khoảng thời gian (tính bằng giây) mà công cụ sẽ chờ sau khi một prompt bị lỗi trước khi chuyển sang prompt tiếp theo.
    * **Khuyến nghị:** Nên đặt giá trị từ `10` giây trở lên để tránh Whisk khóa tạm thời tính năng của bạn do gửi yêu cầu quá nhanh.
* **Bắt Đầu Từ Prompt Số (Start From Prompt #):**
    * **Công dụng:** Nếu bạn muốn bỏ qua một vài prompt đầu tiên hoặc muốn tiếp tục một phiên làm việc bị dừng trước đó, hãy điền số thứ tự của prompt bạn muốn bắt đầu vào đây.
    * **Ví dụ:** Điền số `5`, WhiskFlow sẽ bắt đầu chạy từ prompt thứ 5 trong danh sách của bạn.
* **Tự Động Tải Về Hình Ảnh (Auto-download images):**
    * **Công dụng:** Khi tùy chọn này được bật, WhiskFlow sẽ tự động nhấp vào nút tải xuống ngay khi mỗi hình ảnh được tạo xong.
    * **⚠️ Yêu cầu quan trọng:** Để tính năng này hoạt động mượt mà, bạn nên vào phần Cài đặt của trình duyệt và **tắt tùy chọn "Hỏi vị trí lưu file trước khi tải về"**. Nếu không, trình duyệt sẽ hiện một hộp thoại hỏi lưu file mỗi lần tải ảnh, làm gián đoạn quá trình tự động. WhiskFlow có một thông báo nhắc nhở về việc này trong lần chạy đầu tiên.

---

#### **Bước 4: Bắt Đầu & Theo Dõi Tiến Trình**

1.  **Bắt đầu:** Sau khi đã thiết lập xong, nhấp vào nút **"▶️ Bắt đầu"**.
2.  **Theo dõi:**
    * **Thanh tiến trình:** Cho bạn biết tổng quan về tiến độ công việc đã hoàn thành.
    * **Trạng thái trực tiếp:** Hiển thị chính xác hành động hiện tại, ví dụ: "Đang xử lý prompt 5/50..." hoặc "Đã tạm dừng".
    * **Log chi tiết:** Cung cấp nhật ký đầy đủ về tất cả các hành động đã diễn ra, kèm theo thời gian thực.
3.  **Điều khiển:**
    * **Tạm dừng/Tiếp tục:** Trong lúc chạy, nút "Bắt đầu" sẽ chuyển thành **"⏸️ Tạm dừng"**. Bạn có thể nhấp để tạm ngưng và sau đó nhấp **"▶️ Tiếp tục"** để chạy lại.
    * **Dừng hẳn:** Nhấp vào nút **"⏹️ Dừng"** để kết thúc hoàn toàn phiên làm việc. Công cụ sẽ dừng lại ngay lập tức và chờ lệnh mới.

---

#### **Bước 5: Xem Lại và Xử Lý Lỗi**

* Trong mục **"⚠️ Prompt lỗi"**, WhiskFlow sẽ liệt kê tất cả các prompt không thể tạo được hình ảnh trong phiên làm việc.
* Sau khi phiên làm việc kết thúc, bạn có thể nhấp vào nút **"Sao chép các prompt lỗi"** để lưu lại danh sách này, sửa đổi và chạy lại chúng trong một phiên mới.
