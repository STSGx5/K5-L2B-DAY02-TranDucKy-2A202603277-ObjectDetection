# Mini guideline — bài làm cá nhân

> Điền nội dung này trước khi bắt đầu gán nhãn. Giữ lại các quyết định sau khi self-QC.

## Định nghĩa lớp

| Lớp | Định nghĩa của bạn | Ví dụ/điểm phân biệt |
| --- | --- | --- |
| `car` | Phương tiện cơ giới cá nhân hoặc gia đình được thiết kế chủ yếu để chở người, có không gian khoang hành khách liền khối hoặc tách biệt gọn gàng, thường từ 4 đến 9 chỗ ngồi.| • Ví dụ: Sedan, SUV, hatchback, coupe, crossover. Phân biệt: Kích thước nhỏ/trung bình, không có khoang chở hàng lớn tách rời như truck, không cao lớn và nhiều chỗ như bus.|
| `truck` | Phương tiện cơ giới chuyên dụng được thiết kế để vận chuyển hàng hóa, vật liệu hoặc kéo rơ-moóc. Đặc điểm nhận dạng là có sự tách biệt rõ ràng giữa cabin lái và thùng xe phía sau.| • Ví dụ: Xe tải nhẹ, xe tải thùng, xe ben, xe đầu kéo container. Phân biệt: Khác với van (van có khoang liền khối), truck có phần thùng chở hàng hở hoặc kín nằm tách rời phía sau cabin.|
| `bus` |Phương tiện giao thông công cộng hoặc xe khách cỡ lớn được thiết kế để vận chuyển số lượng lớn hành khách cùng lúc (thường từ 16–30 chỗ trở lên). | • Ví dụ: Xe buýt thành phố, xe khách giường nằm, xe du lịch cỡ lớn. Phân biệt: Thân xe rất dài, cao và rộng; dung tích chứa người lớn hơn nhiều so với van hay xe con.|
| `van` | Phương tiện có cấu trúc thân xe hình hộp liền khối, nơi khoang lái và khoang chở hàng/chở khách nằm chung trong một khung vỏ xe.|Ví dụ: Xe van giao hàng (delivery van), xe tải van cỡ nhỏ, xe khách 16 chỗ (như Ford Transit). Phân biệt: Khác với truck (không tách rời cabin và thùng), khác với car (thân xe cao, vuông vức và thể tích lớn hơn), khác với bus (kích thước nhỏ hơn). |

## Quy tắc chung

- Box bám sát vật thể nghĩa là: Khung bao phải ôm sát các biên ngoài cùng của đối tượng (bao gồm gương chiếu hậu, cản va, bánh xe chạm đất).
- Vật thể bị che khuất: Khi một phần xe bị che khuất bởi vật thể khác (cột điện, người, xe khác), người dán nhãn cần dự phóng và vẽ bounding box bao trọn kích thước thực tế dự kiến của toàn bộ xe (dựa vào hình học chuẩn của xe), hoặc tuân theo quy ước cụ thể của schema dự án (đối với một số dataset chỉ yêu cầu vẽ phần nhìn thấy, tuy nhiên chuẩn chung trong các tác vụ nhận diện toàn phần là dự phóng full-body).
- Vật thể bị cắt bởi rìa ảnh: Khi xe bị cắt cụt bởi khung hình của ảnh (nằm sát mép ảnh), bounding box vẫn ôm lấy toàn bộ phần thân xe còn hiển thị bên trong ảnh và chạm đúng mép biên của khung hình tại vị trí bị cắt.
- Vật thể rất nhỏ/mơ hồ: Các phương tiện xuất hiện quá nhỏ hoặc bị mờ nhòe nặng khiến con người khó xác định chính xác ranh giới: Thường sẽ bỏ qua hoặc gán nhãn thuộc tính đặc biệt tùy theo tài liệu kỹ thuật của dự án.

## Ghi lại quyết định cho ít nhất ba ca mơ hồ

| Ảnh | Tình huống | Quyết định cuối | Lý do theo schema |
| --- | --- | --- | --- |
| `drive_...` | | | |
| `drive_...` | | | |
| `drive_...` | | | |
