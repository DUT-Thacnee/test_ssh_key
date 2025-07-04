
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
