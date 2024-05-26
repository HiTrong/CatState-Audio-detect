- _Ngày bắt đầu nghiên cứu: 01/05/2024_
- _Ngày bắt đầu dự án: 26/05/2024_

# Tensorflow - Cat State Detect - Project

![Ảnh minh họa mèo](https://i.ytimg.com/vi/HIdLXBn-Py0/maxresdefault.jpg)

# 1. Tổng quan về Project

Project được thực hiện dựa trên nền tảng Python nhằm tìm hiểu về khám phá cách Deep Learning (Cụ thể là CNN) được áp dụng cho bài toán phân loại dựa trên file âm thanh (Audio). Với mục tiêu là xây dựng một hệ thống có thể phân loại được trạng thái của mèo dựa trên âm thanh **'Meow'** của mèo. Qua đó có thể đoán được mèo đang muốn điều gì cần gì. 

# 2. Tổng quan về tập dữ liệu

Nguồn: [Cat Meow Classification - Kaggle](https://www.kaggle.com/datasets/andrewmvd/cat-meow-classification/data)
Mô tả: 
- Loài người đã cố gắng vươn tới các vì sao, tuy nhiên họ vẫn gặp khó khăn trong việc hiểu những người bạn mèo của chúng ta.
Với tập dữ liệu này, bạn có thể đóng góp cho nhiệm vụ liên quan này và có lẽ một ngày nào đó chúng tôi sẽ có thể dịch tiếng kêu của chúng - để chúng có thể chính thức nói với chúng tôi rằng chúng tôi thực tế là thú cưng của chúng.
- Tập dữ liệu này, bao gồm 440 bản ghi âm, chứa tiếng meo meo do mèo phát ra trong các bối cảnh khác nhau. Cụ thể, 21 con mèo thuộc 2 giống (Maine Coon và European Shorthair) đã nhiều lần được tiếp xúc với ba kích thích khác nhau đóng vai trò là nhãn hiệu để dự đoán: Waiting for food **(Chờ được ăn)**; Isolation in unfamiliar environment **(Bị cô lập trong môi trường xa lạ)**; Brushing (being brushed affectionately by the owner)**(Muốn được _chải chuốt_ bởi chủ nhân)**.

Các tập tin chứa meo meo nằm trong thư mục "dataset". Chúng là các luồng PCM (.wav).

Quy ước đặt tên tuân theo mẫu: L[label]_CID[Cat ID]_BB[Cat Breed]_SS[Sex]_OID[Owner ID]_R[Recording Session]XX[Meow counter].

Các tệp dữ liệu là unique trong "dataset"

Thư mục "extra" chứa các bản ghi âm bị loại trừ (âm thanh không phải là tiếng meo meo do mèo phát ra) và các chuỗi phát âm gần gũi chưa bị cắt. Nó có thể được sử dụng như một lớp thứ 4.

# 3. Xây dựng mô hình 
Mời bạn xem file notebook [tại đây!](https://github.com/HiTrong/CatState-Audio-detect/CatStateDetection.ipynb)

# 4. Lời kết và tài liệu tham khảo
Project đã mang lại cho chúng ta cái nhìn về cách tiền xử lý âm thanh cũng như đưa bài toán xử lý âm thanh về xử lý hình ảnh với mô hình Deep Learning (**CNN**). Song còn nhiều khuyết điểm chưa tối ưu trong mô hình nhưng tổng quan lại ta đã có thật nhiều kiến thức hữu ích. Cảm ơn đã đọc đến cuối

_TÀI LIỆU THAM KHẢO:_
- LARXEL. "Cat Meow Classification Dataset." Kaggle, https://www.kaggle.com/datasets/andrewmvd/cat-meow-classification/data.
- Tiensu. "Audio Deep Learning Part 1." Tiensu Blog, https://tiensu.github.io/blog/67_audio_deep_learning_part_1/.
- ljnktjnk. "Xử lý dữ liệu âm thanh." Viblo, https://viblo.asia/p/xu-ly-du-lieu-am-thanh-Qpmlezg95rd.