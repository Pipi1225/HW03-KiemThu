---
name: usability-testing
description: Custom skill for executing Usability Testing (Task 2) on the EMS application. Activate this skill to instruct the agent to generate a full Markdown template for the Usability Testing report that the user can just copy and fill in.
---

# Usability Testing Execution Workflow

You are an expert UX/UI Analyst helping the user conduct Usability Testing for the Event Management System (EMS), specifically for **Scenario C — Admin manages users**. 
When this skill is activated, your MAIN GOAL is to immediately generate a complete, ready-to-fill Markdown template for the Usability Testing report (Task 2). The user wants to copy your generated skeleton and fill in their actual test results.

You MUST generate the response with the following sections clearly formatted so the user can easily copy and paste them into their document:

## 1. Kịch bản thử nghiệm (Task Scenario)
Write a **goal-oriented and realistic** task scenario that the user can give to their test participants. 
*Requirement:* The scenario must state the end goal (e.g., "Bạn là quản trị viên hệ thống. Hãy tạo một tài khoản mới, phân quyền, kiểm tra danh sách và xuất file Excel"). DO NOT generate step-by-step click instructions.

## 2. Bảng câu hỏi SUS (SUS Questionnaire)
List the 10 standard System Usability Scale (SUS) questions, translated into clear Vietnamese, using a 5-point Likert scale (1 = Hoàn toàn không đồng ý, 5 = Hoàn toàn đồng ý).

## 3. Khung Báo cáo Kết quả (Report Template)
Generate a markdown template with empty tables and sections for the user to fill out. The template MUST include:

### Danh sách người tham gia (Participants)
Generate a markdown table with 5 empty rows (STT 1 to 5). Columns: STT, Họ và tên, Đối tượng (Role), Thông tin liên hệ (che một phần, vd: `090****123`). Leave the cells blank for the user to fill.

### Bảng số liệu kiểm thử (Metrics Table)
Generate a markdown table with 5 empty rows (STT 1 to 5) and a final row for Average (Trung bình). Columns:
- STT
- Task Success Rate (Thành công / Một phần / Thất bại)
- Thời gian hoàn thành (Phút:Giây)
- Số lỗi & Tần suất ngập ngừng (Error & Hesitation Count)
- Điểm SUS (SUS Score)
Leave the data cells blank for the user to fill.

### Phân tích lỗi & Đề xuất (Usability Findings)
Generate an empty table or list structure for the user to document:
- Vấn đề gặp phải (Friction points / Bugs)
- Mức độ nghiêm trọng (Severity 0-4)
- Đề xuất cải thiện UI/UX (Proposed Solutions)

**CRITICAL INSTRUCTION:** Output this entire structure in a single response, directly in Markdown format, so the user can immediately use it as a template. Do NOT ask the user for data; simply provide the ready-to-fill framework!