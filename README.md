<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>أكاديمية المهارات الإدارية | 2026</title>
    
    <!-- مكتبة الأيقونات والخطوط -->
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

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Almarai', sans-serif; }
        body { background-color: var(--bg-light); color: #333; line-height: 1.6; }

        header {
            background: var(--primary); padding: 15px 5%;
            display: flex; justify-content: space-between; align-items: center;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1); position: sticky; top: 0; z-index: 1000;
        }

        .logo { color: var(--accent); font-size: 1.4rem; font-weight: 800; text-decoration: none; display: flex; align-items: center; gap: 10px; }
        .logo i { font-size: 1.8rem; color: var(--accent); } /* هذا هو اللوجو */

        nav a { color: var(--white); text-decoration: none; margin-right: 20px; font-weight: 700; }

        .hero {
            background: linear-gradient(135deg, #1a2a6c, #b21f1f, #fdbb2d);
            background-size: 400% 400%; animation: gradientBG 15s ease infinite;
            color: white; padding: 80px 5%; text-align: center;
        }

        @keyframes gradientBG { 0% { background-position: 0% 50%; } 50% { background-position: 100% 50%; } 100% { background-position: 0% 50%; } }

        .about-section { padding: 50px 10%; text-align: center; background: white; border-bottom: 2px solid #eee; }
        .about-section h2 { color: var(--primary); margin-bottom: 15px; }
        .about-section p { font-size: 1.1rem; color: #666; max-width: 900px; margin: 0 auto; }

        .services { display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 30px; padding: 50px 5%; }

        .service-card {
            background: var(--white); border-radius: 20px; overflow: hidden;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1); transition: 0.3s;
            border-bottom: 5px solid var(--accent);
        }
        .service-card:hover { transform: translateY(-10px); }

        /* تنسيق الصور */
        .course-img { width: 100%; height: 220px; object-fit: cover; display: block; }

        .card-content { padding: 25px; text-align: right; }
        .card-content h3 { color: var(--primary); margin-bottom: 12px; font-size: 1.3rem; }
        .card-content .description { font-size: 0.95rem; color: #555; margin-bottom: 15px; }

        .video-container { border-radius: 12px; overflow: hidden; margin: 15px 0; position: relative; padding-bottom: 56.25%; height: 0; background: #000; }
        .video-container iframe { position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0; }

        .price-tag { font-size: 1.5rem; font-weight: 800; color: var(--secondary); margin-bottom: 15px; }
        .btn-booking {
            background: var(--accent); color: var(--primary); padding: 14px; border-radius: 50px;
            text-decoration: none; font-weight: 800; display: block; text-align: center; transition: 0.3s;
        }
        .btn-booking:hover { background: var(--primary); color: white; }

        .contact-section { background: var(--primary); color: white; padding: 50px 5%; text-align: center; }
        footer { background: #111; color: white; padding: 20px; text-align: center; }
    </style>
</head>
<body>

    <header>
        <a href="#" class="logo">
            <i class="fas fa-graduation-cap"></i> <!-- أيقونة اللوجو -->
            <span>أكاديمية المهارات الإدارية</span>
        </a>
        <nav>
            <a href="#about">من نحن</a>
            <a href="#courses">الدورات</a>
        </nav>
    </header>

    <section class="hero">
        <h1>مستقبلك المهني يبدأ من هنا</h1>
        <p>برامج تدريبية احترافية معتمدة لعام 2026</p>
    </section>

    <section class="about-section" id="about">
        <h2>وصف نشاط الأكاديمية</h2>
        <p>نحن منصة تعليمية متخصصة في تطوير المهارات الإدارية والقيادية. نسعى لتمكين الأفراد والمؤسسات من خلال تقديم دورات تدريبية حديثة تواكب رؤية 2030، مع التركيز على الجانب التطبيقي واستخدام الذكاء الاصطناعي في الإدارة الحديثة.</p>
    </section>

    <section class="services" id="courses">
        
        <!-- دورة PMP -->
        <div class="service-card">
            <img src="https://images.unsplash.com" alt="إدارة المشاريع" class="course-img">
            <div class="card-content">
                <h3>إدارة المشاريع الاحترافية (PMP)</h3>
                <p class="description">تأهيل كامل لاجتياز اختبار PMP وفق منهجية 2026، مع التركيز على الإدارة الرشيقة (Agile).</p>
                <div class="video-container">
                    <iframe src="https://www.youtube.com" allow="autoplay; encrypted-media" allowfullscreen></iframe>
                </div>
                <div class="price-tag">400 ريال</div>
                <a href="https://wa.me" class="btn-booking">احجز مقعدك الآن</a>
            </div>
        </div>

        <!-- دورة القيادة -->
        <div class="service-card">
            <img src="https://images.unsplash.com" alt="القيادة" class="course-img">
            <div class="card-content">
                <h3>القيادة الإبداعية والفعالة</h3>
                <p class="description">دورة شاملة في بناء فرق العمل المتميزة وفن التأثير القيادي واتخاذ القرارات الاستراتيجية.</p>
                <div class="price-tag">950 ريال</div>
                <a href="https://wa.me" class="btn-booking">احجز مقعدك الآن</a>
            </div>
        </div>

        <!-- دورة التحول الرقمي -->
        <div class="service-card">
            <img src="https://images.unsplash.com" alt="التحول الرقمي" class="course-img">
            <div class="card-content">
                <h3>التحول الرقمي و AI</h3>
                <p class="description">كيفية توظيف أدوات الذكاء الاصطناعي في العمل الإداري لرفع الإنتاجية وتقليل التكاليف.</p>
                <div class="price-tag">1200 ريال</div>
                <a href="https://wa.me" class="btn-booking">احجز مقعدك الآن</a>
            </div>
        </div>

    </section>

    <section class="contact-section">
        <h2>للتواصل المباشر</h2>
        <p style="margin-bottom: 20px;">نحن هنا للإجابة على جميع استفساراتكم</p>
        <p><i class="fab fa-whatsapp"></i> واتساب: 966533936881+</p>
        <p><i class="fas fa-envelope"></i> ايميل: awaad852@gmail.com</p>
    </section>

    <footer>
        <p>جميع الحقوق محفوظة &copy; 2026 | أكاديمية المهارات الإدارية</p>
    </footer>

</body>
</html>
