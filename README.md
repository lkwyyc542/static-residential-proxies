# proxy dân cư tĩnh: phân biệt IP tĩnh thật với phiên giữ IP dài, và cách chọn gói 9Proxy theo nhu cầu MMO

Từ khóa "proxy dân cư tĩnh" thường được gõ vào ô tìm kiếm khi bạn đang mắc một vấn đề rất cụ thể: tài khoản cứ bị checkpoint, hoặc một luồng công việc cần cùng một IP qua nhiều phiên đăng nhập. Vấn đề nằm ở chỗ cụm từ này đang bị dùng cho hai thứ khác nhau, và giá của chúng chênh nhau tới hàng chục lần.

Hiểu sai chỗ này thì bạn sẽ mua thừa tiền, hoặc mua thiếu và vẫn gặp lại đúng cái lỗi cũ sau vài ngày.

## "Proxy dân cư tĩnh" đang bị dùng cho hai khái niệm khác nhau

Nghĩa gốc của static residential proxy là IP dân cư thật nhưng cố định – thường gọi là ISP proxy. IP thuộc về một nhà mạng cụ thể (AT&T, Verizon, Cox…), không đổi trong suốt thời gian thuê, và thường được bán theo gói tháng, ví dụ 10 IP trong 30 ngày. Nó gần với "một đường internet cố định ở nhà" hơn là một proxy xoay.

Nhưng khi nói chuyện với người làm MMO, cụm "proxy dân cư tĩnh" phần lớn được dùng để chỉ loại proxy dân cư xoay giữ nguyên IP trong một phiên – gọi là sticky session. IP là IP nhà dân thật, chỉ khác ở chỗ nó không nhảy mỗi request mà bám theo session bạn cấu hình.

| Tiêu chí | ISP / static residential "thật" | Phiên sticky của proxy dân cư |
| --- | --- | --- |
| IP có đổi không | Không đổi trong thời gian thuê | Đổi khi phiên kết thúc |
| Bạn thuê IP hay thuê phiên | Thuê theo IP, thường theo tháng | Trả theo IP hoặc theo GB |
| Giá tham chiếu | Cao hơn nhiều lần, tính bằng đơn vị USD/IP/tháng | Từ vài chục cent đến vài USD |
| Hợp với | Nuôi tài khoản dài hạn, đăng nhập định kỳ, cần fingerprint trùng khớp | Đăng nhập, thao tác tài khoản, kiểm tra giá, automation cần một danh tính ổn định trong phiên |
| Rủi ro | Ít đổi IP → dễ bị nhận diện là proxy hơn nếu IP bẩn | Hiệu quả tốt nhưng hết phiên là IP khác |

Với phần lớn người làm affiliate, dropshipping, quản lý fanpage hay vận hành nhiều tài khoản sàn thương mại điện tử, thứ họ cần thực chất nằm ở cột phải: một IP ổn định trong vài chục phút đến vài giờ, đủ để đăng nhập, xử lý xong việc và thoát ra sạch sẽ. Thuê ISP theo tháng cho việc này thường là trả tiền cho sự cố định mà bạn không dùng hết.

## Khi nào "IP không đổi vài giờ" là đủ, khi nào không

Có một cách phân loại khá thực dụng. Nếu tác vụ của bạn kết thúc trong một phiên làm việc – đăng nhập Facebook, lên đơn, kiểm tra dashboard, đọc dữ liệu từ một trang cần geo chính xác – thì sticky session là đủ. Bạn không cần IP đó tồn tại đến tuần sau.

Ngược lại, có ba tình huống mà sticky "vài giờ" tỏ ra thiếu:

- Tài khoản được đăng nhập từ cùng một IP theo lịch cố định trong nhiều ngày, ví dụ nuôi tài khoản TikTok theo mốc giờ.
- Nền tảng lưu lịch sử IP và coi việc đổi IP liên tục là dấu hiệu bất thường, kể cả khi mỗi phiên đều sạch.
- Bạn cần cấu hình IP đó vào antidetect browser và dùng lại lâu dài, không muốn sửa profile mỗi ngày.

Ba tình huống trên mới là địa hạt của ISP proxy. Còn lại, cùng một danh tính trong phiên là mức ổn định mà phần lớn công việc cần.

## 9Proxy cung cấp đúng phần nào của nhu cầu đó

9Proxy là nền tảng proxy dân cư với pool được công bố khoảng 20 triệu IP trải trên hơn 90 quốc gia, hỗ trợ cả HTTP/HTTPS và SOCKS5. Điểm cần nói rõ ngay: 9Proxy không bán ISP proxy theo tháng kiểu truyền thống. Thứ họ có là hai mô hình dân cư, và một trong hai chính là phần mà người tìm "proxy dân cư tĩnh" đang cần.

**Gói theo IP (Residential Proxy by IPs).** Bạn mua một lượng IP cố định, trả tiền theo IP chứ không theo dung lượng, băng thông không giới hạn trong thời gian IP hoạt động. IP chỉ bị trừ khi bạn forward nó ra một port, và IP chưa dùng thì không hết hạn – nằm nguyên trong số dư. Khi đã kích hoạt, một IP sống từ vài giờ đến khoảng 24 giờ, tùy từng IP do đây là pool nhà dân thật. Nếu IP chết giữa chừng, có Auto Refresh để tự thay IP mới, hoặc Auto Rotation để xoay theo chu kỳ bạn đặt.

Đây là mô hình gần nhất với tinh thần "tĩnh": IP không nhảy loạn, bạn giữ nó suốt phiên làm việc, và vì băng thông không giới hạn nên bạn không phải canh dung lượng khi tải dữ liệu nặng.

**Gói theo GB (Residential Proxy by GB).** Trả theo lưu lượng, tạo endpoint không giới hạn, hiệu lực tối thiểu 180 ngày. Điểm đáng chú ý với chủ đề này nằm ở chỗ gói GB hỗ trợ cả chế độ xoay và chế độ sticky. Sticky được điều khiển bằng hai tham số nhét trong username: `sst` (số phút giữ nguyên IP) và `ssid` (mã phiên, để bạn có nhiều IP sticky song song từ cùng một cấu hình).

Ví dụ cấu trúc username theo tài liệu của 9Proxy:


subaccount-country-us-sst-15-ssid-device1
subaccount-country-vn-city-hanoi-sst-20
subaccount-isp-as22773_Cox_Communications_Inc.-sst-30


Bạn có thể lọc theo quốc gia, bang/tỉnh, thành phố, mã bưu chính và cả ISP. Với người làm antidetect browser, bộ lọc theo ISP khá hữu dụng: profile khớp cả IP lẫn nhà mạng thì fingerprint trông nhất quán hơn.

Một điểm khác biệt về vận hành: gói theo IP yêu cầu app desktop (Windows, macOS, Linux) để forward port ra `localhost`, còn gói theo GB dùng trực tiếp từ dashboard bằng username/password hoặc whitelist IP. Nếu bạn muốn cắm thẳng vào browser hay script mà không cài gì, gói GB nhẹ nhàng hơn.

### Còn chuyện "static residential" thì sao?

Trang FAQ và một số hồ sơ sản phẩm của 9Proxy có ghi họ hỗ trợ Static Residential Proxies, cho phép giữ một địa chỉ IP cố định trong thời gian dài. Tài liệu kỹ thuật chính thức tại docs.9proxy.com thì chỉ mô tả hai mô hình dân cư như trên, và nêu rõ tuổi thọ IP của gói theo IP là vài giờ đến khoảng 24 giờ, thay đổi tự nhiên theo tính chất của pool. Một số bài đánh giá độc lập cũng cho rằng 9Proxy hiện không có dòng sản phẩm ISP/static riêng biệt như các nhà cung cấp chuyên ISP.

Nói thẳng: nếu yêu cầu của bạn là "cùng một IP trong 30 ngày", hãy xác nhận với bộ phận hỗ trợ trước khi nạp tiền, đừng suy ra từ dòng marketing. Còn nếu yêu cầu là "một IP ổn định trong phiên, không đổi giữa các request", gói theo IP làm được việc đó ngay.

## Bảng giá đầy đủ các gói đang niêm yết

9Proxy công bố điều chỉnh giá với gói theo IP và gói kết hợp từ ngày 1/6/2026; giá gói theo GB được giữ nguyên. Các mức dưới đây là giá niêm yết công khai trên thị trường, đơn vị USD, không phải phí thuê bao định kỳ – bạn nạp số dư và dùng dần.

**Nhóm gói theo IP (băng thông không giới hạn, IP chưa dùng không hết hạn):**

| Gói | Bạn nhận được | Đơn giá/IP | Tổng | Link mua |
| --- | --- | --- | --- | --- |
| 100 IPs | 100 IP | $0,24 | $24 | [ Xem gói 100 IP tại 9Proxy](https://bit.ly/9-Proxy) |
| 500 IPs | 500 IP | $0,144 | $72 | [ Xem gói 500 IP tại 9Proxy](https://bit.ly/9-Proxy) |
| 1.000 + 500 IPs | 1.000 IP, tặng thêm 500 IP | $0,084 | $126 | [ Xem gói 1.000 + 500 IP tại 9Proxy](https://bit.ly/9-Proxy) |
| 2.500 IPs | 2.500 IP | $0,084 | $210 | [ Xem gói 2.500 IP tại 9Proxy](https://bit.ly/9-Proxy) |
| 5.000 IPs | 5.000 IP | $0,072 | $360 | [ Xem gói 5.000 IP tại 9Proxy](https://bit.ly/9-Proxy) |
| 15.000 IPs | 15.000 IP | $0,048 | $720 | [ Xem gói 15.000 IP tại 9Proxy](https://bit.ly/9-Proxy) |
| 25.000 IPs | 25.000 IP | $0,035 | $863 | [ Xem gói 25.000 IP tại 9Proxy](https://bit.ly/9-Proxy) |
| 50.000 IPs | 50.000 IP | $0,029 | $1.438 | [ Xem gói 50.000 IP tại 9Proxy](https://bit.ly/9-Proxy) |
| 100.000 IPs (Business) | 100.000 IP | $0,023 | $2.300 | [ Xem gói Business 100.000 IP tại 9Proxy](https://bit.ly/9-Proxy) |
| 200.000 IPs (Business) | 200.000 IP | $0,021 | $4.140 | [ Xem gói Business 200.000 IP tại 9Proxy](https://bit.ly/9-Proxy) |
| 500.000 IPs (Business) | 500.000 IP | $0,018 | $8.625 | [ Xem gói Business 500.000 IP tại 9Proxy](https://bit.ly/9-Proxy) |

**Nhóm gói theo GB – hiệu lực 180 ngày:**

| Gói | Lưu lượng | Đơn giá/GB | Tổng | Link mua |
| --- | --- | --- | --- | --- |
| 5 GB | 5 GB | $3,00 | $15 | [ Xem gói 5 GB tại 9Proxy](https://bit.ly/9-Proxy) |
| 50 + 5 GB | 55 GB | $2,10 | $105 | [ Xem gói 50 + 5 GB tại 9Proxy](https://bit.ly/9-Proxy) |
| 100 GB | 100 GB | $1,50 | $150 | [ Xem gói 100 GB tại 9Proxy](https://bit.ly/9-Proxy) |
| 200 GB | 200 GB | $1,00 | $200 | [ Xem gói 200 GB tại 9Proxy](https://bit.ly/9-Proxy) |
| 1.000 GB | 1.000 GB | $0,80 | $800 | [ Xem gói 1.000 GB tại 9Proxy](https://bit.ly/9-Proxy) |
| 2.000 GB | 2.000 GB | $0,75 | $1.500 | [ Xem gói 2.000 GB tại 9Proxy](https://bit.ly/9-Proxy) |

**Nhóm gói theo GB dành cho Enterprise – không giới hạn hiệu lực:**

| Gói | Lưu lượng | Đơn giá/GB | Tổng | Link mua |
| --- | --- | --- | --- | --- |
| 3.000 GB | 3.000 GB | $0,72 | $2.160 | [ Xem gói Enterprise 3.000 GB tại 9Proxy](https://bit.ly/9-Proxy) |
| 6.000 GB | 6.000 GB | $0,70 | $4.200 | [ Xem gói Enterprise 6.000 GB tại 9Proxy](https://bit.ly/9-Proxy) |
| 10.000 GB | 10.000 GB | $0,68 | $6.800 | [ Xem gói Enterprise 10.000 GB tại 9Proxy](https://bit.ly/9-Proxy) |

**Nhóm gói kết hợp (IP + GB trong cùng một gói):**

| Gói | Nội dung | Tổng | Link mua |
| --- | --- | --- | --- |
| Starter | 100 IP + 5 GB | $30 | [ Xem gói Bundle Starter tại 9Proxy](https://bit.ly/9-Proxy) |
| Popular | 1.500 IP + 50 GB | $180 | [ Xem gói Bundle Popular tại 9Proxy](https://bit.ly/9-Proxy) |
| Pro | 5.000 IP + 500 GB | $720 | [ Xem gói Bundle Pro tại 9Proxy](https://bit.ly/9-Proxy) |

Vài quan sát từ chính bảng này. Thứ nhất, bậc 1.000 + 500 IP là điểm rẻ đi rõ rệt so với bậc 500 IP – đơn giá gần như giảm một nửa. Thứ hai, gói GB có hiệu lực 180 ngày nên phù hợp với công việc theo dự án, không bị ép tiêu hết trong 30 ngày. Thứ ba, nhóm Enterprise GB bỏ hẳn giới hạn hiệu lực, đây là lựa chọn cho ai chạy hạ tầng liên tục.

Cần lưu ý: giá có thể được điều chỉnh và một số đợt khuyến mãi theo dịp (ví dụ đợt giảm giá theo mùa cho gói IP và GB, hoặc ưu đãi khi thanh toán bằng crypto) chỉ tồn tại trong thời gian giới hạn. Trước khi nạp, hãy kiểm tra mức giá hiển thị tại thời điểm mua thay vì tin vào bảng giá được chia sẻ lại ở đâu đó.

## Chọn gói nào cho công việc cụ thể

Nếu bạn quản lý vài chục profile antidetect browser (Hidemium, Multilogin, AdsPower, ixBrowser, Dolphin Anty…) và cần mỗi profile một IP ổn định trong phiên làm việc, gói theo IP ở bậc 100 hoặc 500 là điểm khởi đầu hợp lý. Bạn trả một lần, IP chưa dùng vẫn còn nguyên, và không phải nghĩ đến dung lượng khi mở hàng loạt tab.

Nếu công việc là scraping, kiểm tra giá, xác minh quảng cáo hay đối chiếu SERP theo khu vực – tức mỗi request chỉ tốn vài trăm KB nhưng cần nhiều IP khác nhau – thì gói theo GB rẻ hơn nhiều về mặt lý thuyết. Bạn cũng được lợi ở chỗ cấu hình sticky không cần cài app, chỉ cần chỉnh `sst` trong username.

Nếu bạn vừa cần IP giữ phiên vừa cần băng thông cho tác vụ nặng, gói kết hợp là cấu hình gọn nhất về mặt quản lý: một số dư, một dashboard.

Và nếu bạn là reseller bán lại proxy cho khách của mình, các bậc Business từ 100.000 IP trở lên mới là vùng đáng xem, vì đơn giá rơi xuống quanh $0,018–0,023/IP.

## Bắt đầu vài phút, nhưng đừng bỏ qua phần chính sách

Quy trình gọn: tạo tài khoản, chọn gói, rồi dùng theo một trong hai cách – tải app desktop để forward port (gói theo IP), hoặc lấy host/port/username/password từ dashboard cho gói GB. Có cả Proxy2Web để chạy ngay trên trình duyệt không cần cài đặt, và API công khai cho ai muốn tự động hóa việc tạo proxy, xoay IP, quản lý sub-user.

Thanh toán khá rộng: thẻ tín dụng/ghi nợ, Apple Pay, Google Pay, Alipay và crypto qua CoinPayments (BTC, ETH, LTC, TRX, USDT-TRC20/ERC20, DOGE, DAI, BCH). Theo hồ sơ sản phẩm, người trả bằng crypto được cộng thêm 5% IP – khoản này chỉ có ý nghĩa nếu bạn vốn đã giữ stablecoin.

Phần cần đọc kỹ là hoàn tiền. Chính sách được công bố khá hẹp, chủ yếu xử lý trường hợp IP không kết nối được trong khoảng 60 giây đầu. Không có bản dùng thử miễn phí rõ ràng cho mọi người – một số kênh của 9Proxy nói có bản dùng thử giới hạn cho người dùng mới tùy tình trạng còn hay hết, nên nếu muốn thử trước, hãy hỏi hỗ trợ. Một số bài đánh giá độc lập cũng ghi nhận khiếu nại xoay quanh chính sách hoàn tiền, và lưu ý rằng 9Proxy đã tuyên bố không hỗ trợ streaming (ví dụ YouTube) trên gói theo IP theo điều khoản sử dụng mới. Nếu mục đích của bạn là xem nội dung giới hạn vùng, hãy kiểm tra lại điều khoản hiện hành trước khi mua.

## Câu hỏi thường gặp

**Gói theo IP của 9Proxy có phải proxy tĩnh không?**
Không theo nghĩa ISP proxy thuê theo tháng. Bạn giữ được một IP ổn định trong phiên, kéo dài từ vài giờ đến khoảng 24 giờ. Muốn IP cố định dài hạn, cần xác nhận trực tiếp với hỗ trợ.

**Muốn nhiều IP sticky dùng song song thì làm thế nào?**
Dùng gói GB và thêm `ssid` khác nhau cho mỗi phiên, ví dụ `ssid-device1`, `ssid-device2`. Mỗi `ssid` sẽ cho một IP riêng dù các tham số khác giống nhau.

**Sticky tối đa bao lâu?**
`sst` là số phút bạn tự đặt trong username. Đặt quá dài sẽ thu hẹp pool khả dụng, nhất là khi bạn lọc thêm thành phố và ISP cùng lúc – tài liệu của 9Proxy cũng khuyến nghị tránh lọc chồng nhiều lớp.

**Có dùng được với antidetect browser không?**
Có. SOCKS5 và HTTP/HTTPS đều được hỗ trợ, và một số antidetect browser như ixBrowser hay Multilogin có tài liệu hướng dẫn tích hợp riêng.

**Nên mua IP hay mua GB?**
Nếu băng thông khó đoán và bạn cần IP giữ ổn định, mua theo IP. Nếu mỗi request tốn ít dữ liệu nhưng cần nhiều IP, mua theo GB.

Nếu bạn đã xác định được mình thuộc nhóm nào, bước tiếp theo chỉ là chọn bậc phù hợp: [👉 tạo tài khoản 9Proxy và xem bảng giá hiện hành](https://bit.ly/9-Proxy).

## Tóm lại

"Proxy dân cư tĩnh" là một cụm từ bị dùng lẫn, và cái giá phải trả cho việc hiểu sai không hề nhỏ. Phần lớn công việc MMO chỉ cần một IP ổn định trong phiên – đó chính là thứ gói theo IP của 9Proxy cung cấp, với băng thông không giới hạn và IP chưa dùng không hết hạn. Việc cần IP cố định hàng tháng là câu chuyện khác, và trước khi trả tiền cho nó, hãy chắc chắn rằng nhà cung cấp thực sự có dòng sản phẩm đó.
