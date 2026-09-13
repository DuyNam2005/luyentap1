A. Câu hỏi ôn tập lý thuyết
Câu 1. Khái niệm phát triển ứng dụng mobile đa nền tảng

Phát triển ứng dụng mobile đa nền tảng (Cross-platform Mobile Development) là phương pháp xây dựng ứng dụng có thể chạy trên nhiều hệ điều hành khác nhau như Android và iOS bằng cách sử dụng chung một phần lớn mã nguồn.

Thay vì phải xây dựng hai ứng dụng riêng biệt, ví dụ Android dùng Java/Kotlin và iOS dùng Swift, lập trình viên có thể sử dụng một công nghệ như React Native để viết một codebase và sử dụng cho cả hai nền tảng.

Việc sử dụng một cơ sở mã nguồn chung mang lại nhiều lợi ích. Đầu tiên, thời gian phát triển được rút ngắn vì lập trình viên không phải viết lại cùng một chức năng hai lần. Ví dụ, chức năng đăng nhập, hiển thị sản phẩm, giỏ hàng có thể được viết một lần rồi sử dụng trên cả Android và iOS.

Thứ hai, chi phí phát triển cũng giảm vì doanh nghiệp không cần duy trì hai nhóm lập trình viên riêng biệt cho Android và iOS. Ngoài ra, việc bảo trì và cập nhật ứng dụng cũng đơn giản hơn do phần lớn mã nguồn được dùng chung.

Tuy nhiên, trong một số trường hợp cần hiệu năng rất cao hoặc sử dụng nhiều tính năng đặc thù của hệ điều hành thì phát triển Native vẫn có thể phù hợp hơn.


Câu 2. Sự cần thiết của phát triển ứng dụng đa nền tảng

Hiện nay người dùng sử dụng nhiều loại thiết bị khác nhau, trong đó phổ biến nhất là thiết bị Android và iOS. Nếu doanh nghiệp chỉ phát triển ứng dụng trên một nền tảng thì sẽ bỏ qua một lượng lớn người dùng ở nền tảng còn lại.

Phát triển đa nền tảng giúp doanh nghiệp xây dựng ứng dụng có thể tiếp cận người dùng trên nhiều hệ điều hành mà không cần phát triển riêng hoàn toàn từng ứng dụng.

Một số lợi ích chính gồm:

Giảm thời gian phát triển.
Giảm chi phí nhân sự.
Dùng chung phần lớn mã nguồn.
Dễ bảo trì và nâng cấp.
Có thể phát hành Android và iOS gần như cùng thời điểm.
Giao diện và chức năng giữa hai nền tảng dễ đồng bộ hơn.

Doanh nghiệp nên ưu tiên giải pháp đa nền tảng khi cần đưa sản phẩm ra thị trường nhanh, ngân sách có giới hạn, ứng dụng không yêu cầu xử lý đồ họa hoặc hiệu năng quá cao và cần hỗ trợ cả Android lẫn iOS.

Ví dụ, các ứng dụng như bán hàng, đặt lịch, học trực tuyến, đọc tin tức, quản lý công việc hoặc mạng xã hội cơ bản đều khá phù hợp với React Native.

Ngược lại, nếu ứng dụng là game 3D nặng, ứng dụng xử lý đồ họa phức tạp hoặc phụ thuộc rất sâu vào phần cứng của điện thoại thì Native có thể là lựa chọn tốt hơn.


Câu 3. React Native là gì và cách React Native hoạt động?

React Native là framework phát triển ứng dụng mobile đa nền tảng do Meta phát triển. React Native cho phép lập trình viên sử dụng JavaScript/TypeScript và React để xây dựng ứng dụng chạy trên Android và iOS.

Điểm đặc biệt của React Native là giao diện ứng dụng không đơn giản là trang web chạy bên trong ứng dụng mà sử dụng các thành phần giao diện Native thực sự của hệ điều hành.

Quy trình hoạt động có thể hiểu đơn giản như sau:

Code JavaScript / React Native
            ↓
      JavaScript Engine
            ↓
   Bridge / Native Module
            ↓
      Native Components
            ↓
     Android / iOS UI
JavaScript Engine

JavaScript Engine chịu trách nhiệm thực thi mã JavaScript trong ứng dụng.

Ví dụ:

const name = "Nguyen Van A";

function hello() {
    console.log("Hello " + name);
}

Đoạn code trên sẽ được JavaScript Engine xử lý.

Trong các phiên bản React Native hiện đại, engine thường được sử dụng là Hermes.

Bridge

Bridge có nhiệm vụ giúp phần JavaScript giao tiếp với các chức năng Native của Android hoặc iOS.

Ví dụ khi JavaScript yêu cầu:

Mở camera

thì React Native có thể gọi chức năng camera của hệ điều hành thông qua các module Native.

Ở kiến trúc React Native mới, cơ chế giao tiếp đã được cải tiến đáng kể so với mô hình Bridge cũ, nhưng khái niệm Bridge vẫn thường được sử dụng để giải thích nguyên lý cơ bản.

Native Views

Native Views là các thành phần giao diện thật của Android hoặc iOS.

Ví dụ React Native:

<View>
    <Text>Hello React Native</Text>
    <Button title="Login" />
</View>

Các component này sẽ được ánh xạ thành những thành phần giao diện tương ứng trên Android hoặc iOS.

Nhờ vậy React Native có thể tạo trải nghiệm gần với ứng dụng Native nhưng vẫn cho phép chia sẻ phần lớn mã nguồn.


Câu 4. So sánh Native và React Native
Native
Ưu điểm:

Hiệu năng tốt nhất.
Truy cập đầy đủ tính năng hệ điều hành.
Tối ưu tốt cho từng thiết bị.
Phù hợp ứng dụng có yêu cầu cao về phần cứng.

Nhược điểm:

Phải xây dựng riêng Android và iOS.
Tốn thời gian.
Chi phí cao.
Khó duy trì nếu đội phát triển nhỏ.

React Native
Ưu điểm:

Một codebase cho nhiều nền tảng.
Phát triển nhanh.
Giảm chi phí.
Dễ bảo trì.
Phù hợp với lập trình viên đã biết JavaScript hoặc React.

Nhược điểm:

Một số chức năng đặc thù vẫn cần Native Module.
Một số trường hợp hiệu năng thấp hơn Native.
Debug đôi khi phức tạp khi lỗi liên quan đến cả JavaScript và Native.


Câu 5. Kiến thức cần có khi học React Native

Để học React Native, người học nên nắm được các kiến thức cơ bản của JavaScript, JSX, Component, Props và State.

JavaScript

JavaScript là ngôn ngữ chính được sử dụng để xử lý logic trong React Native.

Ví dụ:

const price = 100000;
const quantity = 2;

const total = price * quantity;

Có thể dùng để xử lý tổng tiền trong ứng dụng bán hàng.

JSX

JSX cho phép viết giao diện gần giống HTML bên trong JavaScript.

Ví dụ:

<View>
    <Text>Xin chào React Native</Text>
</View>

JSX giúp code giao diện dễ đọc và dễ quản lý.

Component

Component là các khối giao diện có thể tái sử dụng.

Ví dụ:

function Product() {
    return (
        <View>
            <Text>Áo thun</Text>
        </View>
    );
}

Sau đó có thể sử dụng:

<Product />
<Product />
<Product />
Props

Props dùng để truyền dữ liệu từ component cha xuống component con.

function Product({ name }) {
    return <Text>{name}</Text>;
}

Sử dụng:

<Product name="Áo thun" />
<Product name="Quần jean" />
State

State dùng để quản lý dữ liệu có thể thay đổi.

Ví dụ:

const [count, setCount] = useState(0);

Có thể dùng để quản lý:

Số lượng sản phẩm.
Giỏ hàng.
Trạng thái đăng nhập.
Nội dung form.
Dữ liệu API.


B. Bài tập luyện tập thực hành
Bài tập 1 – Mức dễ
Chọn ứng dụng bán hàng trực tuyến

Ứng dụng bán hàng trực tuyến thường có các chức năng chính:

Đăng ký tài khoản.
Đăng nhập.
Xem danh sách sản phẩm.
Xem chi tiết sản phẩm.
Tìm kiếm sản phẩm.
Thêm sản phẩm vào giỏ hàng.
Đặt hàng.
Theo dõi đơn hàng.
Nhận thông báo khuyến mãi.

Ứng dụng này rất phù hợp để phát triển bằng React Native.

Lý do là phần lớn các chức năng của ứng dụng không yêu cầu xử lý phần cứng hoặc đồ họa quá phức tạp. React Native có thể chia sẻ phần lớn mã nguồn giữa Android và iOS.

Ngoài ra, React Native giúp quá trình phát triển nhanh hơn, tiết kiệm chi phí và giúp giao diện của hai phiên bản Android và iOS tương đối nhất quán.

Do đó, React Native là một lựa chọn phù hợp để phát triển ứng dụng bán hàng trực tuyến.


Bài tập 2 – Mức dễ đến trung bình
Nếu cần tối ưu hiệu năng cao, nên lựa chọn Native.


Bài tập 3 – Mức trung bình
Quy trình hoạt động cơ bản của React Native:

┌────────────────────────────┐
│      JavaScript Code       │
│ React + JSX + Components   │
└──────────────┬─────────────┘
               ↓
┌────────────────────────────┐
│     JavaScript Engine      │
│          Hermes            │
└──────────────┬─────────────┘
               ↓
┌────────────────────────────┐
│ Bridge / Native Interface  │
│       Native Modules       │
└──────────────┬─────────────┘
               ↓
┌────────────────────────────┐
│        Native Views        │
│     Android / iOS UI       │
└──────────────┬─────────────┘
               ↓
┌────────────────────────────┐
│       Màn hình thiết bị    │
└────────────────────────────┘

Đầu tiên lập trình viên viết mã bằng JavaScript hoặc TypeScript và sử dụng React Native Component.

JavaScript Engine chịu trách nhiệm thực thi phần JavaScript.

Khi ứng dụng cần sử dụng các chức năng của thiết bị như camera, GPS, thông báo hoặc bộ nhớ, React Native có thể giao tiếp với phần Native thông qua Native Module.

Sau đó giao diện được hiển thị bằng các Native View của Android hoặc iOS.

Nhờ kiến trúc này, React Native cho phép lập trình viên chia sẻ phần lớn mã nguồn nhưng vẫn sử dụng những thành phần giao diện Native, vì vậy trải nghiệm ứng dụng có thể gần với ứng dụng Native.


Bài tập 4 – Mức trung bình đến khó
Tình huống

Một cửa hàng thời trang muốn xây dựng ứng dụng bán hàng chạy trên Android và iOS.

Ứng dụng cần:

Giao diện đẹp.
Danh sách sản phẩm.
Chi tiết sản phẩm.
Giỏ hàng.
Đăng nhập người dùng.
Thông báo khuyến mãi.

Ngoài ra:

Thời gian triển khai ngắn.
Kinh phí giới hạn.
Nhóm phát triển có kinh nghiệm JavaScript/React.
Đề xuất

Trong trường hợp này, nên lựa chọn React Native.

Lý do đầu tiên là ứng dụng phải hoạt động trên cả Android và iOS. React Native cho phép chia sẻ phần lớn mã nguồn giữa hai nền tảng nên giảm được đáng kể thời gian phát triển.

Thứ hai, kinh phí của cửa hàng có giới hạn. Nếu sử dụng Native, doanh nghiệp có thể cần lập trình viên Android và lập trình viên iOS riêng. Với React Native, một nhóm phát triển có thể xây dựng ứng dụng cho cả hai nền tảng.

Thứ ba, đội phát triển đã có kinh nghiệm JavaScript và React nên việc chuyển sang React Native sẽ tương đối dễ dàng.

Các chức năng như:

Danh sách sản phẩm
Chi tiết sản phẩm
Giỏ hàng
Đăng nhập
Thông báo
API

đều có thể triển khai tốt bằng React Native.

Ứng dụng bán hàng cũng không yêu cầu xử lý đồ họa nặng như game 3D nên hiệu năng của React Native hoàn toàn có thể đáp ứng.

Kết luận: React Native là lựa chọn phù hợp hơn Native cho trường hợp này vì giúp giảm chi phí, rút ngắn thời gian phát triển và tận dụng được kỹ năng sẵn có của nhóm lập trình viên.


Bài tập 5 – Mức khó

Để xây dựng môi trường phát triển React Native trên máy tính cá nhân, có thể chuẩn bị các công cụ sau.

1. Node.js
Node.js cung cấp môi trường để chạy JavaScript bên ngoài trình duyệt và hỗ trợ các công cụ của React Native.

2. npm hoặc Yarn
npm/Yarn được sử dụng để quản lý thư viện của project.

3. Java JDK
JDK cần thiết cho quá trình build ứng dụng Android.

4. Android Studio
Android Studio cung cấp môi trường và công cụ để phát triển ứng dụng Android.

5. Android SDK
Android SDK cung cấp các thư viện và công cụ cần thiết để biên dịch ứng dụng Android.

6. AVD Emulator
AVD là máy Android ảo.

7. Visual Studio Code
VS Code có thể được dùng để viết mã React Native.