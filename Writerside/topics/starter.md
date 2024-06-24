# Code compasion HSV

## Mục tiêu
Mục tiêu của plugin Code Companion HSV là hỗ trợ lập trình viên trong việc phát triển ứng dụng một cách nhanh chóng và hiệu quả bằng cách tự động hóa các tác vụ lặp đi lặp lại và cung cấp các gợi ý thông minh. Plugin này được thiết kế để nâng cao năng suất của lập trình viên, giảm thiểu lỗi và giúp họ tập trung vào các khía cạnh sáng tạo của việc phát triển phần mềm.

## Lý do sử dụng
Việc phát triển phần mềm hiện đại đòi hỏi lập trình viên phải xử lý nhiều tác vụ phức tạp và tốn thời gian. Các công việc như tạo CRUD API, viết tài liệu, và tạo commit message thường chiếm nhiều thời gian mà đáng lẽ có thể dùng để giải quyết các vấn đề kỹ thuật khó hơn. Code Companion HSV được tạo ra để giải quyết vấn đề này bằng cách tự động hóa các công việc này và cung cấp các gợi ý thông minh, từ đó giúp lập trình viên làm việc hiệu quả hơn và giảm thiểu lỗi phát sinh.

## Ý tưởng
### Giải quyết các vấn đề mà GitHub Copilot và các công cụ khác chưa giải quyết

1. Tùy chỉnh cho từng kiến trúc phần mềm
- GitHub Copilot và các công cụ tương tự thường không cho phép tùy chỉnh cụ thể cho từng kiến trúc phần mềm. Code Companion HSV cho phép tùy chỉnh prompt cho từng kiến trúc như Controller, Service, Repo, giúp lập trình viên cấu hình theo nhu cầu cụ thể của dự án.
2. Hỗ trợ tự động tạo cấu trúc mã theo use case cụ thể
- Các công cụ hiện tại không cung cấp khả năng tự động tạo mã theo cấu trúc và framework cụ thể như NestJS, SpringBoot cho backend hoặc Angular, React cho frontend. Code Companion HSV giải quyết vấn đề này bằng cách cung cấp tính năng tạo CRUD API và CRUD Table theo cấu trúc có thể tùy chỉnh.
3. Tạo tài liệu tự động
- Việc viết tài liệu thường tốn thời gian và dễ bỏ sót. Code Companion HSV tự động tạo tài liệu theo cấu trúc mã, giúp đảm bảo tính nhất quán và đầy đủ của tài liệu, từ đó giúp việc bảo trì dễ dàng hơn.
4. Tích hợp AI Chat dựa trên ngữ cảnh repository
- GitHub Copilot cung cấp gợi ý mã nhưng thiếu tính năng trò chuyện AI để giải quyết các vấn đề ngữ cảnh trong repository. Code Companion HSV cung cấp tính năng AI Chat, giúp lập trình viên đặt câu hỏi và nhận câu trả lời dựa trên ngữ cảnh của mã nguồn, từ đó giải quyết vấn đề một cách nhanh chóng và chính xác.
5. Tích hợp Git thông minh
- Các công cụ hiện tại không hỗ trợ tốt việc tạo commit message theo ngữ cảnh từ mã nguồn và review mã trước khi commit. Code Companion HSV cung cấp tính năng tích hợp Git thông minh, giúp đảm bảo chất lượng và tính nhất quán của mã nguồn trước khi commit.

## Chức năng
Code companion HSV plugin hỗ trợ các tính năng sau:

- **Hỗ trợ các đa ngôn ngữ lập trình** : Java, Typescript, JS,...
- **Automatic Code Generation**:
    - CRUD api: tạo code theo feature (NestJS, SpringBoot,...) theo 1 cấu trúc source có thể tùy chỉnh cấu hình sẵn
    - CRUD table: tạo code theo feature (Angular, React,...) theo 1 cấu trúc source có thể tùy chỉnh cấu hình sẵn
    - Auto document: tự động tạo document theo cấu trúc source có thể tùy chỉnh cấu hình sẵn
- **Copilot Support**
    - Giúp tự động tìm bug, giải thích bug, tạo commit message.
    - Gợi ý code theo pattern đã được định nghĩa trước đó.
- **AI Chat**
    - Trò chuyện đặt câu hỏi dựa trên ngữ cảnh từ repo
- **Customization**
    - Có thể tùy chỉnh prompt cho từng kiến trúc phần mềm, ví dụ : Controller, Service, Repo
    - Có thể tùy chỉnh server LLM, có thể tự tạo server AI và tích hợp vào plugin
    - Hỗ trợ ghi đè lên các prompt có sẵn
- **Git Integration**
    - Hỗ trợ tạo commit message theo ngữ cảnh từ code
    - Hỗ trợ review code trước khi commit

## Ngỗn ngữ lập trình sẽ được hỗ trợ

| Feature            | Java | JS/TS | Python |
|--------------------|:----:|:-----:|:------:|
| Auto generate CRUD |  ✅   |   ✅   |   ✅    |
| Copilot            |  ✅   |       |        |
| Chat with AI       |  ✅   |   ✅   |        |
| Customize          |  ✅   |       |        |
| Git                |  ✅   |       |        |

## Đối tượng sử dụng
Lập trình viên backend và frontend
