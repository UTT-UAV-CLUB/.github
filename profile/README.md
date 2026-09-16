<div align="center">

<img src="banner.svg" alt="UTT UAV CLUB" width="100%">

<br><br>

[![Facebook](https://img.shields.io/badge/Facebook-0EA5E9?style=flat-square&labelColor=0A1E3C)](https://www.facebook.com/profile.php?id=100076017564067)
[![Email](https://img.shields.io/badge/Email-22D3EE?style=flat-square&labelColor=0A1E3C)](mailto:utt.uav.club@gmail.com)
[![Hanoi](https://img.shields.io/badge/Ha%20Noi-6366F1?style=flat-square&labelColor=0A1E3C)](#)

</div>

<br>

## Giới thiệu

**UTT UAV CLUB** là nhóm nghiên cứu do sinh viên Trường Đại học Công nghệ Giao thông Vận tải vận hành. Chúng tôi thiết kế và chế tạo hệ thống bay không người lái theo chuỗi khép kín — từ bo mạch điều khiển bay và firmware, tới khả năng tự hành, thị giác máy tính trên máy bay, cho đến phần mềm trạm mặt đất kết nối toàn bộ hệ thống.

Đây là nơi lưu trữ mã nguồn, file thiết kế phần cứng và tài liệu kỹ thuật của câu lạc bộ. Các kho mã nguồn công khai mở cho bất kỳ ai muốn đọc và học hỏi. Những phần còn đang phát triển, phục vụ cuộc thi, hoặc ràng buộc với đối tác sẽ được để riêng tư và chỉ chia sẻ trong nội bộ.

<br>

## Bắt đầu từ đâu

> [!TIP]
> **Mới vào câu lạc bộ, hoặc đang cân nhắc tham gia?**
> Đọc **[Định hướng cho thành viên mới](https://github.com/UTT-UAV-CLUB/Dinh-huong)** trước.

Tài liệu đó trả lời đúng câu hỏi mà hầu hết người mới đang mắc: *muốn làm drone tự bay / AI nhận diện / hệ thống IoT thì phải bắt đầu học từ đâu?*

Nội dung gồm: bốn nền nghề để bạn chọn một hướng đi sâu, ba mảng sản phẩm câu lạc bộ đang làm, bài tự kiểm tra để biết mình đang ở đâu, và bài tự chấm cho từng nền. Không yêu cầu kiến thức nền trước khi đọc.

<br>

## Hướng nghiên cứu

<table>
<tr>
<td width="50%" valign="top">

![](https://img.shields.io/badge/01-Flight%20Control%20%26%20Firmware-0EA5E9?style=for-the-badge&labelColor=0A1E3C)

Bo mạch điều khiển bay tự thiết kế, driver mức thấp, tích hợp ArduPilot / PX4, điều khiển thời gian thực.

</td>
<td width="50%" valign="top">

![](https://img.shields.io/badge/02-Autonomy%20%26%20Perception-22D3EE?style=for-the-badge&labelColor=0A1E3C)

Bay theo waypoint, hạ cánh chính xác, bám mục tiêu bằng thị giác, suy luận AI ngay trên máy bay.

</td>
</tr>
<tr>
<td width="50%" valign="top">

![](https://img.shields.io/badge/03-Hardware%20%26%20PCB-6366F1?style=for-the-badge&labelColor=0A1E3C)

Thiết kế nguyên lý, layout nhiều lớp, hệ thống nguồn, tích hợp khung bay và cơ khí.

</td>
<td width="50%" valign="top">

![](https://img.shields.io/badge/04-Telemetry%20%26%20GCS-14B8A6?style=for-the-badge&labelColor=0A1E3C)

Trạm điều khiển mặt đất, giao thức MAVLink, đường truyền radio và 4G/LTE, phân tích dữ liệu bay.

</td>
</tr>
</table>

<br>

## Công nghệ sử dụng

```text
 Flight stack       →  ArduPilot, PX4, MAVLink, MAVSDK
 Onboard compute    →  STM32, ESP32, Raspberry Pi, NVIDIA Jetson
 Vision & AI        →  OpenCV, YOLO, Hailo, Coral Edge TPU
 Hardware design    →  Altium Designer, KiCad, EasyEDA
 Languages          →  C / C++, Python
```

<br>

## Kho mã nguồn

| Kho mã nguồn | Mô tả |
| --- | --- |
| [**Dinh-huong**](https://github.com/UTT-UAV-CLUB/Dinh-huong) | Định hướng cho thành viên mới — mỗi mảng cần nền gì, học gì, bắt đầu từ đâu |

> [!NOTE]
> Phần lớn kho mã nguồn của câu lạc bộ đang để **riêng tư**: dự án còn đang phát triển, bài dự thi, hoặc có ràng buộc với đối tác. Các kho công khai sẽ lần lượt được liệt kê ở đây.

**Muốn xem các kho riêng tư?** Liên hệ ban quản lý câu lạc bộ để được thêm vào tổ chức.

| | |
| --- | --- |
| **Cách liên hệ** | Nhắn [Facebook](https://www.facebook.com/profile.php?id=100076017564067) hoặc gửi email tới utt.uav.club@gmail.com |
| **Cần cung cấp** | Họ tên, khoa/lớp, tên tài khoản GitHub của bạn, và mảng bạn đang tham gia |
| **Sau khi được duyệt** | Bạn nhận lời mời qua email đã đăng ký GitHub — bấm chấp nhận, rồi mở tab **Repositories** để xem các kho mình có quyền truy cập |

Thành viên đã ở trong tổ chức mà không thấy kho mình cần: nhắn người phụ trách mảng đó, quyền truy cập được cấp theo từng nhóm.

<br>

## Quy trình đóng góp

Mọi thay đổi đi vào `main` đều phải qua Pull Request — không push thẳng.

```text
 main                    ổn định, đã kiểm chứng trên phần cứng thật
 dev                     nhánh tích hợp
 feat/<tên>-<nội dung>   nhánh làm việc của bạn
```

1. Tạo nhánh mới tách ra từ `dev`.
2. Commit thành từng bước nhỏ, thông điệp rõ ràng.
3. Mở Pull Request và yêu cầu review từ nhóm phụ trách mảng đó.
4. Không đưa file nhị phân lớn vào Git.

> [!IMPORTANT]
> Log bay, rosbag và video FPV phải để trên kho lưu trữ chung của lab, chỉ ghi đường dẫn vào `README` của kho mã nguồn. Đẩy lên Git là kho phình vĩnh viễn và không gỡ ra được.

Hướng dẫn chi tiết: [CONTRIBUTING.md](https://github.com/UTT-UAV-CLUB/.github/blob/main/CONTRIBUTING.md)

<br>

## Tham gia cùng chúng tôi

Chúng tôi chào đón sinh viên từ mọi khoa muốn làm việc với phần cứng bay thật — dù thế mạnh của bạn là firmware, điện tử, lý thuyết điều khiển, thị giác máy tính hay thiết kế cơ khí. Không yêu cầu kinh nghiệm từ trước; điều cần là sự tò mò và theo được đến cùng.

Chưa biết mình hợp với mảng nào? Đọc **[Định hướng cho thành viên mới](https://github.com/UTT-UAV-CLUB/Dinh-huong)** — tài liệu mô tả rõ từng hướng để bạn tự thấy mình hợp với cái gì trước khi đăng ký.

Liên hệ với chúng tôi qua các kênh bên dưới.

<br>

## Liên hệ

| | |
| --- | --- |
| **Facebook** | [UTT UAV Club](https://www.facebook.com/profile.php?id=100076017564067) |
| **Email** | utt.uav.club@gmail.com |
| **Địa chỉ** | Phòng 102, Nhà Chuyên Gia, Trường Đại học Công nghệ Giao thông Vận tải, Hà Nội |

<br>

---

<div align="center">
<sub>Được xây dựng bởi sinh viên Trường Đại học Công nghệ Giao thông Vận tải.</sub>
</div>
