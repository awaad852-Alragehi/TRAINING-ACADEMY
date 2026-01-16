<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>أكاديمية المهارات الإدارية | 2026</title>
    
    <!-- روابط مكتبات مشفرة وآمنة لعام 2026 -->
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
        
        nav a { color: var(--white); text-decoration: none; margin-right: 20px; font-weight: 700; }

        .hero {
            background: linear-gradient(135deg, #1a2a6c, #b21f1f, #fdbb2d);
            padding: 80px 5%; text-align: center; color: white;
        }

        .about-section { padding: 50px 10%; text-align: center; background: white; }
        .about-section h2 { color: var(--primary); margin-bottom: 15px; }

        .services { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 25px; padding: 40px 5%; }

        .service-card {
            background: var(--white); border-radius: 15px; overflow: hidden;
            box-shadow: 0 8px 20px rgba(0,0,0,0.1); border-bottom: 5px solid var(--accent);
        }

        /* حاوية الصور مع رابط بديل في حال الفشل */
        .image-box { width: 100%; height: 200px; background: #ddd; overflow: hidden; }
        .image-box img { width: 100%; height: 100%; object-fit: cover; }

        .card-content { padding: 20px; text-align: right; }
        .card-content h3 { color: var(--primary); margin-bottom: 10px; }

        /* حاوية الفيديو - تم تحديثها لتعمل مع سياسات 2026 */
        .video-container {
            position: relative; padding-bottom: 56.25%; height: 0; 
            overflow: hidden; background: #000; border-radius: 10px; margin: 15px 0;
        }
        .video-container iframe {
            position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0;
        }

        .price-tag { font-size: 1.4rem; font-weight: 800; color: var(--secondary); margin: 15px 0; }
        
        .btn-booking {
            background: var(--accent); color: var(--primary); padding: 12px; border-radius: 50px;
            text-decoration: none; font-weight: 800; display: block; text-align: center;
        }

        .contact-section { background: var(--primary); color: white; padding: 50px 5%; text-align: center; }
        footer { background: #111; color: white; padding: 20px; text-align: center; }
    </style>
</head>
<body>

    <header>
        <a href="#" class="logo">
            <i class="fas fa-graduation-cap"></i>
            <span>أكاديمية المهارات الإدارية</span>
        </a>
        <nav><a href="#courses">الدورات</a></nav>
    </header>

    <section class="hero">
        <h1>مستقبلك المهني يبدأ معنا</h1>
        <p>نقدم برامج تدريبية احترافية تواكب رؤية 2030</p>
    </section>

    <section class="about-section">
        <h2>من نحن</h2>
        <p>أكاديمية متخصصة في تأهيل القادة والمدراء بأحدث المنهجيات العالمية والذكاء الاصطناعي.</p>
    </section>

    <section class="services" id="courses">
        
        <!-- دورة PMP -->
        <div class="service-card">
            <div class="image-box">
                <img src="https://images.unsplash.com" alt="PMP Course">
            </div>
            <div class="card-content">
                <h3>إدارة المشاريع (PMP)</h3>
                <p>وصف: دورة مكثفة لاجتياز اختبار PMP العالمي.</p>
                <div class="video-container">
                    <!-- رابط التضمين الآمن -->
                    <iframe src="https://www.youtube-nocookie.com" allowfullscreen></iframe>
                </div>
                <div class="price-tag">400 ريال</div>
                <a href="https://wa.me" class="btn-booking">حجز مقعد</a>
            </div>
        </div>

        <!-- دورة القيادة -->
        <div class="service-card">
            <div class="image-box">
                <img src="https://images.unsplash.com" alt="Leadership">
            </div>
            <div class="card-content">
                <h3>القيادة الإبداعية</h3>
                <p>وصف: مهارات القيادة الحديثة وبناء فرق العمل.</p>
                <div class="price-tag">950 ريال</div>
                <a href="https://wa.me" class="btn-booking">حجز مقعد</a>
            </div>
        </div>

    </section>

    <section class="contact-section">
        <h2>تواصل معنا</h2>
        <p>واتساب: 966533936881+</p>
        <p>ايميل: awaad852@gmail.com</p>
    </section>

    <footer>
        <p>جميع الحقوق محفوظة &copy; 2026</p>
    </footer>

</body>
</html>
