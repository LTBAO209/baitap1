<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website của tôi</title>
    <link rel="stylesheet" href="styles.css">
    <script src="script.js" defer></script>
    <style> 
        body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #e0f7fa; 
}
header {
    background-color: #00796b;
    color: white;
    padding: 1em 0;
    text-align: center;
}
nav ul {
    list-style: none;
    padding: 0;
    background-color: #004d40;
    text-align: center;
}
nav ul li {
    display: inline;
    margin: 0 10px;
}
nav ul li a {
    color: white;
    text-decoration: none;
}
main {
    padding: 20px;
}
section {
    margin-bottom: 20px;
}
footer {
    background-color: #00796b;
    color: white;
    text-align: center;
    padding: 1em 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}
form {
    display: flex;
    flex-direction: column;
}
form label {
    margin-top: 10px;
}
form input, form textarea {
    margin-top: 5px;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
}
form input[type="submit"] {
    margin-top: 20px;
    background-color: #00796b;
    color: white;
    border: none;
    cursor: pointer;
}
form input[type="submit"]:hover {
    background-color: #004d40;
}
    </style>
</head>
<body>
    <header>
        <h1>Chào mừng đến với website của tôi</h1>
    </header>
    <nav>
        <ul>
            <li><a href="#" onclick="showSection('home')">Trang chủ</a></li>
            <li><a href="#" onclick="showSection('study-plan')">Kế hoạch học tập</a></li>
            <li><a href="#" onclick="showSection('hobbies')">Sở thích</a></li>
            <li><a href="#" onclick="showSection('contact')">Liên hệ</a></li>
        </ul>
    </nav>
    <main>
        <section id="home">
            <h2>SINH VIÊN ĐH SƯ PHẠM TPHCM</h2>
            <p>Họ tên: LÊ THẾ BẢO</p>
            <p>Tuổi: 18</p>
            <p>Ngày sinh: 20/09/2006</p>
            <p>Điện thoại: 0773721369</p>
            <p>Địa chỉ: 100 LÝ PHỤC MAN Q7 TP.HCM</p>
            <p>Email: LETHEBAO@.GMAILCOM</p>
        </section>
        <section id="study-plan" style="display:none;">
            <h2>Kế hoạch học tập</h2>
            <p>HỌC TRÊN LỊCH HỌC.</p>
        </section>
        <section id="hobbies" style="display:none;">
            <h2>Sở thích</h2>
            <p>nghe truyện, nghe nhạc.</p>
        </section>
        <section id="contact" style="display:none;">
            <h2>Liên hệ</h2>
            <form>
                <label for="name">Họ tên:</label>
                <input type="text" id="name" name="name"><br><br>
                <label for="message">Nội dung:</label>
                <textarea id="message" name="message"></textarea><br><br>
                <label for="email">Email:</label>
                <input type="email" id="email" name="email"><br><br>
                <input type="submit" value="Gửi">
            </form>
            <div id="map">
                <img src="C:\Users\Le The Bao\Pictures\Screenshots\Ảnh chụp màn hình (12).png" height="300" width="400" alt="bản đồ từ nhà tới trường">
            </div>
        </section>
    </main>
    <footer>
        <p>&copy; HELLO mấy bồ đến web của tôi</p>
    </footer>
</body>
</html>
<script>
    function showSection(sectionId) {
    const sections = document.querySelectorAll('main section');
    sections.forEach(section => {
        section.style.display = 'none';
    });
    document.getElementById(sectionId).style.display = 'block';
}
 </script>
.
