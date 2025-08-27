
## **Hướng dẫn Sử dụng WhiskFlow**

### **Giới thiệu**

**WhiskFlow** là một tiện ích mở rộng cho trình duyệt Chrome, được thiết kế để tự động hóa hoàn toàn quy trình làm việc với công cụ tạo ảnh Whisk của Google. Thay vì phải sao chép và dán thủ công từng prompt, WhiskFlow cho phép bạn xử lý hàng trăm prompt một cách tự động, giúp bạn tiết kiệm thời gian và giải phóng sức sáng tạo.

Tiện ích này lý tưởng cho các nghệ sĩ, nhà thiết kế, và bất kỳ ai cần tạo ra số lượng lớn hình ảnh để thử nghiệm ý tưởng hoặc xây dựng dữ liệu.

---

### **Tổng quan Giao diện**



Giao diện của WhiskFlow được chia thành các khu vực chính:

1.  **📝 Danh sách prompt:** Nơi bạn nhập hoặc dán danh sách các prompt cần chạy. Bạn cũng có thể nhập từ file `.txt`.
2.  **Các nút điều khiển chính:**
    * `▶️ Bắt đầu / Tiếp tục`: Bắt đầu quy trình hoặc tiếp tục sau khi tạm dừng.
    * `⏸️ Tạm dừng`: Tạm ngưng quy trình đang chạy.
    * `⏹️ Dừng`: Chấm dứt hoàn toàn quy trình.
3.  **Khu vực Trạng thái:**
    * **Thanh tiến trình:** Hiển thị tiến độ tổng thể của tác vụ.
    * **Trạng thái trực tiếp:** Hiển thị hành động đang được thực hiện (ví dụ: "Đang xử lý prompt 5/100...").
4.  **Các mục chi tiết:**
    * `⚙️ Cài đặt`: Nơi tùy chỉnh tất cả các thông số cho phiên làm việc.
    * `📄 Log chi tiết`: Ghi lại nhật ký từng bước của quá trình tự động hóa, giúp bạn dễ dàng theo dõi.
    * `⚠️ Prompt lỗi`: Liệt kê các prompt không thực thi thành công để bạn có thể sao chép và kiểm tra lại.

---

### **Hướng dẫn Bắt đầu Nhanh (3 Bước)**

1.  **Chuẩn bị:** Mở trang làm việc của **Google Whisk** (`https://labs.google/fx/vi/tools/whisk`). Chuẩn bị sẵn danh sách prompt của bạn (mỗi prompt một dòng).
2.  **Cài đặt:** Mở tiện ích WhiskFlow, dán danh sách prompt vào ô **"Danh sách prompt"**. Mở mục **"Cài đặt"** và chọn chế độ bạn muốn.
3.  **Chạy:** Nhấn nút `▶️ Bắt đầu` và để WhiskFlow tự động làm việc!

---

### **Giải thích Chi tiết các Tính năng Cài đặt**

WhiskFlow cung cấp hai chế độ hoạt động chính, mỗi chế độ có tùy chỉnh riêng để phù hợp với nhu-cầu của bạn.

#### **Cài đặt Chế độ Siêu nhanh**

Đây là chế độ được thiết kế cho tốc độ tối đa, hoạt động như một cuộc chạy nước rút.
* **Khi nào nên dùng?** Khi bạn cần thử nghiệm nhanh hàng loạt ý tưởng, tạo dữ liệu thô, hoặc không có nhu cầu tải ảnh về ngay lập tức.
* **Bật chế độ siêu nhanh:** Tích vào ô này để kích hoạt. Khi bật, **tính năng tự động tải ảnh sẽ bị vô hiệu hóa**.
* **Thời gian chờ (giây):** Đây là khoảng thời gian (tính bằng giây) mà tool sẽ chờ sau khi gửi một prompt trước khi gửi prompt tiếp theo. Thời gian này đã bao gồm cả việc kiểm tra lỗi.

#### **Cài đặt Chế độ Thường**

Đây là chế độ ổn định, được thiết kế cho các phiên làm việc cần độ tin cậy và lưu trữ kết quả, hoạt động như một cuộc chạy marathon.
* **Khi nào nên dùng?** Khi bạn muốn chạy một danh sách prompt dài và cần tất cả các ảnh được tự động tải về máy.
* **Thời gian chờ ngẫu nhiên (giây):** Để mô phỏng hành vi của người dùng và tăng tính ổn định, tool sẽ chờ một khoảng thời gian ngẫu nhiên giữa hai giá trị bạn đặt (tối thiểu và tối đa) trước khi xử lý prompt tiếp theo.
* **Tự động tải ảnh:** Tích vào ô này để WhiskFlow tự động nhấn nút tải về mỗi khi ảnh được tạo xong.

#### **Cài đặt Chung**

Các tùy chọn này áp dụng cho cả hai chế độ.
* **Thực thi mỗi prompt:** Cho phép bạn chạy mỗi prompt nhiều hơn một lần. Ví dụ, nếu bạn đặt là `3`, mỗi prompt trong danh sách sẽ được chạy lặp lại 3 lần trước khi chuyển sang prompt tiếp theo. Rất hữu ích để khám phá các biến thể của cùng một ý tưởng.
* **Bắt đầu từ prompt:** Nếu quy trình bị lỗi hoặc bạn muốn chạy lại từ một vị trí cụ thể, hãy điền số thứ tự của prompt bạn muốn bắt đầu.
* **Ngôn ngữ (Language):** Chuyển đổi giao diện giữa Tiếng Việt và Tiếng Anh.

---

### **Mẹo và Thủ thuật để có Trải nghiệm Tốt nhất**

* **Tắt "Hỏi vị trí lưu file":** Để tính năng tự động tải ảnh hoạt động mượt mà nhất, bạn nên vào phần cài đặt của trình duyệt (`chrome://settings/downloads`) và tắt tùy chọn **"Ask where to save each file before downloading"**.
* **Chạy trong cửa sổ riêng:** Để tăng sự ổn định, bạn nên chạy tab Whisk và tiện ích trong một cửa sổ trình duyệt riêng, không bị ảnh hưởng bởi các tác vụ khác.
* **Sử dụng Log:** Nếu có lỗi xảy ra, mục **"Log chi tiết"** và **"Prompt lỗi"** là những công cụ hữu ích nhất để bạn tìm ra nguyên nhân.
* **Lỗi không click được icon:** Icon của tiện ích chỉ có thể được nhấn khi bạn đang truy cập vào một trang của Google Labs (`labs.google`). Nếu bạn đang ở trang khác, icon sẽ bị mờ đi.
***
## **WhiskFlow User Guide**

### **Introduction**

**WhiskFlow** is a Chrome browser extension designed to fully automate your workflow with Google's Whisk image generation tool. Instead of manually copying and pasting every single prompt, WhiskFlow allows you to process hundreds of prompts automatically, helping you save time and unleash your creativity.

This extension is ideal for artists, designers, and anyone who needs to generate a large number of images for testing ideas or building datasets.

---

### **Interface Overview**



The WhiskFlow interface is divided into several main areas:

1.  **📝 Prompt List:** Where you type or paste the list of prompts to be processed. You can also import from a `.txt` file.
2.  **Main Control Buttons:**
    * `▶️ Start / Resume`: Begins the process or resumes after pausing.
    * `⏸️ Pause`: Pauses the currently running process.
    * `⏹️ Stop`: Completely terminates the process.
3.  **Status Area:**
    * **Progress Bar:** Displays the overall progress of the task.
    * **Live Status:** Shows the action currently being performed (e.g., "Processing prompt 5/100...").
4.  **Details Sections:**
    * `⚙️ Settings`: Where you customize all parameters for your session.
    * `📄 Detailed Log`: Records a step-by-step log of the automation process, making it easy to track.
    * `⚠️ Failed Prompts`: Lists any prompts that failed to execute, allowing you to copy and review them.

---

### **Quick Start Guide (3 Steps)**

1.  **Prepare:** Open a **Google Whisk** project page (`https://labs.google/..../whisk`). Have your list of prompts ready (one prompt per line).
2.  **Setup:** Open the WhiskFlow extension, paste your prompt list into the **"Prompt List"** text area. Open the **"Settings"** section and choose your desired mode.
3.  **Run:** Click the `▶️ Start` button and let WhiskFlow do the work for you!

---

### **Detailed Explanation of Settings**

WhiskFlow offers two main operating modes, each with its own customizations to fit your needs.

#### **Super-Fast Mode Settings**

This mode is designed for maximum speed, like a sprint.
* **When to use it?** When you need to rapidly test batches of ideas, generate raw data, or do not need to download the images immediately.
* **Enable Super-Fast Mode:** Check this box to activate. When enabled, the **auto-download feature will be disabled**.
* **Wait Time (s):** This is the amount of time (in seconds) the tool will wait after submitting one prompt before sending the next one. This duration includes the time for error checking.

#### **Normal Mode Settings**

This is the stable mode, designed for sessions that require reliability and saved results, like a marathon.
* **When to use it?** When you want to run a long list of prompts and need all the generated images to be automatically downloaded to your computer.
* **Random wait time (s):** To simulate human behavior and increase stability, the tool will wait for a random duration between the two values you set (min and max) before processing the next prompt.
* **Auto-download images:** Check this box to have WhiskFlow automatically click the download button as soon as an image is generated.

#### **General Settings**

These options apply to both modes.
* **Runs per prompt:** Allows you to execute each prompt more than once. For example, if you set it to `3`, each prompt in your list will be run 3 times before moving to the next one. This is very useful for exploring variations of the same idea.
* **Start from prompt:** If the process fails or you want to restart from a specific point, enter the number of the prompt you wish to begin with.
* **Language:** Switch the interface between Vietnamese and English.

---

### **Tips and Tricks for the Best Experience**

* **Disable "Ask where to save...":** For the auto-download feature to work seamlessly, it's highly recommended to go into your browser's settings (`chrome://settings/downloads`) and turn off the option **"Ask where to save each file before downloading"**.
* **Run in a Separate Window:** To increase stability, you should run the Whisk tab and the extension in a separate browser window, free from the interference of other tasks.
* **Use the Logs:** If an error occurs, the **"Detailed Log"** and **"Failed Prompts"** sections are the most useful tools for diagnosing the cause.
* **Extension Icon is Unclickable?:** The extension's icon can only be clicked when you are on a Google Labs page (`labs.google`). If you are on another website, the icon will be grayed out.
