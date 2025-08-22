### **Hướng Dẫn Sử Dụng WhiskFlow Chi Tiết**
*Cập nhật lần cuối: 23 tháng 8, 2025*

WhiskFlow được thiết kế để giúp bạn tự động hóa công việc trên Whisk một cách thông minh và linh hoạt nhất. Hãy làm theo các bước dưới đây để tận dụng tối đa sức mạnh của công cụ này.

---

#### **Bước 1: Cài Đặt & Khởi Động**

1.  **Cài đặt:** Cài đặt tiện ích **[WhiskFlow](https://chromewebstore.google.com/detail/gedfnhdibkfgacmkbjgpfjihacalnlpn)** vào trình duyệt của bạn.
2.  **Mở Whisk:** Truy cập vào trang làm việc của **[Whisk Project](https://labs.google/fx/vi/tools/whisk/project)**.
3.  **Mở Giao Diện WhiskFlow:** Nhấp vào biểu tượng WhiskFlow trên thanh công cụ của trình duyệt để mở bảng điều khiển.

    > **Lưu ý:** WhiskFlow chỉ hoạt động khi bạn đang mở đúng trang Whisk. Nếu bạn ở trang khác, một giao diện chặn sẽ hiện ra để hướng bạn chuyển đến trang làm việc.

---

#### **Bước 2: Chuẩn Bị Danh Sách Prompt**

Đây là trái tim của WhiskFlow. Bạn có hai cách để nhập danh sách các ý tưởng của mình:

* **Cách 1: Dán trực tiếp:** Sao chép danh sách prompt từ bất cứ đâu (Notepad, Google Docs,...) và dán vào ô văn bản lớn có ghi "📝 Danh sách prompt". Hãy chắc chắn rằng mỗi prompt nằm trên một dòng riêng biệt.

* **Cách 2: Nhập từ file:**
    1.  Nhấp vào nút **"Nhập từ file (.txt)"**.
    2.  Chọn một file văn bản (`.txt`) từ máy tính của bạn. Nội dung của file sẽ tự động được đưa vào ô nhập liệu.
    3.  Sau khi nhập thành công, **log chi tiết** sẽ hiển thị thông báo ‘Đã nhập X prompts từ file...’ để bạn biết chính xác số lượng.

---

#### **Bước 3: Tinh Chỉnh Cài Đặt (Phần Quan Trọng Nhất)**

Giao diện cài đặt được thiết kế lại gọn gàng và chia thành hai nhóm chính để bạn dễ dàng tùy chỉnh.

##### **Cài đặt Tác vụ**
Đây là các tùy chọn ảnh hưởng trực tiếp đến quy trình chạy.

* **Thời gian chờ ngẫu nhiên (giây):**
    * **Công dụng:** Đây là nâng cấp mạnh mẽ nhất giúp tool hoạt động "giống người" hơn. Thay vì một số cố định, bạn cung cấp một **khoảng** thời gian (ví dụ: từ `5` đến `15` giây). Tool sẽ chọn ngẫu nhiên một con số trong khoảng này để làm thời gian chờ sau khi gặp lỗi hoặc khi chờ tải ảnh.
    * **Khuyến nghị:** Giữ khoảng thời gian tối thiểu từ `5` giây trở lên để đảm bảo an toàn, tránh bị Whisk phát hiện.

* **Thực thi mỗi prompt:**
    * **Công dụng:** Tính năng mới cho phép bạn chạy mỗi prompt nhiều lần trước khi chuyển sang prompt tiếp theo.
    * **Ví dụ:** Điền số `2`, tool sẽ chạy prompt 1 hai lần, sau đó mới chuyển sang chạy prompt 2 hai lần, và cứ thế tiếp tục.

* **Bắt đầu từ prompt:**
    * **Công dụng:** Nếu bạn muốn bỏ qua một vài prompt đầu tiên hoặc muốn tiếp tục một phiên làm việc bị dừng trước đó, hãy điền số thứ tự của prompt bạn muốn bắt đầu vào đây.
    * **Ví dụ:** Điền số `5`, WhiskFlow sẽ bắt đầu chạy từ prompt thứ 5 trong danh sách của bạn.

##### **Cài đặt Chung**
Đây là các tùy chọn về hành vi chung của công cụ.

* **Tự động tải ảnh:**
    * **Công dụng:** Khi tùy chọn này được bật, WhiskFlow sẽ tự động nhấp vào nút tải xuống ngay khi mỗi hình ảnh được tạo xong.
    * **⚠️ Yêu cầu quan trọng:** Để tính năng này hoạt động mượt mà, bạn nên vào phần Cài đặt của trình duyệt và **tắt tùy chọn "Hỏi vị trí lưu file trước khi tải về"**. Nếu không, trình duyệt sẽ hiện một hộp thoại hỏi lưu file mỗi lần tải ảnh, làm gián đoạn quá trình tự động.

* **Ngôn ngữ (Language):** Lựa chọn giao diện hiển thị là Tiếng Việt hoặc Tiếng Anh.

---

#### **Bước 4: Bắt Đầu & Theo Dõi Tiến Trình**

1.  **Bắt đầu:** Sau khi đã thiết lập xong, nhấp vào nút **"▶️ Bắt đầu"**.
2.  **Theo dõi:**
    * **Thanh tiến trình:** Cho bạn biết tổng quan về tiến độ công việc đã hoàn thành.
    * **Trạng thái trực tiếp:** Hiển thị chính xác hành động hiện tại, ví dụ: ‘Đang xử lý prompt 1/50 (Lần 2/2)...’ hoặc "Đã tạm dừng".
    * **Log chi tiết:** Cung cấp nhật ký đầy đủ về tất cả các hành động đã diễn ra, kèm theo thời gian thực.
3.  **Điều khiển:**
    * **Tạm dừng/Tiếp tục:** Trong lúc chạy, nút "Bắt đầu" sẽ chuyển thành **"⏸️ Tạm dừng"**. Bạn có thể nhấp để tạm ngưng và sau đó nhấp **"▶️ Tiếp tục"** để chạy lại.
    * **Dừng hẳn:** Nhấp vào nút **"⏹️ Dừng"** để kết thúc hoàn toàn phiên làm việc.

---

#### **Bước 5: Xem Lại và Xử Lý Lỗi**

* Trong mục **"⚠️ Prompt lỗi"**, WhiskFlow sẽ liệt kê tất cả các prompt không thể tạo được hình ảnh trong phiên làm việc.
* Sau khi phiên làm việc kết thúc, bạn có thể nhấp vào nút **"Sao chép các prompt lỗi"** để lưu lại danh sách này, sửa đổi và chạy lại chúng trong một phiên mới.
