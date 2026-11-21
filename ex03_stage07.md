**PROMPT 1**

```text
[Context]:
Bạn là nhân viên nhân sự mới tại Công ty ABC Technology. Công ty cung cấp cho bạn một bộ tài liệu nội bộ gồm 5 chương, tổng cộng 120 trang, quy định về:

- Nội quy lao động.

- Quy định nghỉ phép.

- Chính sách làm thêm giờ.

- Quy định đánh giá nhân viên.

- Chính sách khen thưởng và kỷ luật.

Bạn cần nghiên cứu tài liệu để chuẩn bị cho buổi hướng dẫn nhân viên mới. Tuy nhiên, khi đưa toàn bộ tài liệu vào AI, hệ thống không thể xử lý hết nội dung trong một lần do giới hạn Context Window.

[Request]: Bạn hãy đọc dữ liệu có trong file docx rồi sau đó:
    1. Chia tài liệu thành các phần có nội dung logic.

    2. Tóm tắt từng phần theo cấu trúc thống nhất.

    3. Lưu lại những thông tin quan trọng sau mỗi lần xử lý.

[Explantion]:
    - Không được suy đoán những quy định không xuất hiện trong tài liệu.

    - Mỗi chương phải được xử lý riêng.

    - Phải giữ nguyên các con số, thời hạn, tỷ lệ và điều kiện trong tài liệu.

    - Không được bỏ qua các trường hợp ngoại lệ.

    - Khi tổng hợp, phải phân biệt rõ thông tin có trong tài liệu và thông tin chưa được đề cập.
    [Tone]: Chuyên nghiệp, ngắn gọn, chính xác, dể hiểu.

[Extras]: Bản tắt nội dung file docx.
```

**Chạy thử PROMPT1**

PHẦN 1: PHÂN CHIA TÀI LIỆU THEO CẤU TRÚC LOGIC

Bộ tài liệu được phân tách thành 07 khối xử lý độc lập để đảm bảo không vượt quá giới hạn xử lý và tách bạch từng chuyên đề:
1. Khối 0: Phần mở đầu & Pháp lý ban hành (Quyết định 01/2026/QĐ-ABC, Danh mục thuật ngữ).
2. Khối 1 (Chương 1): Nội quy lao động (Điều 1 – Điều 6).
3. Khối 2 (Chương 2): Quy định về Nghỉ phép & Vắng mặt (Điều 7 – Điều 11).
4. Khối 3 (Chương 3): Chính sách Làm thêm giờ – OT (Điều 12 – Điều 16).
5. Khối 4 (Chương 4): Quy định Đánh giá Hiệu suất Nhân viên (Điều 17 – Điều 21).
6. Khối 5 (Chương 5): Chính sách Khen thưởng và Kỷ luật (Điều 22 – Điều 25).
7. Khối 6 (Phụ lục 01 – 06): Ma trận phân quyền, Biểu mẫu, Khung năng lực và Bộ câu hỏi FAQ.

PHẦN 2: TÓM TẮT CHI TIẾT TỪNG CHƯƠNG (THEO CẤU TRÚC THỐNG NHẤT)


CHƯƠNG 1: NỘI QUY LAO ĐỘNG (Điều 1 – Điều 6)

• Đối tượng áp dụng: Toàn thể CBNV (thử việc, xác định thời hạn, không xác định thời hạn); thực tập sinh, cộng tác viên, chuyên gia, nhà thầu và khách đến công tác phải tuân thủ quy định về trật tự, an toàn, bảo mật.
• Quy định & Định lượng cốt lõi:
	• Thời giờ làm việc: 40 giờ/tuần (Thứ Hai – Thứ Sáu). Giờ tiêu chuẩn: Sáng 08:30 – 12:00, Nghỉ trưa 12:00 – 13:30 (không tính giờ làm), Chiều 13:30 – 18:00.
	• Giờ linh hoạt (Khối Kỹ thuật – Sản phẩm): Ca Sớm (08:00 – 17:30), Ca Tiêu chuẩn (08:30 – 18:00), Ca Muộn (09:00 – 18:30), bắt buộc có mặt trong Core Hours (09:30 – 11:30 và 14:00 – 17:00).
	• Chấm công & Ân hạn: Cho phép đi muộn tối đa 10 phút/lần, không quá 03 lần/tháng. Từ lần thứ 4 (muộn 11 đến dưới 60 phút) trừ 0,25 ngày công/lần. Muộn/về sớm từ 60 phút trở lên không phép trừ 0,5 ngày công. Giải trình quên chấm công trong 48 giờ (tối đa 02 lần/tháng).
	• Làm việc từ xa (Remote): Tối đa 02 ngày/tháng cho nhân viên chính thức; phải phản hồi tin nhắn/cuộc gọi trong 15 phút.
	• Trật tự & Trang phục: Thứ Hai – Thứ Năm mặc công sở lịch sự; Thứ Sáu mặc tự do (Casual Friday). Mất thẻ nhân viên phí cấp lại 100.000 VNĐ.
	• An toàn & Bảo mật (NDA): Khám sức khỏe định kỳ tối thiểu 01 lần/năm. NDA có hiệu lực tối thiểu 03 năm sau khi nghỉ việc. Mật khẩu tối thiểu 12 ký tự, bật MFA/2FA, đổi định kỳ 90 ngày/lần. Điều tra khiếu nại quấy rối tình dục trong 05 ngày làm việc.
• Trường hợp ngoại lệ:
	• Bộ phận vận hành ca (NOC/SOC, Technical Support) làm việc và nghỉ luân phiên theo phân ca nhưng đảm bảo nghỉ ít nhất 01 ngày (24 giờ liên tục)/tuần.
	• Cấm đi dép lê/xỏ ngón, ngoại trừ khu vực pantry hoặc khi trời mưa ngập (phải thay giày khi vào khu vực làm việc).
	• Cấm uống rượu bia tại văn phòng, ngoại trừ tiệc liên hoan chính thức được Ban Giám đốc phê duyệt.

CHƯƠNG 2: QUY ĐỊNH VỀ NGHỈ PHÉP & VẮNG MẶT (Điều 7 – Điều 11)

• Đối tượng áp dụng: Toàn thể CBNV ký hợp đồng lao động với ABC Technology (một số quyền lợi chỉ áp dụng khi đã ký hợp đồng chính thức).
• Quy định & Định lượng cốt lõi:
	• Phép năm: 12 ngày/năm (đủ 12 tháng); cộng 01 ngày mỗi 05 năm thâm niên. Làm chưa đủ 12 tháng tính theo tỷ lệ số tháng làm việc thực tế (làm tròn từ 0,5 lên 1, dưới 0,5 xuống 0). Tháng có từ 50% ngày làm việc tiêu chuẩn trở lên được tính là 01 tháng làm việc.
	• Chuyển phép: Tối đa 05 ngày sang năm sau, phải dùng hết trước ngày 31/03.
	• Nghỉ lễ, Tết: 11 ngày/năm hưởng nguyên lương.
	• Nghỉ việc riêng hưởng nguyên lương: Kết hôn (03 ngày); con đẻ/con nuôi kết hôn (01 ngày); tứ thân phụ mẫu, vợ/chồng, con mất (03 ngày).
	• Nghỉ việc riêng không lương (luật định): Ông bà nội/ngoại, anh chị em ruột mất; cha/mẹ hoặc anh chị em ruột kết hôn (01 ngày).
	• Phúc lợi riêng: 01 ngày nghỉ hưởng lương trong tháng sinh nhật (không cộng dồn).
	• Nghỉ BHXH: Nộp giấy chứng nhận nghỉ BHXH bản gốc trong 03 ngày làm việc sau khi đi làm lại. Khám thai tối đa 05 lần (01 ngày/lần). Nghỉ sinh con 06 tháng (sinh đôi trở lên thêm 01 tháng/con từ con thứ 2). Nam giới khi vợ sinh nghỉ 05 – 14 ngày làm việc tùy trường hợp; báo trước nghỉ thai sản ít nhất 30 ngày.
	• Nghỉ không hưởng lương: Tối đa 30 ngày/năm. Nghỉ từ 14 ngày làm việc/tháng trở lên không đóng BHXH và không tích lũy phép tháng đó.
	• Thời hạn báo trước trên HRIS: Nghỉ 0,5 – 01 ngày báo trước 24 giờ; nghỉ 02 – 03 ngày báo trước 03 ngày làm việc; nghỉ trên 03 ngày báo trước 05 ngày làm việc. Bàn giao công việc (Handover) bắt buộc khi nghỉ từ 02 ngày làm việc trở lên.
• Trường hợp ngoại lệ:
	• Nhân viên thử việc tích lũy 01 ngày phép/tháng nhưng chỉ được dùng sau khi ký hợp đồng chính thức; nếu không đạt thử việc không quy đổi thành tiền.
	• Người nước ngoài được nghỉ thêm 01 ngày Tết cổ truyền và 01 ngày Quốc khánh của nước họ.
	• Khám thai ở xa cơ sở y tế hoặc thai bệnh lý được nghỉ 02 ngày/lần.
	• Nghỉ đột xuất (ốm đau, tang gia) báo trước 09:00 sáng ngày nghỉ và tạo đơn bù trên HRIS trong 24 giờ.

CHƯƠNG 3: CHÍNH SÁCH LÀM THÊM GIỜ – OT (Điều 12 – Điều 16)

• Đối tượng áp dụng: CBNV thực hiện công việc ngoài giờ theo yêu cầu cấp bách được Quản lý trực tiếp phê duyệt và có sự tự nguyện của NLĐ.
• Quy định & Định lượng cốt lõi:
	• Giới hạn OT: Không quá 50% giờ làm bình thường/ngày (tổng giờ làm chính + OT không quá 12 giờ/ngày); không quá 40 giờ/tháng; không quá 200 giờ/năm.
	• Hệ số lương OT: Ngày thường (150%); Ngày nghỉ hằng tuần (200%); Ngày lễ/Tết (300%). Ban đêm (22:00 – 06:00): Đêm ngày thường (210%), Đêm ngày nghỉ tuần (270%), Đêm ngày lễ/Tết (390%).
	• Nghỉ bù (Compensatory Leave): Quy đổi theo hệ số OT tương ứng, sử dụng trong vòng 60 ngày kể từ ngày phát sinh.
	• Phụ cấp OT: Tiền ăn 80.000 VNĐ/suất (làm liên tục từ 03 giờ ngày thường hoặc từ 04 giờ ngày nghỉ/lễ). Hỗ trợ taxi/xe công nghệ khi kết thúc OT tại văn phòng sau 21:30.
	• Trực On-call (DevOps/SRE/NOC): 300.000 VNĐ/ca ngày thường; 500.000 VNĐ/ca ngày nghỉ/lễ.
	• Quy trình & Chi trả: Đăng ký trước 16:00 (ngày thường) hoặc trước 17:00 Thứ Sáu (cuối tuần). Quản lý nghiệm thu trong 02 ngày làm việc. Chốt công OT ngày 26 hằng tháng, chi trả vào ngày 05 tháng kế tiếp.
• Trường hợp ngoại lệ:
	• Trần OT năm có thể lên tới 300 giờ/năm đối với các trường hợp đặc biệt theo quy định của Chính phủ.
	• Tự ý ở lại làm việc không có OT Request duyệt trước sẽ không được tính OT, ngoại trừ xử lý sự cố khẩn cấp hệ thống Live có xác nhận của Giám đốc Kỹ thuật trong vòng 24 giờ sau đó.
	• Trực On-call tại nhà chỉ tính giờ OT chính thức (theo Điều 13) khi phát sinh xử lý sự cố thực tế từ 15 phút trở lên.

CHƯƠNG 4: QUY ĐỊNH ĐÁNH GIÁ HIỆU SUẤT NHÂN VIÊN (Điều 17 – Điều 21)

• Đối tượng áp dụng: Toàn thể CBNV trong giai đoạn thử việc và nhân viên chính thức.
• Quy định & Định lượng cốt lõi:
	• Các kỳ đánh giá: Thử việc (trước khi kết thúc ít nhất 07 ngày làm việc, thường sau 60 ngày); Giữa năm (01/07 – 15/07); Cuối năm (01/12 – 20/12); Đột xuất.
	• Trọng số đánh giá (KPI/OKR – Năng lực – Văn hóa): Quản lý (60% - 30% - 10%); Chuyên viên/Kỹ sư (70% - 20% - 10%); Khối Hỗ trợ (60% - 25% - 15%).
	• Thang xếp loại (5 cấp độ & Bell Curve):
		• S (95 – 100 điểm, tỷ lệ 5% – 10%): Tăng lương vượt khung 10% – 20%, thưởng 1,5x – 2,0x.
		• A (85 – 94 điểm, tỷ lệ 20% – 25%): Tăng lương vượt khung 10% – 20%, thưởng 1,5x – 2,0x.
		• B (70 – 84 điểm, tỷ lệ 55% – 65%): Điều chỉnh lương 5% – 8%, thưởng 1,0x.
		• C (55 – 69 điểm, tỷ lệ 5% – 10%): Không tăng lương, thưởng 0,5x, bắt buộc vào PIP.
		• D (Dưới 55 điểm, tỷ lệ 0% – 5%): Không tăng lương/thưởng, áp dụng PIP khẩn cấp hoặc xem xét chấm dứt HĐLĐ.
	• Quy trình 6 bước: Thiết lập mục tiêu (Tuần 1) \(\rightarrow \) Tự đánh giá (03 ngày) \(\rightarrow \) Đánh giá chéo 360 độ (03 – 05 đồng nghiệp, 03 ngày) \(\rightarrow \) Quản lý chấm điểm (05 ngày) \(\rightarrow \) Calibration (03 ngày) \(\rightarrow \) Phản hồi 1-1 & ký IDP (05 ngày).
	• Kế hoạch cải thiện hiệu suất (PIP): Kéo dài 30 – 60 ngày, kiểm tra tiến độ (Check-in) hằng tuần. Khiếu nại kết quả KPI trong vòng 03 ngày làm việc sau họp 1-1 (Phụ lục 06).
• Trường hợp ngoại lệ:
	• Đánh giá đột xuất áp dụng ngoài chu kỳ định kỳ khi xét bổ nhiệm/thăng chức, điều chuyển vị trí hoặc đưa vào diện PIP.

CHƯƠNG 5: CHÍNH SÁCH KHEN THƯỞNG VÀ KỶ LUẬT (Điều 22 – Điều 25)

• Đối tượng áp dụng: Toàn thể CBNV vi phạm nội quy lao động hoặc có thành tích đóng góp cho ABC Technology.
• Quy định & Định lượng cốt lõi:
	• 5 Hình thức Khen thưởng:
		1. Spot Bonus: 1.000.000 – 5.000.000 VNĐ/lần + Thư tuyên dương.
		2. Ngôi sao của Quý: 3.000.000 VNĐ + Cúp + 01 ngày phép thưởng.
		3. Xuất sắc nhất Năm: 10.000.000 – 20.000.000 VNĐ + Bảng vinh danh + Ưu tiên đào tạo quốc tế.
		4. Referral Bonus (chi sau thử việc): Junior/Middle (3.000.000 VNĐ), Senior/Lead (7.000.000 VNĐ), Manager/Architect (12.000.000 VNĐ).
		5. Thâm niên: 03 năm (3.000.000 VNĐ + Kỷ niệm chương Bạc), 05 năm (7.000.000 VNĐ + Kỷ niệm chương Vàng), 10 năm (15.000.000 VNĐ + Du lịch gia đình).
	• 3 Hình thức Kỷ luật:
		1. Khiển trách: Đi muộn/về sớm không lý do từ 05 lần/tháng; nghỉ không phép 01 ngày/tháng; sai trang phục/không đeo thẻ từ 03 lần/tháng; không khóa màn hình máy tính từ 02 lần.
		2. Kéo dài thời hạn nâng lương (tối đa 06 tháng) hoặc Cách chức: Tái phạm sau khiển trách (trong 03 tháng); nghỉ không phép 02 – 04 ngày cộng dồn trong 30 ngày; khai gian OT/chấm công hộ; cài phần mềm crack; gây thiệt hại từ 5.000.000 đến dưới 20.000.000 VNĐ.
		3. Sa thải: Trộm cắp, tham ô, đánh bạc, ma túy; tiết lộ bí mật công nghệ/kinh doanh; xâm phạm quyền sở hữu trí tuệ; quấy rối tình dục; gây thiệt hại từ 20.000.000 VNĐ trở lên hoặc làm gián đoạn dịch vụ khách hàng trên 04 giờ; tự ý bỏ việc 05 ngày cộng dồn trong 30 ngày hoặc 20 ngày cộng dồn trong 365 ngày.
	• Thời hiệu & Xóa kỷ luật: Thời hiệu xử lý tối đa 06 tháng (hoặc 12 tháng nếu liên quan tài chính, tài sản, bí mật công nghệ/kinh doanh). Gửi thông báo họp kỷ luật trước ít nhất 05 ngày làm việc. Xóa kỷ luật sau 03 tháng (Khiển trách) và 06 tháng (Kéo dài nâng lương; có thể xét giảm sau 03 tháng nếu tiến bộ).
• Trường hợp ngoại lệ:
	• Chưa được xử lý kỷ luật khi NLĐ đang nghỉ ốm đau, điều dưỡng; nghỉ việc được Công ty đồng ý; tạm giữ/tạm giam; chờ kết quả điều tra cơ quan có thẩm quyền; lao động nữ mang thai, nghỉ thai sản, nuôi con dưới 12 tháng tuổi.
	• Nếu NLĐ vắng mặt sau 03 lần thông báo hợp lệ mà không có lý do chính đáng, Công ty vẫn tiến hành họp xử lý kỷ luật.

PHẦN 3: BẢNG TỔNG HỢP DỮ LIỆU QUAN TRỌNG & ĐỐI CHIẾU THIẾU SÓT


1. Bảng lưu trữ thông số cốt lõi (Cheat-sheet cho HR Onboarding)


Nhóm chỉ số	Con số / Thời hạn chuẩn	Ghi chú áp dụng
Giờ làm việc & Core Hours	40h/tuần (08:30–18:00) | Core: 09:30–11:30 & 14:00–17:00	Nghỉ trưa 1,5 tiếng (12:00–13:30)
Ân hạn & Remote	Muộn tối đa 10 phút (03 lần/tháng) | Remote: 02 ngày/tháng	Phản hồi online trong 15 phút
Phép năm & Lễ Tết	12 ngày/năm (+1 ngày/5 năm) | Lễ Tết: 11 ngày/năm	Chuyển tối đa 05 ngày đến 31/03
Báo trước nghỉ phép	24h (≤1 ngày) | 03 ngày (2–3 ngày) | 05 ngày (>3 ngày)	Bàn giao việc khi nghỉ ≥ 02 ngày
Hệ số & Giới hạn OT	150% (Thường) | 200% (Cuối tuần) | 300% (Lễ) | Đêm: 210%/270%/390%	Trần: 12h/ngày, 40h/tháng, 200–300h/năm
Phụ cấp OT & On-call	Ăn: 80.000đ | Taxi: sau 21:30 | On-call: 300k (thường) / 500k (lễ)	Nghỉ bù OT dùng trong 60 ngày
Chu kỳ Đánh giá & PIP	Thử việc (60 ngày) | Giữa năm (01–15/07) | Cuối năm (01–20/12)	PIP kéo dài 30 – 60 ngày
Xóa kỷ luật & Thời hiệu	Thời hiệu: 06 – 12 tháng | Xóa: 03 tháng (Khiển trách), 06 tháng (Nâng lương)	Báo họp kỷ luật trước 05 ngày làm việc


2. Phân biệt rõ: Thông tin có trong tài liệu vs. Thông tin chưa được đề cập

• Thông tin ĐÃ CÓ trong tài liệu:
	• Toàn bộ cơ cấu 05 Chương (25 Điều) và 06 Phụ lục.
	• Đầy đủ định mức giờ làm việc, nghỉ phép, hệ số lương OT, trọng số đánh giá KPI/OKR, mức thưởng cụ thể và khung hình thức kỷ luật.
	• Các mẫu biểu dự phòng (Đơn nghỉ phép/OT, Biểu mẫu PIP, Biên bản vi phạm) và Khung năng lực L1–L5 cho khối Kỹ thuật, QA, PM/BA.
• Thông tin CHƯA ĐƯỢC ĐỀ CẬP trong tài liệu (HR cần lưu ý không tự ý suy đoán khi hướng dẫn nhân viên mới):
	1. Ngày ký, số hiệu chính thức và ngày có hiệu lực cụ thể: Các trường thông tin trên Quyết định ban hành hiện đang để trống (ngày ... tháng ... năm 2026).
	2. Mức lương cơ bản, phụ cấp cố định (ăn trưa, gửi xe, điện thoại) và lương tháng 13: Tài liệu chỉ nêu công thức tính đơn giá giờ OT dựa trên lương cơ bản + phụ cấp cố định nhưng không quy định mức tiền cụ thể của từng vị trí.
	3. Chính sách bảo hiểm sức khỏe tư nhân (PVI/Bảo Việt) và ngân sách đào tạo/team building: Chưa có điều khoản quy định mức chi trả bảo hiểm sức khỏe bổ sung hoặc hạn mức tài trợ khóa học/chứng chỉ cho nhân viên.
	4. Quy định về Công tác phí (trong nước và nước ngoài): Chưa nêu định mức vé máy bay, khách sạn, phụ cấp lưu trú khi nhân viên đi công tác.
	5. Thủ tục chấm dứt Hợp đồng lao động (báo trước khi nghỉ việc, quy trình bàn giao nghỉ việc chi tiết): Mới chỉ đề cập nghĩa vụ bàn giao tài sản trước ngày nghỉ việc cuối cùng tại Điều 5, chưa có điều khoản riêng về thời hạn báo trước khi đơn phương chấm dứt hợp đồng.
	6. Khung năng lực chuyên môn (Phụ lục 05) của Khối Kinh doanh (Sales/Marketing) và Khối Hỗ trợ (HCNS, Kế toán): Phụ lục 05 mới chỉ có bảng chi tiết cho Software Engineering, QA/QC và PM/BA.

**PROMPT 2**
```text
[Context]: Bạn là nhân viên nhân sự mới tại Công ty ABC Technology. Bạn được giao nhiệm vụ tóm tổng hợp dữ liệu có trong file Docx.

[Request]: Bạn hãy đọc dữ liệu có trong file .docx rồi sau đó:

    1. Tổng hợp các bản tóm tắt thành một bảng markdown.

    2. Phát hiện những nội dung có liên quan giữa các chương.

    3. Kiểm tra xem bản tổng hợp có bỏ sót thông tin quan trọng không.

[Explantion]:
    - Không được suy đoán những quy định không xuất hiện trong tài liệu.

    - Mỗi chương phải được xử lý riêng.

    - Phải giữ nguyên các con số, thời hạn, tỷ lệ và điều kiện trong tài liệu.

    - Không được bỏ qua các trường hợp ngoại lệ.

    - Khi tổng hợp, phải phân biệt rõ thông tin có trong tài liệu và thông tin chưa được đề cập.

    - Không thực hiện phần 2 và 3 trong [Request].

[Tone]: Chuyên nghiệp, ngắn gọn, chính xác, dể hiểu.

[Extras]: 
    1. Bảng Markdown chuẩn tổng hợp gồm các cột: Chủ đề, Quy định chính, Điều kiện áp dụng, Ngoại lệ.
    2. Ít nhất 5 câu hỏi kiểm tra thông tin được trích xuất từ tài liệu gốc, kèm câu trả lời và vị trí nội dung trong tài liệu.
```

**Chạy thử PROMPT 2**

# **BÁO CÁO TỔNG HỢP QUY ĐỊNH NỘI BỘ ABC TECHNOLOGY**

**Nguồn dữ liệu:** File `Tomtat.docx` (05 trang).

**Phạm vi thực hiện:**

- Đọc và tổng hợp nội dung riêng biệt của 05 chương.
- Trình bày theo bảng Markdown gồm 04 cột theo yêu cầu.
- Xây dựng câu hỏi kiểm tra, kèm đáp án và vị trí trong tài liệu.

**Lưu ý:** Theo yêu cầu, không thực hiện phần phân tích mối liên hệ giữa các chương và kiểm tra thiếu sót của bản tổng hợp.

## **I. BẢNG TỔNG HỢP NỘI DUNG 05 CHƯƠNG**

### **1. Chương 1 – Nội quy lao động (Điều 1 – Điều 6)**

| Chủ đề                 | Quy định chính                                                                                                                                                                          | Điều kiện áp dụng                                                                               | Ngoại lệ                                                                                                                          |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| Đối tượng áp dụng      | Toàn thể CBNV, thực tập sinh, cộng tác viên, chuyên gia, nhà thầu và khách đến công tác.                                                                                                | Tất cả phải tuân thủ quy định về trật tự, an toàn, bảo mật.                                     | Không nêu ngoại lệ về đối tượng.                                                                                                  |
| Thời giờ làm việc      | 40 giờ/tuần, từ thứ Hai đến thứ Sáu. Sáng 08:30–12:00; nghỉ trưa 12:00–13:30; chiều 13:30–18:00.                                                                                        | Áp dụng theo giờ làm việc tiêu chuẩn.                                                           | Bộ phận NOC/SOC, Technical Support làm việc và nghỉ luân phiên theo phân ca, bảo đảm nghỉ ít nhất 01 ngày (24 giờ liên tục)/tuần. |
| Giờ làm việc linh hoạt | Ca sớm 08:00–17:30; ca tiêu chuẩn 08:30–18:00; ca muộn 09:00–18:30.                                                                                                                     | Áp dụng cho khối Kỹ thuật – Sản phẩm. Phải có mặt trong Core Hours: 09:30–11:30 và 14:00–17:00. | Không nêu thêm.                                                                                                                   |
| Chấm công và đi muộn   | Được đi muộn tối đa 10 phút/lần, không quá 03 lần/tháng. Từ lần thứ 4 (muộn 11 đến dưới 60 phút): trừ 0,25 ngày công/lần. Muộn/về sớm từ 60 phút trở lên không phép: trừ 0,5 ngày công. | Áp dụng đối với việc chấm công và thời gian làm việc.                                           | Quên chấm công được giải trình trong 48 giờ, tối đa 02 lần/tháng.                                                                 |
| Làm việc từ xa         | Tối đa 02 ngày/tháng. Phải phản hồi tin nhắn/cuộc gọi trong 15 phút.                                                                                                                    | Nhân viên chính thức.                                                                           | Không nêu thêm.                                                                                                                   |
| Trang phục             | Thứ Hai–Thứ Năm mặc công sở lịch sự; Thứ Sáu được mặc tự do (Casual Friday). Mất thẻ nhân viên phải trả 100.000 VNĐ phí cấp lại.                                                        | Toàn thể nhân viên.                                                                             | Được đi dép lê/xỏ ngón tại pantry hoặc khi trời mưa ngập, nhưng phải thay giày khi vào khu vực làm việc.                          |
| An toàn và bảo mật     | Khám sức khỏe định kỳ tối thiểu 01 lần/năm. NDA có hiệu lực tối thiểu 03 năm sau khi nghỉ việc. Mật khẩu tối thiểu 12 ký tự, bật MFA/2FA, đổi định kỳ 90 ngày/lần.                      | Nhân viên thuộc phạm vi quy định an toàn và bảo mật.                                            | Khiếu nại quấy rối tình dục phải được điều tra trong 05 ngày làm việc.                                                            |
| Rượu bia               | Cấm uống rượu bia tại văn phòng.                                                                                                                                                        | Áp dụng tại nơi làm việc.                                                                       | Tiệc liên hoan chính thức được Ban Giám đốc phê duyệt.                                                                            |

Tomtat.docx

### **2. Chương 2 – Quy định về nghỉ phép và vắng mặt (Điều 7 – Điều 11)**

| Chủ đề                      | Quy định chính                                                                                                                                                                                                   | Điều kiện áp dụng                                                                                                                                                                | Ngoại lệ                                                                                                                                           |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| Đối tượng áp dụng           | Toàn thể CBNV ký hợp đồng lao động với ABC Technology.                                                                                                                                                           | Một số quyền lợi chỉ áp dụng khi đã ký hợp đồng chính thức.                                                                                                                      | Nhân viên thử việc có cơ chế tích lũy phép riêng.                                                                                                  |
| Phép năm                    | 12 ngày/năm khi làm đủ 12 tháng. Cộng thêm 01 ngày mỗi 05 năm thâm niên.                                                                                                                                         | Làm chưa đủ 12 tháng tính theo tỷ lệ số tháng làm việc thực tế. Làm tròn từ 0,5 lên 1, dưới 0,5 xuống 0. Tháng có từ 50% ngày làm việc tiêu chuẩn trở lên được tính là 01 tháng. | Nhân viên thử việc tích lũy 01 ngày/tháng nhưng chỉ được sử dụng sau khi ký hợp đồng chính thức. Nếu không đạt thử việc, không quy đổi thành tiền. |
| Chuyển phép                 | Được chuyển tối đa 05 ngày phép sang năm sau.                                                                                                                                                                    | Phải sử dụng hết trước ngày 31/03.                                                                                                                                               | Không nêu thêm.                                                                                                                                    |
| Nghỉ lễ, Tết                | 11 ngày/năm, hưởng nguyên lương.                                                                                                                                                                                 | Theo quy định nghỉ lễ, Tết.                                                                                                                                                      | Người nước ngoài được nghỉ thêm 01 ngày Tết cổ truyền và 01 ngày Quốc khánh của nước họ.                                                           |
| Nghỉ việc riêng hưởng lương | Kết hôn: 03 ngày; con đẻ/con nuôi kết hôn: 01 ngày; tứ thân phụ mẫu, vợ/chồng, con mất: 03 ngày.                                                                                                                 | Theo từng sự kiện cá nhân được quy định.                                                                                                                                         | Không nêu thêm.                                                                                                                                    |
| Nghỉ việc riêng không lương | Ông bà nội/ngoại, anh chị em ruột mất; cha/mẹ hoặc anh chị em ruột kết hôn: 01 ngày.                                                                                                                             | Theo các trường hợp được liệt kê.                                                                                                                                                | Không nêu thêm.                                                                                                                                    |
| Nghỉ sinh nhật              | 01 ngày nghỉ hưởng lương trong tháng sinh nhật.                                                                                                                                                                  | Áp dụng theo tháng sinh nhật của nhân viên.                                                                                                                                      | Không được cộng dồn.                                                                                                                               |
| Nghỉ BHXH                   | Nộp giấy chứng nhận nghỉ BHXH bản gốc trong 03 ngày làm việc sau khi đi làm lại. Khám thai tối đa 05 lần, mỗi lần 01 ngày. Nghỉ sinh con 06 tháng. Nam giới khi vợ sinh nghỉ 05–14 ngày làm việc tùy trường hợp. | Thực hiện theo chế độ BHXH. Phải báo trước nghỉ thai sản ít nhất 30 ngày.                                                                                                        | Sinh đôi trở lên được nghỉ thêm 01 tháng/con từ con thứ 2. Khám thai ở xa cơ sở y tế hoặc thai bệnh lý được nghỉ 02 ngày/lần.                      |
| Nghỉ không hưởng lương      | Tối đa 30 ngày/năm.                                                                                                                                                                                              | Nghỉ từ 14 ngày làm việc/tháng trở lên thì không đóng BHXH và không tích lũy phép tháng đó.                                                                                      | Nghỉ đột xuất do ốm đau, tang gia: báo trước 09:00 sáng ngày nghỉ và tạo đơn bù trên HRIS trong 24 giờ.                                            |
| Báo trước nghỉ phép         | Nghỉ 0,5–01 ngày: báo trước 24 giờ. Nghỉ 02–03 ngày: báo trước 03 ngày làm việc. Nghỉ trên 03 ngày: báo trước 05 ngày làm việc.                                                                                  | Thực hiện đăng ký trên HRIS.                                                                                                                                                     | Nghỉ đột xuất thực hiện theo quy định riêng.                                                                                                       |
| Bàn giao công việc          | Bắt buộc bàn giao công việc (Handover).                                                                                                                                                                          | Khi nghỉ từ 02 ngày làm việc trở lên.                                                                                                                                            | Không nêu thêm.                                                                                                                                    |

Tomtat.docx

### **3. Chương 3 – Chính sách làm thêm giờ (OT) (Điều 12 – Điều 16)**

| Chủ đề                | Quy định chính                                                                                                                         | Điều kiện áp dụng                                                                   | Ngoại lệ                                                                                                                                                                            |
| --------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Đối tượng áp dụng     | CBNV thực hiện công việc ngoài giờ theo yêu cầu cấp bách.                                                                              | Phải được Quản lý trực tiếp phê duyệt và có sự tự nguyện của người lao động.        | Không nêu thêm.                                                                                                                                                                     |
| Giới hạn OT           | Không quá 50% giờ làm bình thường/ngày; tổng giờ làm chính và OT không quá 12 giờ/ngày; không quá 40 giờ/tháng; không quá 200 giờ/năm. | Áp dụng theo giới hạn làm thêm giờ.                                                 | Trần OT có thể lên tới 300 giờ/năm đối với trường hợp đặc biệt theo quy định của Chính phủ.                                                                                         |
| Hệ số lương OT        | Ngày thường: 150%; ngày nghỉ hằng tuần: 200%; ngày lễ/Tết: 300%.                                                                       | Tính theo ngày thực hiện OT.                                                        | Làm ban đêm từ 22:00–06:00: ngày thường 210%; ngày nghỉ tuần 270%; ngày lễ/Tết 390%.                                                                                                |
| Nghỉ bù               | Quy đổi theo hệ số OT tương ứng.                                                                                                       | Thời gian sử dụng trong vòng 60 ngày kể từ ngày phát sinh.                          | Không nêu thêm.                                                                                                                                                                     |
| Phụ cấp OT            | Tiền ăn 80.000 VNĐ/suất. Hỗ trợ taxi/xe công nghệ khi kết thúc OT tại văn phòng sau 21:30.                                             | Tiền ăn áp dụng khi làm liên tục từ 03 giờ ngày thường hoặc từ 04 giờ ngày nghỉ/lễ. | Không nêu thêm.                                                                                                                                                                     |
| Trực On-call          | DevOps/SRE/NOC: 300.000 VNĐ/ca ngày thường; 500.000 VNĐ/ca ngày nghỉ/lễ.                                                               | Áp dụng cho nhân sự trực On-call.                                                   | Trực On-call tại nhà chỉ tính giờ OT chính thức khi phát sinh xử lý sự cố thực tế từ 15 phút trở lên.                                                                               |
| Đăng ký và nghiệm thu | Đăng ký trước 16:00 ngày thường hoặc trước 17:00 Thứ Sáu đối với cuối tuần. Quản lý nghiệm thu trong 02 ngày làm việc.                 | OT phải được đăng ký và phê duyệt.                                                  | Tự ý ở lại làm việc không có OT Request duyệt trước sẽ không được tính OT, ngoại trừ xử lý sự cố khẩn cấp hệ thống Live có xác nhận của Giám đốc Kỹ thuật trong vòng 24 giờ sau đó. |
| Chốt công và chi trả  | Chốt công OT ngày 26 hằng tháng; chi trả vào ngày 05 tháng kế tiếp.                                                                    | Theo kỳ thanh toán OT hằng tháng.                                                   | Không nêu thêm.                                                                                                                                                                     |

Tomtat.docx

### **4. Chương 4 – Quy định đánh giá hiệu suất nhân viên (Điều 17 – Điều 21)**

| Chủ đề             | Quy định chính                                                                                                                                                                                        | Điều kiện áp dụng                                     | Ngoại lệ                                                                                 |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| Đối tượng áp dụng  | Toàn thể CBNV trong giai đoạn thử việc và nhân viên chính thức.                                                                                                                                       | Áp dụng trong quá trình đánh giá hiệu suất.           | Không nêu thêm.                                                                          |
| Chu kỳ đánh giá    | Thử việc: trước khi kết thúc ít nhất 07 ngày làm việc, thường sau 60 ngày. Giữa năm: 01/07–15/07. Cuối năm: 01/12–20/12. Ngoài ra có đánh giá đột xuất.                                               | Theo từng kỳ đánh giá.                                | Đánh giá đột xuất khi xét bổ nhiệm/thăng chức, điều chuyển vị trí hoặc đưa vào diện PIP. |
| Trọng số đánh giá  | Quản lý: KPI/OKR 60%, năng lực 30%, văn hóa 10%. Chuyên viên/Kỹ sư: 70%, 20%, 10%. Khối Hỗ trợ: 60%, 25%, 15%.                                                                                        | Theo nhóm chức danh.                                  | Không nêu thêm.                                                                          |
| Xếp loại S         | 95–100 điểm; tỷ lệ 5%–10%. Tăng lương vượt khung 10%–20%; thưởng 1,5x–2,0x.                                                                                                                           | Theo thang đánh giá và Bell Curve.                    | Không nêu thêm.                                                                          |
| Xếp loại A         | 85–94 điểm; tỷ lệ 20%–25%. Tăng lương vượt khung 10%–20%; thưởng 1,5x–2,0x.                                                                                                                           | Theo thang đánh giá và Bell Curve.                    | Không nêu thêm.                                                                          |
| Xếp loại B         | 70–84 điểm; tỷ lệ 55%–65%. Điều chỉnh lương 5%–8%; thưởng 1,0x.                                                                                                                                       | Theo thang đánh giá và Bell Curve.                    | Không nêu thêm.                                                                          |
| Xếp loại C         | 55–69 điểm; tỷ lệ 5%–10%. Không tăng lương; thưởng 0,5x; bắt buộc vào PIP.                                                                                                                            | Theo thang đánh giá và Bell Curve.                    | Không nêu thêm.                                                                          |
| Xếp loại D         | Dưới 55 điểm; tỷ lệ 0%–5%. Không tăng lương/thưởng; áp dụng PIP khẩn cấp hoặc xem xét chấm dứt HĐLĐ.                                                                                                  | Theo thang đánh giá và Bell Curve.                    | Không nêu thêm.                                                                          |
| Quy trình đánh giá | 06 bước: thiết lập mục tiêu (Tuần 1); tự đánh giá (03 ngày); đánh giá chéo 360 độ (03–05 đồng nghiệp, 03 ngày); quản lý chấm điểm (05 ngày); Calibration (03 ngày); phản hồi 1-1 và ký IDP (05 ngày). | Thực hiện theo trình tự đánh giá.                     | Không nêu thêm.                                                                          |
| Kế hoạch PIP       | Kéo dài 30–60 ngày; kiểm tra tiến độ (Check-in) hằng tuần.                                                                                                                                            | Áp dụng cho nhân viên thuộc diện cải thiện hiệu suất. | Khiếu nại kết quả KPI trong vòng 03 ngày làm việc sau họp 1-1, theo Phụ lục 06.          |

Tomtat.docx

### **5. Chương 5 – Chính sách khen thưởng và kỷ luật (Điều 22 – Điều 25)**

| Chủ đề                                     | Quy định chính                                                                                                                                                                                                                                                  | Điều kiện áp dụng                                                                                                                                                                              | Ngoại lệ                                                                                                            |
| ------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| Đối tượng áp dụng                          | Toàn thể CBNV có thành tích đóng góp hoặc vi phạm nội quy lao động.                                                                                                                                                                                             | Theo kết quả công việc và hành vi vi phạm.                                                                                                                                                     | Không nêu thêm.                                                                                                     |
| Spot Bonus                                 | 1.000.000–5.000.000 VNĐ/lần + Thư tuyên dương.                                                                                                                                                                                                                  | Theo hình thức khen thưởng Spot Bonus.                                                                                                                                                         | Không nêu thêm.                                                                                                     |
| Ngôi sao của Quý                           | 3.000.000 VNĐ + Cúp + 01 ngày phép thưởng.                                                                                                                                                                                                                      | Theo hình thức khen thưởng Ngôi sao của Quý.                                                                                                                                                   | Không nêu thêm.                                                                                                     |
| Xuất sắc nhất Năm                          | 10.000.000–20.000.000 VNĐ + Bảng vinh danh + Ưu tiên đào tạo quốc tế.                                                                                                                                                                                           | Theo hình thức khen thưởng Xuất sắc nhất Năm.                                                                                                                                                  | Không nêu thêm.                                                                                                     |
| Referral Bonus                             | Junior/Middle: 3.000.000 VNĐ; Senior/Lead: 7.000.000 VNĐ; Manager/Architect: 12.000.000 VNĐ.                                                                                                                                                                    | Chi trả sau khi ứng viên được giới thiệu hoàn thành thử việc.                                                                                                                                  | Không nêu thêm.                                                                                                     |
| Thưởng thâm niên                           | 03 năm: 3.000.000 VNĐ + Kỷ niệm chương Bạc. 05 năm: 7.000.000 VNĐ + Kỷ niệm chương Vàng. 10 năm: 15.000.000 VNĐ + Du lịch gia đình.                                                                                                                             | Theo số năm thâm niên.                                                                                                                                                                         | Không nêu thêm.                                                                                                     |
| Khiển trách                                | Đi muộn/về sớm không lý do từ 05 lần/tháng; nghỉ không phép 01 ngày/tháng; sai trang phục/không đeo thẻ từ 03 lần/tháng; không khóa màn hình máy tính từ 02 lần.                                                                                                | Các hành vi vi phạm được liệt kê.                                                                                                                                                              | Không nêu thêm.                                                                                                     |
| Kéo dài thời hạn nâng lương hoặc cách chức | Kéo dài thời hạn nâng lương tối đa 06 tháng hoặc cách chức.                                                                                                                                                                                                     | Tái phạm sau khiển trách trong 03 tháng; nghỉ không phép 02–04 ngày cộng dồn trong 30 ngày; khai gian OT/chấm công hộ; cài phần mềm crack; gây thiệt hại từ 5.000.000 đến dưới 20.000.000 VNĐ. | Không nêu thêm.                                                                                                     |
| Sa thải                                    | Áp dụng đối với các hành vi nghiêm trọng: trộm cắp, tham ô, đánh bạc, ma túy; tiết lộ bí mật công nghệ/kinh doanh; xâm phạm quyền sở hữu trí tuệ; quấy rối tình dục; gây thiệt hại từ 20.000.000 VNĐ trở lên hoặc làm gián đoạn dịch vụ khách hàng trên 04 giờ. | Tự ý bỏ việc 05 ngày cộng dồn trong 30 ngày hoặc 20 ngày cộng dồn trong 365 ngày cũng thuộc trường hợp được liệt kê.                                                                           | Không nêu thêm về các hành vi vi phạm thuộc nhóm này.                                                               |
| Thời hiệu xử lý kỷ luật                    | Tối đa 06 tháng; 12 tháng nếu liên quan tài chính, tài sản, bí mật công nghệ/kinh doanh. Gửi thông báo họp kỷ luật trước ít nhất 05 ngày làm việc.                                                                                                              | Theo thời hiệu và quy trình xử lý kỷ luật.                                                                                                                                                     | Không nêu thêm.                                                                                                     |
| Xóa kỷ luật                                | Khiển trách: sau 03 tháng. Kéo dài nâng lương: sau 06 tháng.                                                                                                                                                                                                    | Theo thời gian chấp hành kỷ luật.                                                                                                                                                              | Có thể xét giảm thời hạn kéo dài nâng lương sau 03 tháng nếu tiến bộ.                                               |
| Tạm hoãn xử lý kỷ luật                     | Chưa xử lý khi NLĐ đang nghỉ ốm đau, điều dưỡng; nghỉ việc được Công ty đồng ý; tạm giữ/tạm giam; chờ kết quả điều tra của cơ quan có thẩm quyền; lao động nữ mang thai, nghỉ thai sản hoặc nuôi con dưới 12 tháng tuổi.                                        | Trong các trường hợp được liệt kê.                                                                                                                                                             | Nếu NLĐ vắng mặt sau 03 lần thông báo hợp lệ mà không có lý do chính đáng, Công ty vẫn tiến hành họp xử lý kỷ luật. |

Tomtat.docx

## **II. CÂU HỎI KIỂM TRA THÔNG TIN TRÍCH XUẤT**

Dưới đây là 10 câu hỏi kiểm tra kiến thức, được xây dựng dựa trên nội dung của 05 chương trong tài liệu.

### **Câu 1 – Nội quy lao động**

**Hỏi:** Nhân viên thuộc khối Kỹ thuật – Sản phẩm phải có mặt trong những khung giờ Core Hours nào?

**Trả lời:**

- Buổi sáng: 09:30–11:30.
- Buổi chiều: 14:00–17:00.

**Vị trí:** Chương 1, Điều 1–Điều 6, trang 1.

### **Câu 2 – Nội quy lao động**

**Hỏi:** Nhân viên chính thức được làm việc từ xa tối đa bao nhiêu ngày mỗi tháng và phải phản hồi liên lạc trong thời gian bao lâu?

**Trả lời:** Tối đa 02 ngày/tháng và phải phản hồi tin nhắn/cuộc gọi trong 15 phút.

**Vị trí:** Chương 1, trang 1.

### **Câu 3 – Nghỉ phép**

**Hỏi:** Nhân viên làm đủ 12 tháng được hưởng bao nhiêu ngày phép năm? Có thể chuyển tối đa bao nhiêu ngày sang năm sau?

**Trả lời:** Được hưởng 12 ngày phép/năm và được chuyển tối đa 05 ngày sang năm sau. Phải sử dụng hết trước ngày 31/03.

**Vị trí:** Chương 2, Điều 7–Điều 11, trang 2.

### **Câu 4 – Nghỉ phép**

**Hỏi:** Nhân viên nghỉ phép 02–03 ngày phải báo trước bao lâu?

**Trả lời:** Phải báo trước 03 ngày làm việc trên HRIS.

**Vị trí:** Chương 2, trang 2.

### **Câu 5 – Làm thêm giờ**

**Hỏi:** Giới hạn làm thêm giờ thông thường của nhân viên là bao nhiêu giờ/ngày, tháng và năm?

**Trả lời:**

- Không quá 50% giờ làm bình thường/ngày.
- Tổng giờ làm chính và OT không quá 12 giờ/ngày.
- Không quá 40 giờ/tháng.
- Không quá 200 giờ/năm.

Trường hợp đặc biệt theo quy định của Chính phủ có thể lên tới 300 giờ/năm.

**Vị trí:** Chương 3, Điều 12–Điều 16, trang 2–3.

### **Câu 6 – Làm thêm giờ**

**Hỏi:** Hệ số tính lương OT vào ngày thường, ngày nghỉ hằng tuần và ngày lễ/Tết là bao nhiêu?

**Trả lời:**

- Ngày thường: 150%.
- Ngày nghỉ hằng tuần: 200%.
- Ngày lễ/Tết: 300%.

Nếu làm ban đêm từ 22:00–06:00, hệ số tương ứng là 210%, 270% và 390%.

**Vị trí:** Chương 3, trang 2.

### **Câu 7 – Đánh giá hiệu suất**

**Hỏi:** Nhân viên được xếp loại B có khoảng điểm, tỷ lệ và chế độ thưởng như thế nào?

**Trả lời:**

- Điểm: 70–84.
- Tỷ lệ: 55%–65%.
- Điều chỉnh lương: 5%–8%.
- Thưởng: 1,0x.

**Vị trí:** Chương 4, Điều 17–Điều 21, trang 3.

### **Câu 8 – Đánh giá hiệu suất**

**Hỏi:** Kế hoạch cải thiện hiệu suất PIP kéo dài bao lâu và được kiểm tra tiến độ với tần suất như thế nào?

**Trả lời:** PIP kéo dài 30–60 ngày và được kiểm tra tiến độ hằng tuần.

**Vị trí:** Chương 4, trang 3.

### **Câu 9 – Khen thưởng**

**Hỏi:** Nhân viên có thâm niên 05 năm được nhận phần thưởng gì?

**Trả lời:** Nhận 7.000.000 VNĐ và Kỷ niệm chương Vàng.

**Vị trí:** Chương 5, Điều 22–Điều 25, trang 4.

### **Câu 10 – Kỷ luật lao động**

**Hỏi:** Thời hiệu xử lý kỷ luật lao động thông thường là bao lâu? Trường hợp liên quan tài chính, tài sản hoặc bí mật công nghệ/kinh doanh là bao lâu?

**Trả lời:**

- Thông thường: tối đa 06 tháng.
- Liên quan tài chính, tài sản hoặc bí mật công nghệ/kinh doanh: tối đa 12 tháng.

**Vị trí:** Chương 5, trang 4.

