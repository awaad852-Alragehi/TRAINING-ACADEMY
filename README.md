<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>أكاديمية المهارات الإدارية | 2026</title>
    
    <!-- مكتبات الأيقونات والخطوط -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com">
    <link href="https://fonts.googleapis.com" rel="stylesheet">
    
    <style>
        :root {
            --primary: #1a2a6c;
            --secondary: #b21f1f;
            --accent: #fdbb2d;
            --white: #ffffff;
            --bg-light: #f4f7f6;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Almarai', sans-serif; background: var(--bg-light); color: #333; line-height: 1.8; }

        /* الهيدر واللوجو */
        header {
            background: var(--primary); padding: 20px 5%;
            display: flex; justify-content: space-between; align-items: center;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3); position: sticky; top: 0; z-index: 1000;
        }
        .logo-container { display: flex; align-items: center; gap: 15px; color: var(--accent); text-decoration: none; }
        .logo-text h1 { font-size: 1.2rem; color: var(--white); }

        /* قسم البطولة */
        .hero {
            background: linear-gradient(rgba(26, 42, 108, 0.8), rgba(26, 42, 108, 0.8)), 
                        url('https://images.pexels.com');
            background-size: cover; background-position: center;
            color: white; padding: 100px 5%; text-align: center;
        }

        /* وصف الأكاديمية - لغتين */
        .about-section { padding: 60px 5%; background: white; }
        .dual-lang-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 40px; margin-top: 30px; }
        .lang-box { padding: 20px; border-radius: 10px; background: #f9f9f9; border-right: 5px solid var(--accent); }
        .lang-en { direction: ltr; text-align: left; border-right: none; border-left: 5px solid var(--primary); font-family: 'Poppins', sans-serif; }

        /* شبكة الدورات */
        .services { display: grid; grid-template-columns: repeat(auto-fit, minmax(350px, 1fr)); gap: 30px; padding: 50px 5%; }
        .course-card { background: white; border-radius: 20px; overflow: hidden; box-shadow: 0 10px 30px rgba(0,0,0,0.1); transition: 0.3s; }
        .course-card:hover { transform: translateY(-10px); }

        /* إصلاح الصور */
        .img-container { width: 100%; height: 230px; background: #eee; }
        .img-container img { width: 100%; height: 100%; object-fit: cover; }

        /* إصلاح الفيديو */
        .video-container { position: relative; padding-bottom: 56.25%; height: 0; background: #000; }
        .video-container iframe { position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0; }

        .card-body { padding: 25px; text-align: right; }
        .price { font-size: 1.5rem; color: var(--secondary); font-weight: 800; margin: 15px 0; }

        .btn-booking {
            background: #25d366; color: white; padding: 15px; border-radius: 50px;
            text-decoration: none; display: block; text-align: center; font-weight: 800;
        }

        .footer { background: var(--primary); color: white; padding: 50px 5%; text-align: center; }
        
        @media (max-width: 768px) { .dual-lang-grid { grid-template-columns: 1fr; } }
    </style>
</head>
<body>

    <header>
        <a href="#" class="logo-container">
            <i class="fas fa-graduation-cap fa-2x"></i>
            <div class="logo-text"><h1>أكاديمية المهارات الإدارية</h1></div>
        </a>
    </header>

    <section class="hero">
        <h1>Management Skills Academy 2026</h1>
        <p>نصنع القادة.. ونبني المستقبل</p>
    </section>

    <!-- وصف الأكاديمية بالتفصيل -->
    <section class="about-section">
        <h2 style="text-align: center; color: var(--primary);">عن الأكاديمية | About Us</h2>
        <div class="dual-lang-grid">
            <div class="lang-box">
                <h3>رؤيتنا الإستراتيجية</h3>
                <p>أكاديمية المهارات الإدارية هي منصة تدريبية عالمية تهدف إلى تمكين المهنيين والمدراء في الشرق الأوسط. نحن نقدم برامج تدريبية متقدمة في إدارة المشاريع، القيادة، والتحول الرقمي. نعتمد في عام 2026 على دمج تقنيات الذكاء الاصطناعي مع أحدث نظريات الإدارة لتزويد المتدربين بمهارات عملية تتماشى مع رؤية المملكة 2030 وتحديات السوق العالمي.</p>
            </div>
            <div class="lang-box lang-en">
                <h3>Our Strategic Vision</h3>
                <p>Management Skills Academy is a global training platform dedicated to empowering professionals in the Middle East. We provide advanced programs in project management, leadership, and digital transformation. In 2026, we integrate AI technologies with the latest management theories to provide trainees with practical skills aligned with Vision 2030 and global market challenges.</p>
            </div>
        </div>
    </section>

    <section class="services">
        
        <!-- دورة PMP -->
        <div class="course-card">
            <div class="video-container">
                <!-- استخدام رابط nocookie لضمان الظهور -->
                <iframe src="https://www.youtube-nocookie.com" allowfullscreen></iframe>
            </div>
            <div class="card-body">
                <h3>إدارة المشاريع الاحترافية (PMP)</h3>
                <p>الدورة الأشهر عالمياً لاحتراف إدارة المشاريع وفق الإصدار السابع من PMI. (Project Management Professional - 7th Edition).</p>
                <div class="price">400 ريال</div>
                <a href="https://wa.me" class="btn-booking">سجل الآن | Register Now</a>
            </div>
        </div>

        <!-- دورة القيادة -->
        <div class="course-card">
            <div class="img-container">
                <img src="https://images.pexels.com" alt="Leadership">
            </div>
            <div class="card-body">
                <h3>القيادة الإبداعية والفعالة</h3>
                <p>بناء الشخصية القيادية وفن إدارة فرق العمل المتميزة. (Creative and Effective Leadership Skills).</p>
                <div class="price">950 ريال</div>
                <a href="https://wa.me" class="btn-booking">سجل الآن | Register Now</a>
            </div>
        </div>

        <!-- دورة التحول الرقمي -->
        <div class="course-card">
            <div class="img-container">
                <img src="https://images.pexels.com" alt="Digital">
            </div>
            <div class="card-body">
                <h3>التحول الرقمي و AI</h3>
                <p>استراتيجيات دمج الذكاء الاصطناعي في الإدارة الحديثة 2026. (Digital Transformation & AI for Managers).</p>
                <div class="price">1200 ريال</div>
                <a href="https://wa.me" class="btn-booking">سجل الآن | Register Now</a>
            </div>
        </div>

    </section>

    <footer class="footer">
        <h2>تواصل معنا | Contact</h2>
        <p>WhatsApp: +966533936881</p>
        <p>Email: awaad852@gmail.com</p>
        <p style="margin-top: 20px; font-size: 0.8rem;">© 2026 Management Skills Academy</p>
    </footer>

</body>
</html>
