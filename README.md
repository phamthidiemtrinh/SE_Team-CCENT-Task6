
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
 - 
