Phân tích lỗi và Test Cases

Nguyên nhân lỗi:
Dùng pop() lấy nhầm xe ở cuối hàng thay vì xe đầu hàng. Cần sửa thành shift() để xe đến trước vào sạc trước.
Vòng lặp duyệt i <= length dẫn đến truy cập phần tử ngoài mảng (undefined) và in thừa dòng "STT 4: undefined". Sửa điều kiện thành i < length.
Bảng Test Cases:
STT	Trường hợp kiểm thử	Dữ liệu đầu vào	Kết quả sai thực tế	Kết quả đúng mong đợi
1	Mảng ban đầu có 3 xe, thêm 1 xe	hangDoi = ['30A-98765', '29B-12345', '51C-45678'], xeMoi = '43D-88888'	Xe vào: 51C-45678
Bảng LED thừa dòng undefined ở cuối	Xe vào: 30A-98765
Bảng LED: STT 1: 29B-12345, STT 2: 51C-45678, STT 3: 43D-88888
2	Mảng ban đầu chỉ có 1 xe	hangDoi = ['14A-11111'], xeMoi = '99B-22222'	Xe vào: 14A-11111
Bảng LED thừa dòng undefined ở cuối	Xe vào: 14A-11111
Bảng LED: STT 1: 99B-22222
