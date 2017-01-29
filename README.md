
# 1. Telnet
- là tầng giao thức thuộc lớp ứng đụng (app), cho phép truy nhập điều khiển các thiết bi ở khoảng cachy xa
- kết nôi TCP và port 23
- điều kiện để thực hiện telnet
  - địa chỉ ip từ thiết bị phải ping thàng công được đến router ở xa
  - router phải mở cổng VTY (sử dụng password) :
  
  ```````
  Router(config)#line vty 0 4
  router(config-line)#password [pass]
  router(config-line)#login
  ``````
  
 # 2. CDP (cisco discovery protocol)
 - là giao thức sử dụng cho các thiết bị Cisco, thuộc lớp 2
 - cho phép thu nhập thông tin về các thiết bị lân cận (mỗi 60s sẽ gửi đi một CDP message)
 - CDP cho biết thông tin của các thiết bị lân cận như: hostname,local-interface, outgoing port, platform, capability, IP láng giềng, IOS version
 
 `````````
 router#show cdp neighbor
 ``````
 
 hoặc
 
 ``````
 router#show cdp neighbor detail
 router#show cdp entry *
 ```````
 
 - để tắt CPD: router(config)#no cdp run
 - để tắt CDP láng giềng : router(config)#no cdp enable
 
 # 3.SSH
 - là giao thức thuộc tầng ứng dụng phục vụ cho việc truy nhập từ xa, chạy trên nền TCP port 22
 - cung cấp cơ chế mã hoa toàn bộ dữ liệu
 
