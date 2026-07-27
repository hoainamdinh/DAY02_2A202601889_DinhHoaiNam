# 03 — Individual Reflection

> **Học viên:** Đinh Hoài Nam  
> **Mã học viên:** 2A202601889  
> **Vai trò trong nhóm:** Main Author  

---

## 1. Tôi đã tham gia vào phần nào trong nhóm?

| Hoạt động | Tôi đã làm gì? | Kết quả / Ảnh hưởng |
|---|---|---|
| **Scan cá nhân** | Scan 10 vấn đề từ trải nghiệm học tập, thực tập và quan sát thực tế (Kế toán, Sales, HR, BA,...). | Đưa ra danh sách 10 bài toán đa dạng góc nhìn, giúp nhóm có nhiều lựa chọn đầu vào. |
| **Pitch Problem Card** | Trình bày Top 3 bài toán cá nhân, tập trung pitch bài toán "HR Recruiter gom CV rải rác & sàng lọc CV đa nguồn". | Thuyết phục nhóm thấy rõ nỗi đau thực tế (mất 4-5 tiếng mở rải rác 3-5 tab ATS TopCV, LinkedIn, ITViec). |
| **Challenge bài của bạn khác** | Thảo luận & phản biện bài toán "Tự động hóa Review Pull Request GitHub": Đặt câu hỏi về sự sai lệch giữa tài liệu README với codebase dự án thực tế và ranh giới Workflow xử lý. | Giúp nhóm nhận ra bài toán PR Review đòi hỏi hiểu ngữ cảnh codebase phức tạp, khó kiểm soát rủi ro nếu AI duyệt sai logic, từ đó đồng thuận hội tụ về bài toán HR. |
| **Chọn candidate problem** | Đóng góp bộ tiêu chí chấm điểm (Actor, Workflow, Impact, Viability) để lựa chọn bài toán HR. | Bài toán HR được chọn với số điểm cao nhất (33/35 điểm). |
| **Validation / Research** | Thực hiện phỏng vấn nhanh 2 HR Recruiters và tổng hợp research về các giải pháp ATS/AI hiện có (Base HR, Pythia). | Phát hiện tín hiệu quan trọng: HR không muốn AI tự gửi mail từ chối ➔ Bổ sung Boundary "Human-in-the-loop". |
| **Workflow nhóm** | Vẽ sơ đồ Mermaid cho Current State và Future State cùng bảng đo lường tác động. | Chỉ rõ Bottleneck ở bước mở rải rác 3-5 tab ATS và bước sàng lọc CV & gõ Excel thủ công, làm nổi bật hiệu quả giảm >85% thời gian của AI. |
| **Problem Statement** | Xây dựng bản draft v0 và tinh chỉnh lên bản v1 (đầy đủ Actor, Workflow, Bottleneck, Metric, Boundary). | Xác định chính xác Success Metric (rút ngắn xuống 43 phút, 85% tỉ lệ chấp nhận) và Boundary an toàn. |
| **Rule / Workflow / Agent** | Phân tích bài toán trên Ma trận độ phù hợp AI và so sánh 4 mức (No AI, Rule, Workflow, Agent). | Thuyết phục nhóm chọn **AI Workflow** vì luồng xử lý cố định, tránh sa lầy vào việc dùng Agent phức tạp. |
| **Decision** | Tổng hợp checklist tiêu chí và chốt quyết định **GO**. | Đi đến quyết định GO có căn cứ lập luận chặt chẽ và lộ trình Pilot rõ ràng. |

## 2. Nhật ký sử dụng AI trong buổi Lab (AI Reflection)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| **Scan** | Gợi ý thêm các lăng kính bài toán trong doanh nghiệp (Sales, HR, DE). | Mở rộng danh sách các vai trò thực tế ngoài môi trường sinh viên. | Gợi ý một số bài toán quá chung chung như "Trợ lý AI quản lý công việc". | Lọc bỏ các ý chung chung, bổ sung dấu hiệu thật (mất bao nhiêu giờ, hậu quả gì). |
| **Problem Card** | Phản biện Problem Card bài toán HR dưới góc nhìn Skeptical PM. | Chỉ ra điểm yếu: chưa làm nổi bật nỗi đau phải chuyển đổi qua lại giữa nhiều tab ATS. | AI gợi ý để AI tự động gửi mail luôn cho ứng viên. | Bổ sung chi tiết "mở 3-5 tab TopCV/LinkedIn" và giữ nguyên việc HR duyệt mail thủ công. |
| **Workflow** | Chuyển đổi mô tả quy trình dạng văn bản thành sơ đồ Mermaid chuẩn. | Tạo khung sơ đồ Mermaid nhanh chóng, chuẩn cú pháp syntax. | Đôi khi AI gom gộp bước review của HR làm một với bước chạy AI. | Tách riêng bước AI (tự động) và bước HR Review (Human boundary) thành 2 block riêng biệt. |
| **Research** | Tìm kiếm 2-3 công cụ ATS và giải pháp AI hiện có trên thị trường. | Tìm nhanh được thông tin về Base HR, Pythia AI và Zapier Workflow. | AI đưa ra một số con số thống kê thị trường không rõ nguồn gốc (hallucination). | Xóa bỏ các số liệu vô căn cứ, chỉ giữ lại các case study và link công cụ verified được. |
| **Problem Statement** | Đặt câu hỏi phản biện cho Problem Statement v0. | Phát hiện ra Success Metric ban đầu ("tăng hiệu quả") còn mơ hồ, chưa đo được. | AI cố tình viết lại toàn bộ Problem Statement theo style văn phong bóng bẩy. | Tự giữ nguyên cấu trúc, chỉ cập nhật Metric bằng số liệu cụ thể (360 phút ➔ 43 phút). |
| **Rule/Workflow/Agent** | So sánh rủi ro giữa việc dùng Rule vs Workflow vs Agent. | Phân tích rõ ràng rủi ro khi dùng Agent tự trị (bias, mất kiểm soát). | AI có xu hướng khuyên nên dựng Agent hoành tráng để "ngầu" hơn. | Kiên quyết giữ quyết định chọn mức **Workflow**, vì rủi ro của Agent trong tuyển dụng là quá lớn. |
| **Decision** | Kiểm tra tính logic của checklist chốt decision. | Gợi ý khung checklist 6 câu hỏi kiểm chứng toàn diện. | AI khuyên Go ngay mà không đưa ra điều kiện Pilot. | Bổ sung phạm vi thử nghiệm nhỏ (Pilot với 20 CV) trước khi triển khai diện rộng. |

---

## 3. Phản tư sâu (Reflection câu hỏi mở)

### ❓ Tôi học được gì khi nghe Top 3 Problems của các bạn khác?
Khi nghe các bạn trong nhóm pitch bài toán của mình (chẳng hạn như bài toán *"Tự động hóa Review Pull Request trên GitHub"*), tôi đã tích cực đặt câu hỏi phản biện: **Làm sao AI có thể review PR chính xác khi tài liệu README của dự án thường xuyên bị sai lệch hoặc trôi so với codebase thực tế? Workflow hiện tại có thực sự cho phép AI duyệt merge tự động không?** Điều này giúp tôi hiểu sâu sắc nguyên tắc: **"Problem First, Not AI First"** — phải nhìn kỹ quy trình, độ mờ của dữ liệu đầu vào và ranh giới kiểm soát rủi ro trước khi vội vã nghĩ đến giải pháp AI.

### ❓ Nhóm có lúc nào bị Solution-First không?
Có. Ở giai đoạn đầu Phase 3, một số thành viên trong nhóm lập tức đề xuất "Xây một con AI Agent tự động đi tìm ứng viên và nhắn tin mời phỏng vấn". Lúc đó, cả nhóm đã bị thu hút bởi sự tiện lợi của công nghệ Agent. Tuy nhiên, sau khi quay lại phân tích Workflow và rủi ro (Boundary), nhóm nhận ra HR thực tế rất sợ AI gửi tin nhắn sai hoặc loại nhầm ứng viên giỏi. Việc quay lại phân tích điểm nghẽn thực sự đã giúp nhóm kéo mình ra khỏi cái bẫy "Solution-first".

### ❓ Điều khó nhất khi viết Problem Statement là gì?
Điều khó nhất là viết phần **Success Metric** và **Boundary**. Ban đầu, nhóm tôi chỉ viết chung chung là "giúp HR tiết kiệm thời gian" hoặc "chọn ứng viên chính xác hơn". Khi bị bắt buộc phải định lượng, nhóm phải ngồi tính toán từng phút cho từng bước trong workflow (từ 360 phút xuống 43 phút) và đặt ra con số >85% tỉ lệ HR chấp nhận đề xuất. Việc thiết lập Boundary (AI không được tự loại ứng viên, không tự gửi mail) cũng đòi hỏi sự thấu hiểu sâu sắc về mặt vận hành thực tế.

### ❓ Tôi đóng góp gì thật sự vào artifact cuối cùng?
Vì bài toán được chọn do bản thân tôi đề xuất, tôi là người trực tiếp định hướng nhóm tập trung vào bài toán HR có nỗi đau thực tế cao, dẫn dắt các bước thực hiện. Tôi cũng là người trực tiếp tổng hợp nội dung, vẽ sơ đồ Workflow Mermaid và viết báo cáo nhóm và thiết kế slide.

### ❓ Nếu làm lại, tôi sẽ đổi gì?
Nếu được làm lại lab này, tôi sẽ dành nhiều thời gian hơn ở Phase 4 để chuẩn bị sẵn một bộ câu hỏi phỏng vấn sâu hơn cho HR về các trường hợp ứng viên nộp CV dạng ảnh hoặc CV có trình bày phức tạp. Điều này sẽ giúp phần đánh giá rủi ro kỹ thuật của AI Workflow trong bài báo cáo trở nên sắc bén hơn nữa.

