Cài đặt bằng hai giải pháp:

Giải pháp 1: Các bạn xem các frame độc lập nhau, áp dụng PCA độc lập nhau, sau đó concatenate các ma trận sau khi đã nén lại.

Giải pháp 2: Các bạn reshape các frame kích thước H x W về "vector" kích thước HW x 1

Sau đó concate các vector lại thành ma trận HW x C ==> áp dụng PCA
