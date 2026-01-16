<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>أكاديمية المهارات الإدارية | 2026</title>
    
    <!-- تحديث مكتبة الأيقونات والخطوط لعام 2026 -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com">
    <link href="https://fonts.googleapis.com" rel="stylesheet">
    
    <style>
        :root {
            --primary: #1a2a6c;
            --secondary: #b21f1f;
            --accent: #fdbb2d;
            --white: #ffffff;
            --bg-light: #f8f9fa;
        }

        * {
            margin: 0; padding: 0; box-sizing: border-box;
            font-family: 'Almarai', sans-serif;
        }

        body { background-color: var(--bg-light); color: #333; line-height: 1.6; }

        header {
            background: var(--primary);
            padding: 15px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
            position: sticky; top: 0; z-index: 1000;
        }

        .logo {
            color: var(--accent);
            font-size: 1.2rem;
            font-weight: 800;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        nav a {
            color: var(--white);
            text-decoration: none;
            margin-right: 20px;
            font-weight: 700;
            transition: 0.3s;
        }

        .hero {
            background: linear-gradient(135deg, #1a2a6c, #b21f1f, #fdbb2d);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            color: white;
            padding: 100px 5%;
            text-align: center;
        }

        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .services {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            padding: 50px 5%;
        }

        .service-card {
            background: var(--white);
            padding: 25px;
            border-radius: 20px;
            text-align: center;
            box-shadow: 0 10px 25px rgba(0,0,0,0.05);
            border-bottom: 5px solid var(--accent);
            transition: transform 0.3s ease;
        }

        .service-card:hover { transform: translateY(-10px); }

        .video-container {
            border-radius: 15px;
            overflow: hidden;
            margin-bottom: 20px;
            background: #000;
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .video-container iframe {
            position: absolute;
            top: 0; left: 0;
            width: 100%; height: 100%;
        }

        .course-features {
            text-align: right;
            margin: 20px 0;
            list-style: none;
        }

        .course-features li { margin-bottom: 10px; font-size: 0.95rem; display: flex; align-items: center; }
        .course-features li i { color: #27ae60; margin-left: 10px; }

        .price-tag {
            font-size: 1.6rem;
            font-weight: 800;
            color: var(--secondary);
            margin-bottom: 20px;
        }

        .btn-booking {
            background: var(--accent);
            color: var(--primary);
            padding: 14px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 800;
            display: block;
            transition: 0.3s;
        }

        .btn-booking:hover { background: var(--primary); color: white; }

        .contact-section {
            background: #f1f1f1;
            padding: 60px 5%;
            text-align: center;
        }

        .contact-card {
            background: var(--primary);
            color: white;
            padding: 30px;
            border-radius: 20px;
            max-width: 600px;
            margin: 0 auto;
        }

        footer { background: #111; color: white; padding: 25px; text-align: center; font-size: 0.9rem; }
    </style>
</head>
<body>

    <header>
        <a href="#" class="logo">
            <i class="fas fa-graduation-cap"></i>
            أكاديمية المهارات الإدارية
        </a>
        <nav>
            <a href="#courses">الدورات</a>
            <a href="https://wa.me" target="_blank">تواصل معنا</a>
        </nav>
    </header>

    <section class="hero" id="home">
        <h1>مستقبلك المهني يبدأ هنا</h1>
        <p>نقدم لك أقوى البرامج التدريبية المعتمدة لعام 2026</p>
    </section>

    <section class="services" id="courses">
        
        <!-- دورة PMP -->
        <div class="service-card">
            <div class="video-container">
               <!-- استبدل ID الفيديو هنا بفيديو اليوتيوب الخاص بك -->
               <iframe src="https://www.youtube.com" frameborder="0" allowfullscreen></iframe>
            </div>
            <i class="fas fa-project-diagram" style="font-size: 2.5rem; color: var(--primary);"></i>
            <h3>إدارة المشاريع الاحترافية (PMP)</h3>
            <ul class="course-features">
                <li><i class="fas fa-check-circle"></i> شرح شامل لمنهجية الإصدار السابع</li>
                <li><i class="fas fa-check-circle"></i> الحصول على 35 ساعة معتمدة</li>
                <li><i class="fas fa-check-circle"></i> بنك أسئلة لمحاكاة اختبارات 2026</li>
            </ul>
            <div class="price-tag">400 ريال</div>
            <a href="https://wa.me?text=أرغب%20في%20التسجيل%20بدورة%20PMP" class="btn-booking">حجز مقعد الآن</a>
        </div>

        <!-- دورة القيادة -->
        <div class="service-card">
            <div class="video-container">
                <iframe src="https://www.youtube.com" frameborder="0" allowfullscreen></iframe>
            </div>
            <i class="fas fa-users-gear" style="font-size: 2.5rem; color: var(--primary);"></i>
            <h3>القيادة الإبداعية والفعالة</h3>
            <ul class="course-features">
                <li><i class="fas fa-check-circle"></i> تطوير مهارات التفكير القيادي</li>
                <li><i class="fas fa-check-circle"></i> إدارة فرق العمل الهجينة</li>
                <li><i class="fas fa-check-circle"></i> شهادة إتمام دورة معتمدة</li>
            </ul>
            <div class="price-tag">950 ريال</div>
            <a href="https://wa.me?text=أرغب%20في%20التسجيل%20بدورة%20القيادة" class="btn-booking">حجز مقعد الآن</a>
        </div>

        <!-- دورة التحول الرقمي -->
        <div class="service-card">
            <div class="video-container">
                <iframe src="https://www.youtube.com" frameborder="0" allowfullscreen></iframe>
            </div>
            <i class="fas fa-microchip" style="font-size: 2.5rem; color: var(--primary);"></i>
            <h3>التحول الرقمي و AI 2026</h3>
            <ul class="course-features">
                <li><i class="fas fa-check-circle"></i> أدوات الذكاء الاصطناعي التوليدي</li>
                <li><i class="fas fa-check-circle"></i> أتمتة العمليات (RPA) للمدراء</li>
                <li><i class="fas fa-check-circle"></i> استراتيجيات رؤية 2030 الرقمية</li>
            </ul>
            <div class="price-tag">1200 ريال</div>
            <a href="https://wa.me?text=أرغب%20في%20التسجيل%20بدورة%20التحول%20الرقمي" class="btn-booking">حجز مقعد الآن</a>
        </div>

    </section>

    <section class="contact-section">
        <div class="contact-card">
            <h2>تواصل معنا مباشرة</h2>
            <div style="margin-top: 20px;">
                <p><i class="fab fa-whatsapp"></i> واتساب: 966533936881+</p>
                <p><i class="fas fa-envelope"></i> ايميل: awaad852@gmail.com</p>
            </div>
        </div>
    </section>

    <footer>
        <p>جميع الحقوق محفوظة &copy; 2026 | أكاديمية المهارات الإدارية</p>
    </footer>

</body>
</html>
