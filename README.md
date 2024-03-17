# HCMUT Thesis/Dissertation Template

## How to run
Youtube: https://www.youtube.com/watch?v=4lyHIQl4VM8&t=648s&ab_channel=FedericoTartarini

## Một số gợi ý về sử dụng

- Để đơn giản, demo chỉ bao gồm 1 file `demo-Chapter1.tex` và đặt ngay trong thư mục gốc, tuy nhiên nếu nhiều chương hay mỗi chương lại có nhiều section dài (đủ tách ra nhỏ hơn để viết cho gọn) thì nên tổ chức vào các thư mục con, tuy nhiên cũng không nên tách quá nhỏ vì sẽ rối
- figures nên được để trong 1 thư mục riêng, e.g., `figs`, và trong đó mỗi chapter nên có 1 thư mục con tương ứng (`figs/intro`, `figs/related-word`, etc.)
- Thực sự có chút khác biệt về font `Times New Roman` trên `latex`, setup hiện tại là đủ dùng trong phần lớn trường hợp, có thể tham khảo thêm về font tại đây https://tex.stackexchange.com/questions/270571/latex-12pt-is-different-from-actual-font-size-12-on-microsoft-word . Tuy nhiên, điều đó trong phần lớn các trường hợp là không thực sự cần thiết.

## Điều chỉnh lại (số) thứ tự trích dẫn

Thường được làm khi đã hoàn thiện báo cáo, sắp in ra và muốn tự điều chỉnh lại thứ thứ theo mong muốn/quy định hơi khác biệt mà các style có sẵn chưa có:
ví dụ, `trích dẫn tiếng Việt đưa lên trước` rồi mới tới các tài liệu tiếng Anh

(áp dụng với Overleaf, nếu build offline thì cũng tìm file tương tự)

- vào `Logs and output files` để tìm và lấy về file `output.bbl`
- copy toàn bộ nội dung file đó, lưu lại với tên mới (e.g., `manually.bbl`)
- Điều chỉnh lại theo thứ tự mình muốn/quy định, ví dụ, trích dẫn tiếng Việt đưa lên trước
- mở file `thesisdemo.tex` (hoặc file main mà bạn đã `đổi tên`)
- comment 2 dòng bibliography tự động sau:

  \bibliographystyle{plain} % ieeetr
  \bibliography{refs}

- bỏ comment cho dòng sau để dùng chế độ manually
        \input{manually.bbl}

Hoan nghênh mọi góp ý cũng như đóng góp của các bạn.
