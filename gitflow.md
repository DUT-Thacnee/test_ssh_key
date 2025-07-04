
Develop Environment
Develop - Nhánh để developer code -> Nhánh này để build môi trường Develop
-------------------------------------------------------------------------------------------
Feature - Nhánh này dùng để đặt tên cho các tính năng của 1 nhánh
        -> chức năng login -> feature/login
        -> Chức năng nhận diện khuôn mặt -> feature/face-detect
        -> Nhánh feature merge vào Develop
Fix     - Nhánh này dùng để fix 1 hoặc 1 số lỗi ở trên nhánh Develop
        -> Nhánh fix merge vào Develop

Production Environment
-------------------------------------------------------------------------------------------
HotFix  - Khác nhánh fix
        - Hotfix nó được tạo ra từ main để fix những lỗi nghiêm trọng từ main 
            trong khi đó nhánh fix chỉ được tạo ra khi fix lỗi từ develop
        - Nhánh develop release lên nhánh main
        - Giả sử nhánh main có lỗi A -> hotfix lỗi A sau đó phải cập nhật fix luôn lỗi của nhánh 
        Develop để nó được đồng bộ với nhánh main.

Release - v1.0 Đưa cho khách hàng dùng với 10 features -> chạy ngon rồi
        - v1.2 Đưa cho khách hàng dùng thêm 2 features -> Chạy lỗi 
        -> Rollback về v1.0 hoặc tạo ra v1.3 để fix lỗi của v1.2
        - Code xong 10 features rồi chừ đưa cho khách  hàng dùng bằng cách tạo ra 1 bản release 
        hoặc đẩy vào main rồi tạo bản release
        - v1.5-beta, v1.6-rc1.2.44
        - Nếu case không cần phức tạp hoá -> đẩy thẳng develop lên nhánh main
        - Nếu case chuẩn đúng qui trình -> tạo ra 1 bản release -> thử nghiệm sau đó đẩy vào main

