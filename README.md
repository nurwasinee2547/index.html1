# index.html1<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>รวมการบ้านของ นูรวาซินีย์ เจ๊ะหามะ</title>
    <!-- Tailwind CSS CDN for easy styling -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom styles for the Inter font and general body */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f4f8; /* Light blue-gray background */
            color: #334155; /* Darker text color */
            display: flex;
            flex-direction: column; /* Use column for header, content, footer layout */
            justify-content: flex-start;
            align-items: center;
            min-height: 100vh;
            padding: 0; /* Remove padding from body as container will handle it */
            box-sizing: border-box;
        }
        .header {
            width: 100%;
            background-color: #1e293b; /* Dark blue-gray for header */
            color: white;
            padding: 15px 20px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap; /* Allow wrapping on smaller screens */
        }
        .header-title {
            font-size: 1.8rem;
            font-weight: bold;
            margin-right: 20px;
        }
        .nav-menu a {
            color: white;
            text-decoration: none;
            padding: 8px 15px;
            border-radius: 8px;
            transition: background-color 0.3s ease;
        }
        .nav-menu a:hover {
            background-color: #334155; /* Slightly lighter dark blue-gray on hover */
        }
        .main-content-wrapper {
            width: 100%;
            max-width: 900px;
            margin-top: 40px;
            margin-bottom: 40px;
            padding: 0 20px; /* Add horizontal padding for smaller screens */
            box-sizing: border-box;
            flex-grow: 1; /* Allow content to take available space */
        }
        .section-title {
            color: #1e293b;
            font-weight: bold;
            font-size: 2.2rem;
            text-align: center;
            margin-bottom: 30px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .section-title .icon-book {
            font-size: 2.5rem; /* Larger icon */
            margin-right: 15px;
            color: #3b82f6; /* Blue color for icon */
        }
        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); /* Responsive grid */
            gap: 25px; /* Space between cards */
            margin-bottom: 40px;
        }
        .card {
            background-color: #ffffff;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            display: flex;
            flex-direction: column;
            justify-content: space-between; /* Push button to bottom */
            transition: transform 0.2s ease, box-shadow 0.2s ease;
            border: 1px solid #e2e8f0;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.12);
        }
        .card-title {
            font-size: 1.4rem;
            font-weight: 600;
            color: #1e293b;
            margin-bottom: 10px;
        }
        .card-description {
            font-size: 0.95rem;
            color: #546e7a;
            margin-bottom: 20px;
            flex-grow: 1; /* Allow description to take space */
        }
        .card-button {
            background-color: #2563eb; /* Blue button */
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 10px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.2s ease;
            display: inline-block; /* Make it behave like a block for full width */
            width: 100%; /* Full width button */
            text-align: center;
            text-decoration: none; /* Remove underline for button links */
        }
        .card-button:hover {
            background-color: #1d4ed8; /* Darker blue on hover */
            transform: translateY(-1px);
        }
        .footer {
            width: 100%;
            background-color: #334155; /* Darker blue-gray for footer */
            color: white;
            padding: 20px 20px;
            text-align: center;
            margin-top: auto; /* Push footer to the bottom */
            border-top-left-radius: 10px;
            border-top-right-radius: 10px;
        }
        .footer p {
            margin-bottom: 5px;
            font-size: 0.9rem;
        }
        /* Responsive adjustments */
        @media (max-width: 768px) {
            .header {
                flex-direction: column;
                align-items: flex-start;
            }
            .nav-menu {
                margin-top: 10px;
                width: 100%;
                display: flex;
                flex-direction: column;
                align-items: flex-start;
            }
            .nav-menu a {
                width: 100%;
                text-align: left;
                margin-bottom: 5px;
            }
            .main-content-wrapper {
                margin-top: 20px;
                margin-bottom: 20px;
            }
            .section-title {
                font-size: 1.8rem;
            }
            .section-title .icon-book {
                font-size: 2rem;
            }
            .card-grid {
                grid-template-columns: 1fr; /* Single column on small screens */
            }
        }
    </style>
</head>
<body>
    <header class="header">
        <div class="header-title"></div> <!-- Removed "พอร์ตโฟลิโอการบ้าน" -->
        <nav class="nav-menu">
            <!-- ลิงก์ "หน้าหลัก" จะนำไปยังโปรแกรม BMI (เปิดในแท็บใหม่) -->
            <a href="https://nurwasinee2547.github.io/bmi-calculator-app/" target="_blank">หน้าหลัก</a>
            <!-- ลิงก์ภายในหน้า เพื่อเลื่อนไปยังส่วนต่างๆ -->
            <a href="#assignments">การบ้าน</a>
            <a href="#projects">โปรเจกต์</a>
            <!-- ลิงก์ไปยังโปรแกรม BMI ของคุณ (จะเปิดในแท็บใหม่) -->
            <a href="https://nurwasinee2547.github.io/bmi-calculator-app/" target="_blank">โปรแกรม BMI</a>
        </nav>
    </header>

    <div class="main-content-wrapper" id="top">
        <!-- Removed the h1 tag and the welcome paragraph -->
        
        <h2 id="assignments" class="section-title">
            <span class="icon-book">&#128214;</span> รายการบทเรียน
        </h2>
        <div class="card-grid">
            <!-- New Card for Assignment 1 -->
            <div class="card">
                <h3 class="card-title">การบ้านครั้งที่ 1: การรับค่าและแสดงผล</h3>
                <p class="card-description">โปรแกรมรับข้อมูลผู้ใช้ (ชื่อ, อายุ) และแสดงผล</p>
                <a href="https://nurwasinee2547.github.io/user-info-assignment/" target="_blank" class="card-button">ดูโปรแกรม</a>
            </div>

            <!-- New Card for Assignment 2 -->
            <div class="card">
                <h3 class="card-title">การบ้านครั้งที่ 2: การใช้ if-else และ switch case</h3>
                <p class="card-description">โปรแกรมคำนวณเกรดจากคะแนนที่ป้อน</p>
                <a href="https://nurwasinee2547.github.io/grade-calculator-assignment/" target="_blank" class="card-button">ดูโปรแกรม</a>
            </div>

            <!-- Existing Cards (example placeholders) -->
            <div class="card">
                <h3 class="card-title">บทที่ 1: การสร้างหน้าเว็บส่วนตัว</h3>
                <p class="card-description">ตัวอย่างการสร้างโครงสร้าง HTML พื้นฐานและการจัดสไตล์ CSS</p>
                <a href="https://github.com/nurwasinee2547/web-programming-assignment-1" target="_blank" class="card-button">ดูโปรแกรม</a>
            </div>
            
            <div class="card">
                <h3 class="card-title">บทที่ 2: การออกแบบฟอร์มติดต่อ</h3>
                <p class="card-description">ตัวอย่างการสร้างฟอร์ม HTML และการจัดการข้อมูลเบื้องต้น</p>
                <a href="https://github.com/nurwasinee2547/web-programming-assignment-2" target="_blank" class="card-button">ดูโปรแกรม</a>
            </div>

            <div class="card">
                <h3 class="card-title">บทที่ 3: การเรียงลำดับข้อมูล</h3>
                <p class="card-description">ตัวอย่างการใช้อัลกอริทึมการเรียงลำดับข้อมูล</p>
                <a href="https://github.com/nurwasinee2547/data-structures-assignment-1" target="_blank" class="card-button">ดูโปรแกรม</a>
            </div>

            <div class="card">
                <h3 class="card-title">บทที่ 4: การค้นหาแบบกราฟ</h3>
                <p class="card-description">ตัวอย่างการใช้อัลกอริทึมการค้นหาข้อมูลในโครงสร้างกราฟ</p>
                <a href="https://github.com/nurwasinee2547/data-structures-assignment-2" target="_blank" class="card-button">ดูโปรแกรม</a>
            </div>

            <div class="card">
                <h3 class="card-title">โปรเจกต์สุดท้าย: เว็บไซต์ E-commerce</h3>
                <p class="card-description">โปรเจกต์การสร้างเว็บไซต์ E-commerce อย่างง่าย</p>
                <a href="https://github.com/nurwasinee2547/web-programming-final-project" target="_blank" class="card-button">ดูโปรแกรม</a>
            </div>
            
            <!-- เพิ่มการบ้านอื่นๆ ที่นี่ในรูปแบบ Card -->
        </div>

        <h2 id="projects" class="section-title">โปรแกรมที่ออกแบบ</h2>
        <div class="card-grid">
            <!-- Card for BMI Calculator Program -->
            <div class="card">
                <h3 class="card-title">โปรแกรมคำนวณดัชนีมวลกาย (BMI)</h3>
                <p class="card-description">โปรแกรมสุขภาพที่คุณออกแบบและพัฒนาขึ้นเอง</p>
                <!-- ลิงก์ไปยัง GitHub Pages ของโปรแกรม BMI -->
                <a href="https://nurwasinee2547.github.io/bmi-calculator-app/" target="_blank" class="card-button">ดูโปรแกรม</a>
            </div>
        </div>
    </div>

    <footer class="footer">
        <p>จัดทำโดย: นูรวาซินีย์ เจ๊ะหามะ</p>
        <p>รหัสนักศึกษา: 6611425018</p>
        <p>สาขา: วิทยาการคอมพิวเตอร์</p>
        <p>IG:@_nurwasinee_</p>
    </footer>
</body>
</html>
