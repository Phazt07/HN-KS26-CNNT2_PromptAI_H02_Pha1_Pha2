# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 04
- **Họ tên:** Lã Đức Phát
- **Lớp:** CNTT2
- **Link repository Pha2:** https://github.com/Phazt07/HN-KS26-CNNT2_PromptAI_H02_Pha1_Pha2.git
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):** ChatGPT

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt vé xe ra JSON

**KET QUA AI**

```text
[{"ma_goi":"SVT","ngay_su_kien":"2026-12-20","nguoi_lon":2,"tre_em":1,"loai_ve":"thuong","ghi_chu":null},{"ma_goi":"FZ","ngay_su_kien":"2027-01-05","nguoi_lon":3,"tre_em":0,"loai_ve":"thuong","ghi_chu":"cần hỗ trợ xe lăn"},{"ma_goi":"VIP","ngay_su_kien":null,"nguoi_lon":4,"tre_em":0,"loai_ve":"vip","ghi_chu":"cần hỗ trợ tìm chỗ"}]
```

**Link trò chuyện:** https://chatgpt.com/s/cx_6b079d82e21c8191aa731a0715a4f9a5

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
Bước 1: Tiền vé 8 người lớn: 8 × 320.000 = **2.560.000 đồng**.

Bước 2: Mỗi trẻ em từ 5 đến 10 tuổi trả 75% giá vé người lớn: 320.000 × 75% = 240.000 đồng. Ba trẻ em trả: 3 × 240.000 = **720.000 đồng**. Bé 2 tuổi được miễn phí vì dưới 5 tuổi và ngồi cùng người lớn: **0 đồng**.

Bước 3: Tiền vé trước giảm giá: 2.560.000 + 720.000 + 0 = **3.280.000 đồng**.

Bước 4: Đoàn có 8 người lớn nên được giảm 5%: 3.280.000 × 5% = **164.000 đồng**. Tiền vé sau giảm: 3.280.000 − 164.000 = **3.116.000 đồng**.

Bước 5: Phụ thu 2 kiện hành lý cồng kềnh: 2 × 100.000 = **200.000 đồng**.

Bước 6: Tổng thanh toán: 3.116.000 + 200.000 = **3.316.000 đồng**.

[RESULT: 3.316.000 đồng]
```

**Link trò chuyện:** https://chatgpt.com/s/cx_6b079e17a5888191b06a0851fdf09722

### b) Kiểm tra kết quả DDUsKeest 

AI đúng 

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{"loai_su_co":"sai_loai_xe","so_khach":3,"so_chang_bi_doi":2,"tom_tat":"Ba khách bị đổi từ xe giường nằm sang xe ghế ngồi ở cả chặng đi và về."}
```

**Link trò chuyện:** https://chatgpt.com/s/cx_6b079f026a8881919522e9e6ada6b96d

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
| Tiêu chí | Điểm tối đa | Điểm đạt | Nhận xét |
|---|---:|---:|---|
| Đúng thông tin | 5 | 1 | “350.000đ” sai giá; giá chuẩn là 380.000 đồng/vé người lớn. “Đổi trước 12 tiếng thì đổi free” sai vì đổi từ 6 đến dưới 24 giờ mất phí 20% (76.000 đồng). Sửa: “Vé người lớn giá 380.000 đồng; đổi trước 12 tiếng mất phí 76.000 đồng.” |
| Đầy đủ | 3 | 1 | Đã trả lời về giá và phí đổi, nhưng chưa mời khách cung cấp ngày đi và số vé để đặt chỗ. Sửa: “Chị cho em xin ngày đi và số vé cần đặt để em hỗ trợ giữ chỗ nhé.” |
| Giọng điệu | 2 | 1 | “Xe xịn lắm luôn”, “Cần gì chị nhắn em liền!” suồng sã; lời mời “nha chị” lặp lại. Có thể dùng giọng chuyên nghiệp hơn: “Dạ, em sẵn sàng hỗ trợ chị đặt vé.” |
| **Tổng điểm** | **10** | **3** | |
```

**Link trò chuyện:** https://chatgpt.com/s/cx_6b079f4baa6881919a98c6d30c8ae0e5
