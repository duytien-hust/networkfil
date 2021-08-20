---


---

<h1 id="network-b1">Network B1</h1>
<h2 id="tìm-hiểu-cơ-bản-mạng-máy-tính.-các-mô-hình-mạng-pan-lan-man-wan.">Tìm hiểu cơ bản mạng máy tính. Các mô hình mạng PAN, LAN, MAN, WAN.</h2>
<ol>
<li>Mạng máy tính là gì?</li>
</ol>
<ul>
<li>Network là tập hợp các thiết bị có khả năng truyền dữ liệu và các thiết bị, hệ thống đầu cuối ( như user, server) được kết nối với nhau để có thể giao tiếp và truyền dược dữ liệu.</li>
</ul>
<ol start="2">
<li>Các thiết bị cơ bản của một hệ thống mạng.</li>
</ol>
<ul>
<li>User đầu cuối</li>
<li>Các đường link kết nối: connector, network interface card.</li>
<li>Những thiết bị tập trung: switch, hub, brigde.</li>
<li>Thiết bị định tuyến đường truyền: Router</li>
</ul>
<ol start="3">
<li>Topology mạng</li>
</ol>
<ul>
<li>Bus Topology</li>
<li>Star Topology</li>
<li>Ring Topology</li>
</ul>
<ol start="4">
<li>Các hình thức kết nối ra Internet.</li>
</ol>
<ul>
<li>ADSL (Asymetric Digital Subscriber Line): kỹ thuật sử dụng đường truyền cáp đồng điện thoại để kết nối cung cấp đường truyền Internet.</li>
<li>FTTH (Fiber to the Home) và FTTB (Fiber to the building): kỹ thuật sử dụng đường cáp quang do ISP (Internet Service Provider) kéo đến nhà hay cơ quan để cung cấp Internet.</li>
<li>Cable TV: mạng lưới truyền hình cáp truy cập Internet. Được các nhà cung cấp cáp truyền hình cung cấp đường truyền Internet kèm theo dịch vụ cáp truyền hình.</li>
<li>Leased Line: một loại hình truy cập Internet dành cho các doanh nghiệp. Các ISP sẽ cung cấp đường truyền đảm bảo về chất lượng dịch vụ truy cập Internet.</li>
</ul>
<ol start="5">
<li>Các mô hình PAN, LAN, MAN, WAN.</li>
</ol>
<ul>
<li>PAN (personal area network): mạng cá nhân dùng để kết nối các thiết bị cá nhân. Phạm vi 5m-10m.</li>
<li>LAN (Local Area Network): mạng cục bộ, dùng để kết nối các máy tính, thiết bị ngoại vi trong phạm vi một cơ quan,  phạm vi vài km</li>
<li>MAN (Metropolitan Area Network): mạng nội thị, để kết nối một vùng rộng lớn như một thành phố,  phạm vi vài chục km.</li>
<li>WAN (Wide Area Network): Mạng diện rộng, để kết nối các mạng LAN, MAN lại với nhau. Phạm vi vài trăm đến vài ngàn km.</li>
</ul>
<h2 id="mô-hình-osi-và-mô-hình-tcpip">Mô hình OSI và mô hình TCP/IP</h2>
<h3 id="protocol">Protocol</h3>
<ul>
<li>Protocol là một tập hợp các quy tắc chuẩn cho phép hai hoặc nhiều thực thể trong một hệ thống thông tin liên lạc để trao đổi thông tin, dữ liệu qua các kênh truyền thông.</li>
<li>Protocol sẽ định nghĩa các quy tắc (rule), cú pháp (syntax), ngữ nghĩa (semantics), sự đồng bộ (synchronization) trong quá trình truyền thông và có thể thêm phương pháp khắc phục lỗi trên đường truyền.</li>
<li>Một số protocol phổ biến: HTTP, TCP, IP, …</li>
</ul>
<h3 id="layers-of-osi-model">Layers of OSI Model</h3>
<ol>
<li>Physical Layer</li>
</ol>
<ul>
<li>Biến đổi dòng bit logic thành tín hiệu vật lý phù hợp với đường truyền vật lý (ở bên phát) và ngược lại (ở bên thu): điều chế/giải điều chế, biến đổi, khôi phục tín hiệu .v.v.</li>
<li>Hub, Repeater, Modem, Cables là các thiết bị của Physical Layer.</li>
</ul>
<ol start="2">
<li>Data Link Layer</li>
</ol>
<ul>
<li>Phát hiện và sửa lỗi khi truyền dữ liệu giữa các thực thể trong mạng (switch, router, thiết bị đầu cuối).</li>
<li>Nhận dữ liệu từ Network Layer, đóng gói dữ liệu Network Layer vào các frame phù hợp với mạng vật lý.</li>
<li>Tổ chức các bit trong frame theo thứ tự định nghĩa sẵn</li>
<li>Lớp Liên kết dữ liệu được xử lý bởi NIC  và trình điều khiển thiết bị của các máy chủ.<br>
*Switch &amp; Bridge là thiết bị Lớp liên kết dữ liệu.</li>
<li>Media Access Control (MAC) của người nhận và người gửi được đặt trong tiêu đề</li>
</ul>
<ol start="3">
<li>Network Layer</li>
</ol>
<ul>
<li>Lớp mạng hoạt động để truyền dữ liệu từ máy chủ này sang máy chủ khác nằm trong các mạng khác nhau. Nó cũng  lựa chọn đường đi ngắn nhất để truyền gói, từ số lượng đường có sẵn. Địa chỉ IP của người gửi và người nhận được đặt trong tiêu đề bởi lớp mạng.</li>
<li>Định tuyến: Các giao thức của lớp mạng xác định tuyến nào phù hợp từ nguồn đến đích. Chức năng này của lớp mạng được gọi là định tuyến.</li>
<li>Định địa chỉ logic: Để xác định duy nhất từng thiết bị trên kết nối internet, lớp mạng xác định sơ đồ định địa chỉ. Địa chỉ IP của người gửi và người nhận được đặt trong tiêu đề theo lớp mạng. Một địa chỉ như vậy phân biệt từng thiết bị duy nhất và phổ biến.</li>
<li>Lớp mạng được thực hiện bởi các thiết bị mạng như Router.</li>
</ul>
<ol start="4">
<li>Transport Layer</li>
</ol>
<ul>
<li>Đảm bảo truyền dữ liệu tin cậy giữa 2 thiết bị đầu cuối (end-to-end)</li>
<li>Điều khiển luồng (flow control)</li>
<li>Chia nhỏ hoặc ghép các khối dữ liệu từ lớp Phiên.</li>
<li>Dữ liệu trong lớp truyền tải được gọi là <em>segments</em></li>
</ul>
<ol start="5">
<li>Session Layer</li>
</ol>
<ul>
<li>Quản lý các kết nối (connection) được thiết lập trên cùng một máy tính, từ một hay nhiều ứng dụng khác nhau.</li>
<li>Ghép kênh nhiều kết nối và gửi xuống lớp Transport.</li>
</ul>
<ol start="6">
<li>Presentation Layer</li>
</ol>
<ul>
<li>Biến đổi định dạng dữ liệu từ các ứng dụng thành một định dạng chung được quy định bởi thiết bị đầu cuối.</li>
</ul>
<ol start="7">
<li>Application Layer</li>
</ol>
<ul>
<li>Cung cấp các giao diện lập trình cho ứng dụng của người sử dụng.</li>
</ul>
<h3 id="layers-of-tcpip">Layers of TCP/IP</h3>
<ol>
<li><em>Application Layer :</em>  Lớp này thực hiện các chức năng của ba lớp trên cùng của mô hình OSI: Ứng dụng, Trình bày và Lớp phiên. Nó chịu trách nhiệm về giao tiếp từ nút đến nút và kiểm soát các thông số kỹ thuật của giao diện người dùng. Một số giao thức có trong lớp này là: HTTP, HTTPS, FTP, TFTP, Telnet, SSH, SMTP, SNMP, NTP, DNS, DHCP, NFS, X Window, LPD.</li>
<li><em>Transport Layer:</em>  Lớp này tương tự như lớp truyền tải của mô hình OSI. Nó chịu trách nhiệm giao tiếp đầu cuối và cung cấp dữ liệu không bị lỗi. Nó bảo vệ các ứng dụng lớp trên khỏi sự phức tạp của dữ liệu. Hai giao thức chính có trong lớp này là: TCP và UDP.</li>
<li><em>Internet</em>  Layer: hoạt động như tầng Network OSI. Đặc trưng và được sử dụng rộng rải của tầng này là giao thức IP, ICMP, ARP.</li>
<li><em>Network Access Layer</em>: có vai trò của 2 lớp Data Link và Physical của mô hình OSI.</li>
</ol>
<h3 id="cách-thức-hoạt-động">Cách thức hoạt động</h3>
<ol>
<li>Service Data Unit</li>
</ol>
<ul>
<li>Service Data Unit là một đơn vị dữ liệu đã được truyền từ lớp trên xuống lớp thấp hơn. Đơn vị dữ liệu (SDU) này vẫn chưa được đóng gói thành đơn vị dữ liệu giao thức (PDU) bởi lớp dưới.</li>
</ul>
<ol start="2">
<li>Protocol Data Unit</li>
</ol>
<ul>
<li>Khi các gói tin đi từ lớp Application xuống lớp Physical. Các giao thức đặc trưng của mỗi lớp sẻ quy định cách thức đóng gói dữ liệu. Các gói tin này được gọi là PDU (Protocol Data Unit) các gói tin PDU gồm 2 phần là Header (Phần thông tin quản lý gói tin của các tầng) và Data (dữ liệu thực của gói tin được truyền).</li>
</ul>
<ol start="3">
<li>Mô tả hoàn thiện 1 gói tin từ đầu vào người dùng tới lúc được được đóng gói gửi đi</li>
</ol>
<ul>
<li>Data đi từ lớp Application qua các lớp dưới cho đến khi đến lớp Physical.</li>
<li>Gói tin PDU đi từ trên xuống dưới chúng sẻ được đóng gói thành data lớp bên dưới và được đóng thêm header của tầng dưới.</li>
<li>Cứ xuống thêm một tầng thì sẻ có một header được thêm vào. Đặc biệt ở tầng Data Link , gói tin sẻ được đóng thêm một trường kiểm soát lỗi FCS (phần trailer).</li>
<li>Đến tầng 7, các gói tin PDU sẽ được chuyển sang dạng bit (0,1).</li>
</ul>

