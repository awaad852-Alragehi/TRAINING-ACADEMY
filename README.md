<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>أكاديمية التدريب والتطوير | TRAINING ACADEMY</title>
    
    <!-- مكتبة الأيقونات والخطوط -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com">
    <link href="https://fonts.googleapis.com" rel="stylesheet">
    
    <style>
        :root {
            --primary: #1a2a6c; /* أزرق ملكي غامق */
            --secondary: #b21f1f; /* أحمر داكن جذاب */
            --accent: #fdbb2d; /* ذهبي للأزرار واللوجو */
            --white: #ffffff;
            --bg-light: #f8f9fa;
        }

        * {
            margin: 0; padding: 0; box-sizing: border-box;
            font-family: 'Almarai', sans-serif;
        }

        body { background-color: var(--bg-light); color: #333; }
.video-container {
    position: relative;
    padding-bottom: 56.25%; /* نسبة أبعاد الفيديو 16:9 */
    height: 0;
}
.video-container iframe {
    position: absolute;
    top: 0; left: 0;
    width: 100%; height: 100%;
}

        /* الهيدر واللوجو */
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
            font-size: 1.8rem;
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

        nav a:hover { color: var(--accent); }

        /* القسم الرئيسي */
        .hero {
            background: linear-gradient(135deg, #1a2a6c, #b21f1f, #fdbb2d);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            color: white;
            padding: 120px 5% 80px;
            text-align: center;
        }

        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .hero h1 { font-size: 3.5rem; margin-bottom: 20px; text-shadow: 2px 2px 4px rgba(0,0,0,0.3); }

        /* تحسين البطاقات */
        .services {
           <section class="services" id="courses">
    <!-- دورة PMP المطورة -->
    <div class="service-card">
       .services {
           <section class="services" id="courses">
    <!-- دورة PMP المطورة -->
    <div class="service-card">
        <!-- الفيديو التعريفي -->
        <div class="video-container" style="margin-bottom: 20px; border-radius: 15px; overflow: hidden; background: #000;">
            <!-- استبدل الرابط أدناه برابط فيديو من يوتيوب -->
            <iframe width="100%" height="200" src="https://www.youtube.com" frameborder="0" allowfullscreen></iframe>
        </div>

        <i class="fas fa-project-diagram" style="color: var(--accent);"></i>
        <h3>إدارة المشاريع الاحترافية (PMP)</h3>
        
        <div class="course-details" style="text-align: right; margin: 15px 0;"
        <!-- الفيديو التعريفي -->
        <div class="video-container" style="margin-bottom: 20px; border-radius: 15px; overflow: hidden; background: #000;">
            <!-- استبدل الرابط أدناه برابط فيديو من يوتيوب -->
            <iframe width="100%" height="200" src="https://www.youtube.com" frameborder="0" allowfullscreen></iframe>
        </div>

        <i class="fas fa-project-diagram" style="color: var(--accent);"></i>
        <h3>إدارة المشاريع الاحترافية (PMP)</h3>
        
        <div class="course-details" style="text-align: right; margin: 15px 0;">
            <p style="font-size: 0.9rem; color: #666; margin-bottom: 10px;">
                <i class="fas fa-check-circle" style="color: green;"></i> 35 ساعة تدريبية معتمدة
            </p>
            <p style="font-size: 0.9rem; color: #666; margin-bottom: 10px;">
                <i class="fas fa-check-circle" style="color: green;"></i> محاكاة كاملة للاختبار الدولي
            </p>
            <p style="font-size: 0.9rem; color: #666; margin-bottom: 10px;">
                <i class="fas fa-check-circle" style="color: green;"></i> شرح منهجية Agile و Waterfall
            </p>
        </div>

        <div class="booking-box" style="background: #fdf2e9; padding: 15px; border-radius: 10px; margin-top: 15px;">
            <p style="font-weight: bold; color: var(--primary);">سعر الدورة: 1500 ريال</p>
            <a href="https://wa.me" class="btn-call" style="width: 100%; font-size: 0.9rem; padding: 10px;">احجز مقعدك الآن</a>
        </div>
    </div>

    <!-- كرر نفس التنسيق للدورات الأخرى -->
</section>

        }

        .service-card {
            background: var(--white);
            padding: 40px 30px;
            border-radius: 20px; /* حواف دائرية */
            text-align: center;
            box-shadow: 0 15px 35px rgba(0,0,0,0.1); /* ظل ناعم */
            transition: all 0.4s ease;
            border-bottom: 5px solid var(--accent);
        }

        .service-card:hover {
            transform: translateY(-15px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.2);
        }

        .service-card i {
            font-size: 3rem;
            color: var(--primary);
            margin-bottom: 20px;
        }

        .btn-call {
            background: var(--accent);
            color: var(--primary);
            padding: 15px 35px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 800;
            display: inline-block;
            margin-top: 20px;
            box-shadow: 0 4px 15px rgba(253, 187, 45, 0.4);
        }

        .contact-section {
            background: var(--primary);
            color: white;
            padding: 60px 5%;
            text-align: center;
        }

        footer { background: #111; color: white; padding: 20px; text-align: center; }
    </style>
</head>
<body>

    <header>
        <a href="#" class="logo">
            <i class="fas fa-graduation-cap"></i> <!-- أيقونة اللوجو -->
            أكاديمية المهارات الادارية
            management skills academy
        </a>
        <nav>
            <a href="#home">الرئيسية</a>
            <a href="#courses">الدورات</a>
            <a href="https://wa.me" target="_blank">تواصل معنا</a>
        </nav>
    </header>

    <section class="hero" id="home">
        <h1>مستقبلك يبدأ هنا</h1>
        <p>نقدم لك أفضل الدورات التدريبية المعتمدة عالمياً لعام 2026</p>
        <a href="#courses" class="btn-call">اكتشف الدورات</a>
    </section>

    <section class="services" id="courses">
        <!-- دورة PMP -->
        <div class="service-card">
            <i class="fas fa-project-diagram"></i>
            <h3>إدارة المشاريع (PMP)</h3>
            <p>احصل على الشهادة الأقوى عالمياً في إدارة المشاريع بأسلوب عملي واحترافي.</p>
        </div>

        <!-- دورة تطوير الذات -->
        <div class="service-card">
            <i class="fas fa-users"></i>
            <h3>القيادة الفعالة</h3>
            <p>تطوير مهارات القيادة والتأثير في الآخرين للارتقاء بمسارك المهني.</p>
        </div>

        <!-- دورة التقنية -->
        <div class="service-card">
            <i class="fas fa-laptop-code"></i>
            <h3>التحول الرقمي</h3>
            <p>تعلم مهارات المستقبل وكيفية توظيف الذكاء الاصطناعي في عملك.</p>
        </div>
    </section>

    <section class="contact-section">
        <h2>هل لديك استفسار؟</h2>
        <p style="margin: 15px 0;">نحن متاحون لخدمتك على مدار الساعة</p>
        <p><i class="fab fa-whatsapp"></i> واتساب: 966533936881+</p>
        <p><i class="fas fa-envelope"></i> ايميل: awaad852@gmail.com</p>
    </section>

    <footer>
        <p>جميع الحقوق محفوظة &copy; 2026 | أكاديمية المهارات الادارية</p>
    </footer>

</body>
</html>
