
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>أكاديمية التدريب والتطوير | ACADEMY FOR TRAINING</title>
    <!-- استيراد خط جـوجل (Almarai) -->
    <link href="fonts.googleapis.com" rel="stylesheet">
    
    <style>
        :root {
            --primary-color: #2c3e50; /* كحلي غامق */
            --secondary-color: #3498db; /* أزرق فاتح */
            --accent-color: #e67e22; /* برتقالي للتمييز */
            --bg-light: #f4f7f6;
            --white: #ffffff;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Almarai', sans-serif;
        }

        body {
            background-color: var(--bg-light);
            color: var(--primary-color);
            line-height: 1.6;
        }

        /* الهيدر (Header) */
        header {
            background-color: var(--white);
            padding: 20px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo {
            font-weight: 800;
            font-size: 1.5rem;
            color: var(--primary-color);
            text-decoration: none;
        }

        nav a {
            margin-right: 20px;
            text-decoration: none;
            color: var(--primary-color);
            font-weight: 700;
            transition: 0.3s;
        }

        nav a:hover {
            color: var(--secondary-color);
        }

        /* القسم الرئيسي (Hero Section) */
        .hero {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: var(--white);
            padding: 100px 5%;
            text-align: center;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }

        .btn {
            background-color: var(--accent-color);
            color: var(--white);
            padding: 12px 30px;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            transition: 0.3s;
            display: inline-block;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
        }

        /* قسم الخدمات/المميزات */
        .services {
            padding: 80px 5%;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .service-card {
            background: var(--white);
            padding: 40px;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
            transition: 0.3s;
        }

        .service-card:hover {
            transform: translateY(-10px);
        }

        .service-card i {
            font-size: 3rem;
            color: var(--secondary-color);
            margin-bottom: 20px;
            display: block;
        }

        .service-card h3 {
            margin-bottom: 15px;
        }

        /* الفوتر (Footer) */
        footer {
            background-color: var(--primary-color);
            color: var(--white);
            text-align: center;
            padding: 40px 5%;
            margin-top: 50px;
        }

        /* استجابة الشاشات الصغيرة */
        @media (max-width: 768px) {
            .hero h1 { font-size: 2rem; }
            header { flex-direction: column; gap: 15px; }
            nav a { margin: 0 10px; font-size: 0.9rem; }
        }
    </style>
</head>
<body>

    <header>
        <a href="#" class="logo">ACADEMY-TRAINING</a>
        <nav>
            <a href="#home">الرئيسية</a>
            <a href="#courses">الدورات</a>
            <a href="#about">عن الأكاديمية</a>
            <a href="#contact">اتصل بنا</a>
        </nav>
    </header>

    <section class="hero" id="home">
        <h1>أكاديمية التدريب والتطوير</h1>
        <p>نحن نسعى لتمكين الأفراد والمؤسسات من خلال برامج تدريبية احترافية تتماشى مع معايير الجودة العالمية ورؤية المستقبل.</p>
        <a href="#courses" class="btn">استعرض الدورات المتاحة</a>
    </section>

    <section class="services" id="courses">
        <div class="service-card">
            <h3>تطوير القيادة</h3>
            <p>برامج متخصصة لإعداد القادة وصقل المهارات الإدارية وفق أحدث النظريات العالمية.</p>
        </div>
        <div class="service-card">
            <h3>التدريب التقني</h3>
            <p>دورات في البرمجة، الذكاء الاصطناعي، وتحليل البيانات لمواكبة سوق العمل الرقمي.</p>
        </div>
        <div class="service-card">
            <h3>تطوير الذات</h3>
            <p>مهارات التواصل، إدارة الوقت، والتفكير الإبداعي لتعزيز الكفاءة الشخصية.</p>
        </div>
    </section>

    <footer>
        <p>جميع الحقوق محفوظة &copy; 2026 | أكاديمية التدريب والتطوير</p>
        <p style="font-size: 0.8rem; margin-top: 10px; opacity: 0.7;">تم التطوير لـ TRAINING-ACADEMY</p>
    </footer>

</body>
</html>

