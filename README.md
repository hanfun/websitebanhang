# websitebanhang
Chức năng

Thiết kế database website bán hàng bao gồm

Front end:
  Tat cả các bảng phai ... ngoài ra còn có ngày tạo, ngày cập nhật, nguoi tạo, nguoi cap nhat
  - Product ( Name, Image, Price, Price Discount, Status ) 
  - Category( Name, Image, Status )
  - User: nguoi dùng mua hàng phan biet voi user admin nhung phai cung table ( user name, password, trang thai, picker, quyen )
  - Tạo Order danh sach các san phan , tong tien khi mua cua tung san pham, trang thai cua order ( moi tao, xac nhan, dang van chuyen, da giao, da huy)
  - Danh sach cac order của 1 user
  - Customer phai dang ky thanh vien thi moi duoc tao order ngoai ra thi chi add cart ko co nut submit tao order khi chua login ( dang ky phai co capchar)
  Nang cao: Tạo captcha khi dang ky, gui mail xac nhan click vao mail de active user
Back end:
  Customer là chi khac hang o ngoai front end
  User admin la nhung user quan tri he thong
  -- Cho phep user quyen admin login vao
  -- Quan ly user
      --- Quan ly user la customer: danh sach, filter
      --- Quan ly user la admin ( tao user, edit user: bao gom phan quyen cho no, delete user) 
  -- Danh sach Category
  -- Product: Danh sach san pham, tạo sp, xóa sp, edit sp ( chọn category cho sp )
  -- Danh sach Order, edit order
  --- Danh sach banner hien o trang chu ( Tao, sua, xoa ) bao gom banner top, banner bottom
 Cấu trúc trang web front end
  -------------> Trang chu
              Header ------------Thanh search------DropDown menu ( Login, Logout, Signup, Danh sach Order ) Button Giỏ hàng 
              Banner Top
              Danh sach 5 Category duoc setup de hien o trang chu    
 Menu bên trai la danh sach category ( Anh - Ten ) click vao thi quan Page category                  
              Content ở giưa  là 20 product duoc admin chi dinh hien ra o trang chu
              Footer
 --------------> Page Search
              Khi bấm vào thanh search và submit thì sẽ quan page search
              Hiện ra các sản phẩm liên quan toi keyword search ( Có phân trang 20 product / page )
 --------------> Page Product detail
              Khi click vào 1 san pham thi show thong tin của sp đó ra Button add cart )
 ---------------> Page category
              Khi click 1 category ở trang chu thi qua đây sẽ load các product của category đó ( có phân trang 20 product / page )
 --------------> Page Cart
              Danh sach cac sp duoc customer add vao
 --------------> Page confirm
              Kiem tra login neu chua login thi đá về page cart
              Nếu login rồi thi show danh sách sp trong cart
              Có nut submit để tiến hành thanh toán
 --------------> Page Thank
              Khi click thanh toán từ page Confirm thì show ra mã đơn hàng đã tạo
 --------------> Page list order: show ra danh sách các order của 1 user
 --------------> Page order detail: Khi click 1 item ở page list order thì show ra các order item của order đó 
    
 
