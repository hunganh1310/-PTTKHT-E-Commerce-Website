|**Mã Use case**|UC2.1|**Tên Use case**|Đăng nhập|
| :-: | :-: | :-: | :-: |
|**Tác nhân**|User (Người dùng)|||
|**Mô tả**|Cho phép người dùng truy cập vào hệ thống bằng tài khoản đã đăng ký.|||
|**Tiền điều kiện**|<p>Người dùng đã có tài khoản được đăng ký trên hệ thống.</p><p>Hệ thống đang hoạt động bình thường.</p>|||
|**Luồng sự kiện chính (Thành công)**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|1|Người dùng|Người dùng truy cập trang đăng nhập của hệ thống.|
|2|Người dùng|Người dùng nhập tên đăng nhập và mật khẩu vào các trường tương ứng.|
|3|Người dùng|<p>Người dùng nhấn nút "Đăng nhập".</p><p></p>|
|4|Hệ thống|<p>Hệ thống kiểm tra thông tin đăng nhập (tên đăng nhập và mật khẩu) trong cơ sở dữ liệu.</p><p></p>|
|5|Hệ thống|<p>Hệ thống xác nhận thông tin hợp lệ và đăng nhập thành công.</p><p></p>|
|6|Hệ thống|<p>Hệ thống chuyển người dùng đến trang chính.</p><p></p>|

|||||
| :-: | :-: | :- | :- |
|**Luồng sự kiện thay thế**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|4a|Hệ thống|Thông báo: Thông tin đăng nhập không đúng.|
|4b|Hệ thống|Thông báo: Tải khoản của bạn đã bị khóa, vui lòng liên hệ Admin|

|||||
| :-: | :-: | :- | :- |
|**Hậu điều kiện**|<p>Người dùng được đăng nhập thành công và chuyển đến trang chính của hệ thống. </p><p>Phiên đăng nhập của người dùng được tạo.</p>|||



|**Mã Use case**|UC2.2|**Tên Use case**|Đăng ký|
| :-: | :-: | :-: | :-: |
|**Tác nhân**|User (Người dùng)|||
|**Mô tả**|Cho phép người dùng tạo một tài khoản mới để sử dụng hệ thống. Người dùng sẽ cung cấp các thông tin cần thiết như tên đăng nhập, mật khẩu,… để hoàn tất quá trình đăng ký.|||
|**Tiền điều kiện**|<p>Người dùng chưa có tài khoản trên hệ thống. </p><p>Hệ thống đang hoạt động bình thường. </p><p>Người dùng có kết nối internet để truy cập trang đăng ký.</p>|||
|**Luồng sự kiện chính (Thành công)**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|1|Người dùng|Người dùng truy cập trang đăng ký của hệ thống.|
|2|Người dùng|Hệ thống hiển thị biểu mẫu đăng ký, yêu cầu người dùng nhập các thông tin: tên đăng nhập, mật khẩu, và các trường khác.|
|3|Người dùng|Người dùng nhập đầy đủ thông tin vào các trường tương ứng.|
|4|Hệ thống|Người dùng nhấn nút "Đăng ký".|
|5|Hệ thống|Hệ thống kiểm tra tính hợp lệ của thông tin.|
|6|Hệ thống|Hệ thống lưu thông tin tài khoản vào cơ sở dữ liệu.|
|7|Hệ thống|Hệ thống thông báo "Đăng ký thành công" và chuyển người dùng đến trang đăng nhập.|

|||||
| :-: | :-: | :- | :- |
|**Luồng sự kiện thay thế**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|5a|Hệ thống|Thông báo: Thông tin đăng ký không hợp lệ (Đã tồn tại tên đăng nhập, mật khẩu không hợp lệ, email không đúng định dạng,…)|
|6a|Hệ thống|Thông báo: Hệ thống gặp lỗi khi lưu tài khoản. Vui lòng liên hệ Admin hoặc thử lại sau.|

|||||
| :-: | :-: | :- | :- |
|**Hậu điều kiện**|<p>Tài khoản của người dùng được tạo thành công và lưu vào cơ sở dữ liệu. </p><p>Người dùng được chuyển đến trang đăng nhập để sử dụng tài khoản mới.</p>|||

|**Mã Use case**|UC2.3|**Tên Use case**|Đăng xuất|
| :-: | :-: | :-: | :-: |
|**Tác nhân**|User (Người dùng)|||
|**Mô tả**|Cho phép người dùng kết thúc phiên đăng nhập hiện tại và thoát khỏi hệ thống. Sau khi đăng xuất, người dùng sẽ không thể truy cập các chức năng yêu cầu đăng nhập cho đến khi đăng nhập lại.|||
|**Tiền điều kiện**|<p>Người dùng đã đăng nhập vào hệ thống. </p><p>Hệ thống đang hoạt động bình thường. </p><p>Người dùng đang ở một trang bất kỳ trong hệ thống (sau khi đăng nhập).</p>|||
|**Luồng sự kiện chính (Thành công)**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|1|Người dùng|Người dùng nhấn nút "Đăng xuất" trên giao diện hệ thống (góc trên bên phải màn hình).|
|2|Hệ thống|Hệ thống hiển thị thông báo xác nhận: "Bạn có chắc chắn muốn đăng xuất không?" với hai tùy chọn "Có" và "Không".|
|3|Người dùng|Người dùng chọn "Có" để xác nhận đăng xuất.|
|4|Hệ thống|Hệ thống kết thúc phiên đăng nhập hiện tại của người dùng (xóa thông tin phiên trong cơ sở dữ liệu hoặc bộ nhớ).|
|5|Hệ thống|Hệ thống thông báo "Bạn đã đăng xuất thành công".|
|6|Hệ thống|Hệ thống chuyển người dùng về trang đăng nhập.|

|||||
| :-: | :-: | :- | :- |
|**Luồng sự kiện thay thế**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|2a|Hệ thống|Hệ thống giữ nguyên phiên đăng nhập hiện tại nếu người dùng chọn “Không” để hủy đăng xuất|

|||||
| :-: | :-: | :- | :- |
|**Hậu điều kiện**|<p>Phiên đăng nhập của người dùng được kết thúc. </p><p>Người dùng được chuyển về trang đăng nhập và không thể truy cập các chức năng yêu cầu đăng nhập cho đến khi đăng nhập lại.</p>|||

|**Mã Use case**|UC2.4|**Tên Use case**|Quên mật khẩu|
| :-: | :-: | :-: | :-: |
|**Tác nhân**|User (Người dùng)|||
|**Mô tả**|Cho phép người dùng khôi phục quyền truy cập vào tài khoản khi họ quên mật khẩu. Người dùng sẽ cung cấp email/số điện thoại đã đăng ký, và hệ thống sẽ gửi một liên kết hoặc mã để đặt lại mật khẩu.|||
|**Tiền điều kiện**|<p>Người dùng đã có tài khoản được đăng ký trên hệ thống.</p><p>Hệ thống đang hoạt động bình thường.</p>|||
|**Luồng sự kiện chính (Thành công)**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|1|Người dùng|Người dùng truy cập trang "Quên Mật Khẩu".|
|2|Người dùng|Người dùng nhập email hoặc số điện thoại.|
|3|Người dùng|Người dùng nhấn nút "Xác nhận".|
|4|Hệ thống|Hệ thống kiểm tra email/số điện thoại có tồn tại trong hệ thống hay không.|
|5|Hệ thống|Hệ thống xác nhận thông tin hợp lệ và gửi link cấp lại mật khẩu về email/số điện thoại.|
|6|Người dùng|Người dùng chờ nhận hướng dẫn từ email/ SMS và tiến hành bước tiếp theo trong quy trình “Cấp lại mật khẩu”|

|||||
| :-: | :-: | :- | :- |
|**Luồng sự kiện thay thế**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|5a|Hệ thống|Thông báo: Thông tin email/số điện thoại không đúng.|
|6a|Người dùng|Thông báo: Không nhận được email/SMS.|

|||||
| :-: | :-: | :- | :- |
|**Hậu điều kiện**|Người dùng nhận được hướng dẫn từ email/SMS hoặc Admin và tiến hành quy trình "Cấp lại mật khẩu".|||




|**Mã Use case**|UC2.5|**Tên Use case**|Sửa thông tin|
| :-: | :-: | :-: | :-: |
|**Tác nhân**|User (Người dùng)|||
|**Mô tả**|Cho phép người dùng chỉnh sửa thông tin cá nhân như họ tên, email, số điện thoại, địa chỉ, ảnh đại diện, mật khẩu v.v.|||
|**Tiền điều kiện**|<p>Người dùng đã đăng nhập vào hệ thống.</p><p>Hệ thống đang hoạt động bình thường.</p>|||
|**Luồng sự kiện chính (Thành công)**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|1|Người dùng|Người dùng truy cập giao diện chỉnh sửa thông tin.|
|2|Người dùng|Người dùng chỉnh sửa thông tin mong muốn.|
|3|Người dùng|Người dùng nhấn nút "Lưu thay đổi".|
|4|Hệ thống|Hệ thống kiểm kiểm tra tính hợp lệ của thông tin mới.|
|5|Hệ thống|Hệ thống xác nhận thông tin hợp lệ, lưu vào cơ sở dữ liệu và thông báo thành công.|
|6|Hệ thống|Hệ thống chuyển người dùng về lại giao diện chỉnh sửa thông tin.|

|||||
| :-: | :-: | :- | :- |
|**Luồng sự kiện thay thế**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|4a|Hệ thống|Thông báo: Thông tin nhập vào không hợp lệ.|
|5a|Hệ thống|Thông báo: Thông tin lưu không thành công do lỗi kỹ thuật.|

|||||
| :-: | :-: | :- | :- |
|**Hậu điều kiện**|Người dùng sửa đổi thông tin thành công và chuyển người dùng về giao diện chỉnh sửa thông tin.|||



|**Mã Use case**|UC2.6|**Tên Use case**|Quản lí tài khoản|
| :-: | :-: | :-: | :-: |
|**Tác nhân**|Admin|||
|**Mô tả**|Admin thực hiện các chức năng quản lý tài khoản người dùng như chỉnh sửa thông tin, khóa/mở tài khoản, đổi mật khẩu hoặc cấp lại mật khẩu cho người dùng.|||
|**Tiền điều kiện**|<p>Admin đã đăng nhập vào hệ thống.</p><p>Hệ thống đang hoạt động bình thường.</p>|||
|**Luồng sự kiện chính (Thành công)**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|1|Admin|Admin truy cập giao diện quản lý tài khoản.|
|2|Admin|Admin tìm kiếm tài khoản cần quản lý.|
|3|Admin|Admin thực hiện các hành động để quản lý tài khoản đã tìm kiếm.|
|4|Hệ thống|Hệ thống kiểm tra và xác nhận thay đổi.|
|5|Hệ thống|Hệ thống lưu lại thông tin mới vào cơ sở dữ liệu và thông báo kết quả.|

|||||
| :-: | :-: | :- | :- |
|**Luồng sự kiện thay thế**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|3a|Hệ thống|Thông báo: Hành động không hợp lệ. (Do khóa admin khác, email không hợp lệ,..)|
|5a|Hệ thống|Thông báo: Lưu thay đổi không thành công do lỗi hệ thống.|

|||||
| :-: | :-: | :- | :- |
|**Hậu điều kiện**|Thông tin tài khoản của người dùng đã được quản lý thành công theo yêu cầu của Admin.|||



|**Mã Use case**|UC2.7|**Tên Use case**|Cấp lại mật khẩu|
| :-: | :-: | :-: | :-: |
|**Tác nhân**|User (Người dùng)|||
|**Mô tả**|<p>Cho phép người dùng tự thiết lập mật khẩu mới sau khi xác minh danh tính qua email/SMS.</p><p>Admin có quyền đặt lại mật khẩu cho User khi nhận yêu cầu.</p>|||
|**Tiền điều kiện**|<p>User đã yêu cầu "Quên Mật Khẩu" và nhận được email/xác nhận OTP.</p><p>Hoặc Admin nhận được yêu cầu từ User.</p><p>`           `Hệ thống đang hoạt động bình thường.</p>|||
|**Luồng sự kiện chính (Thành công)**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|1|Người dùng|Người dùng nhập link xác minh hoặc OTP nhận được từ email/SMS.|
|2|Hệ thống|Hệ thống kiểm tra link/OTP có hợp lệ hay không.|
|3|Người dùng|Người dùng nhập mật khẩu mới và xác nhận.|
|4|Hệ thống|Hệ thống kiểm tra thông tin mật khẩu mới.|
|5|Hệ thống|Hệ thống lưu mật khẩu mới và thông báo thành công.|
|6|Hệ thống|Hệ thống chuyển người dùng đến trang đăng nhập.|

||<p>Nếu người dùng tự cấp lại mật khẩu</p><p></p>|||
| :-: | :-: | :- | :- |

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|1|Admin|Admin truy cập giao diện quản lý tài khoản.|
|2|Admin|Admin tìm người dùng và chọn tùy chọn "Cấp lại mật khẩu".|
|3|Admin|Admin nhập mật khẩu mới hoặc gửi link reset cho User.|
|4|Hệ thống|Hệ thống cập nhật mật khẩu mới và thông báo thành công.|
|5|Hệ thống|Hệ thống xác nhận thông tin hợp lệ và đăng nhập thành công.|
|6|Admin|Admin thông báo cho người dùng về mật khẩu mới hoặc người dùng nhận link reset.|

||Nếu Admin cấp lại mật khẩu cho người dùng|||
| :-: | :-: | :- | :- |
|**Luồng sự kiện thay thế**||||

|**STT**|**Thực hiện bởi**|**Hành động**|
| :-: | :-: | :-: |
|1|Hệ thống|Thông báo: Mật khẩu mới không hợp lệ.|
|2|Hệ thống|Thông báo: Admin nhập sai thông tin người dùng.|

|||||
| :-: | :-: | :- | :- |
|**Hậu điều kiện**|<p>Mật khẩu của người dùng đã được cập nhật.</p><p>Hệ thống chuyển về trang đăng nhập.</p>|||

