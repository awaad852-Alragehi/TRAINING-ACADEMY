<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>أكاديمية المهارات الادارية Management Skills Academy | تدريب عن بعد</title>
    
    <!-- خط الكوفي العربي -->
    <link href="https://fonts.googleapis.com/css2?family=Almarai:wght@300;400;700;800&display=swap" rel="stylesheet">
    <!-- أيقونات Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        :root {
            --primary: #1e3a8a;
            --primary-light: #3b82f6;
            --secondary: #dc2626;
            --accent: #f59e0b;
            --gold: #fbbf24;
            --white: #ffffff;
            --bg-light: #f8fafc;
            --text-dark: #1f2937;
            --success: #10b981;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; scroll-behavior: smooth; }
        
        body { 
            font-family: 'Almarai', sans-serif; 
            background: var(--bg-light); 
            color: var(--text-dark); 
            line-height: 1.8;
            overflow-x: hidden;
        }

        /* ===== HEADER ===== */
        header {
            background: linear-gradient(135deg, var(--primary) 0%, #0f172a 100%);
            padding: 15px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 4px 20px rgba(30, 58, 138, 0.3);
            position: sticky;
            top: 0;
            z-index: 1000;
            backdrop-filter: blur(10px);
        }

        .logo-container { 
            display: flex; 
            align-items: center; 
            gap: 15px; 
            color: var(--gold);
            text-decoration: none;
            transition: transform 0.3s;
        }
        .logo-container:hover { transform: scale(1.02); }
        
        .logo-icon {
            width: 50px;
            height: 50px;
            background: linear-gradient(135deg, var(--accent), var(--gold));
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            color: var(--primary);
            box-shadow: 0 4px 15px rgba(245, 158, 11, 0.4);
        }

        .logo-text h1 { 
            font-size: 1.3rem; 
            color: var(--white);
            font-weight: 800;
            letter-spacing: -0.5px;
        }
        .logo-text span {
            font-size: 0.75rem;
            color: var(--gold);
            font-weight: 400;
        }

        nav { display: flex; gap: 30px; }
        nav a {
            color: var(--white);
            text-decoration: none;
            font-weight: 600;
            font-size: 0.95rem;
            position: relative;
            padding: 5px 0;
            transition: color 0.3s;
        }
        nav a::after {
            content: '';
            position: absolute;
            bottom: 0;
            right: 0;
            width: 0;
            height: 2px;
            background: var(--accent);
            transition: width 0.3s;
        }
        nav a:hover { color: var(--accent); }
        nav a:hover::after { width: 100%; }

        .mobile-menu { display: none; font-size: 1.5rem; color: var(--white); cursor: pointer; }

        /* ===== HERO SECTION ===== */
        .hero {
            background: linear-gradient(135deg, rgba(30, 58, 138, 0.95) 0%, rgba(15, 23, 42, 0.95) 100%), 
                        url('https://images.unsplash.com/photo-1524178232363-1fb2b075b655?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            color: white;
            padding: 120px 5%;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(245, 158, 11, 0.1) 0%, transparent 70%);
            animation: pulse 15s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); opacity: 0.5; }
            50% { transform: scale(1.1); opacity: 0.8; }
        }

        .hero-content { position: relative; z-index: 1; max-width: 800px; margin: 0 auto; }
        
        .badge {
            display: inline-block;
            background: rgba(245, 158, 11, 0.2);
            border: 1px solid var(--accent);
            color: var(--gold);
            padding: 8px 20px;
            border-radius: 50px;
            font-size: 0.85rem;
            font-weight: 700;
            margin-bottom: 25px;
            backdrop-filter: blur(10px);
        }

        .hero h2 {
            font-size: 3rem;
            font-weight: 800;
            margin-bottom: 20px;
            line-height: 1.3;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }
        .hero h2 span { color: var(--accent); }

        .hero p {
            font-size: 1.25rem;
            margin-bottom: 35px;
            opacity: 0.95;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .hero-buttons {
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            padding: 15px 35px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 700;
            font-size: 1rem;
            transition: all 0.3s;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            border: none;
            cursor: pointer;
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--accent), var(--gold));
            color: var(--primary);
            box-shadow: 0 10px 30px rgba(245, 158, 11, 0.3);
        }
        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 40px rgba(245, 158, 11, 0.4);
        }

        .btn-secondary {
            background: transparent;
            color: var(--white);
            border: 2px solid rgba(255,255,255,0.3);
            backdrop-filter: blur(10px);
        }
        .btn-secondary:hover {
            background: rgba(255,255,255,0.1);
            border-color: var(--white);
        }

        /* ===== STATS SECTION ===== */
        .stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            padding: 60px 5%;
            background: var(--white);
            margin-top: -40px;
            position: relative;
            z-index: 10;
            max-width: 1000px;
            margin-left: auto;
            margin-right: auto;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.1);
        }

        .stat-item {
            text-align: center;
            padding: 20px;
        }
        .stat-number {
            font-size: 2.5rem;
            font-weight: 800;
            color: var(--primary);
            display: block;
        }
        .stat-label {
            color: #666;
            font-size: 0.9rem;
            margin-top: 5px;
        }

        /* ===== COURSES SECTION ===== */
        .section {
            padding: 80px 5%;
            max-width: 1400px;
            margin: 0 auto;
        }

        .section-header {
            text-align: center;
            margin-bottom: 60px;
        }
        .section-header h2 {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 15px;
            position: relative;
            display: inline-block;
        }
        .section-header h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 60px;
            height: 4px;
            background: var(--accent);
            border-radius: 2px;
        }
        .section-header p {
            color: #666;
            font-size: 1.1rem;
            max-width: 600px;
            margin: 20px auto 0;
        }

        .courses-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 35px;
        }

        .course-card {
            background: white;
            border-radius: 24px;
            overflow: hidden;
            box-shadow: 0 10px 40px rgba(0,0,0,0.08);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            border: 1px solid rgba(0,0,0,0.05);
            position: relative;
        }

        .course-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 30px 60px rgba(30, 58, 138, 0.15);
        }

        .course-badge {
            position: absolute;
            top: 20px;
            left: 20px;
            background: var(--secondary);
            color: white;
            padding: 6px 15px;
            border-radius: 20px;
            font-size: 0.75rem;
            font-weight: 700;
            z-index: 10;
            box-shadow: 0 4px 15px rgba(220, 38, 38, 0.3);
        }

        .img-container {
            width: 100%;
            height: 220px;
            background: linear-gradient(135deg, var(--primary), var(--primary-light));
            overflow: hidden;
            position: relative;
        }

        .img-container img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.6s, opacity 0.3s;
            opacity: 0.9;
        }

        .course-card:hover .img-container img {
            transform: scale(1.15);
            opacity: 1;
        }

        .card-body {
            padding: 30px;
            text-align: right;
        }

        .course-meta {
            display: flex;
            gap: 15px;
            margin-bottom: 15px;
            font-size: 0.8rem;
            color: #666;
        }
        .course-meta span {
            display: flex;
            align-items: center;
            gap: 5px;
        }

        .card-body h3 {
            color: var(--primary);
            font-size: 1.4rem;
            margin-bottom: 12px;
            font-weight: 700;
            line-height: 1.4;
        }

        .description-box {
            font-size: 0.95rem;
            color: #555;
            margin-bottom: 20px;
            line-height: 1.8;
        }

        .features-list {
            list-style: none;
            margin: 20px 0;
            padding: 0;
        }
        .features-list li {
            padding: 8px 0;
            font-size: 0.9rem;
            color: #444;
            display: flex;
            align-items: center;
            gap: 10px;
            border-bottom: 1px dashed #eee;
        }
        .features-list li:last-child { border-bottom: none; }
        .features-list i {
            color: var(--success);
            font-size: 0.9rem;
        }

        .price-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin: 25px 0;
            padding-top: 20px;
            border-top: 2px solid #f0f0f0;
        }

        .price {
            font-size: 1.9rem;
            color: var(--secondary);
            font-weight: 800;
        }
        .price span {
            font-size: 0.9rem;
            color: #999;
            font-weight: 400;
            text-decoration: line-through;
            margin-right: 8px;
        }

        .seats-left {
            font-size: 0.8rem;
            color: var(--secondary);
            font-weight: 600;
            background: rgba(220, 38, 38, 0.1);
            padding: 5px 12px;
            border-radius: 20px;
        }

        .btn-booking {
            background: linear-gradient(135deg, #25d366, #128c7e);
            color: white;
            padding: 16px;
            border-radius: 12px;
            text-decoration: none;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            font-weight: 700;
            font-size: 1rem;
            transition: all 0.3s;
            box-shadow: 0 5px 20px rgba(37, 211, 102, 0.3);
            border: none;
            cursor: pointer;
            width: 100%;
        }

        .btn-booking:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 30px rgba(37, 211, 102, 0.4);
        }

        /* ===== ABOUT TRAINER ===== */
        .about-section {
            background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
            padding: 80px 5%;
        }

        .trainer-container {
            max-width: 1000px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 300px 1fr;
            gap: 50px;
            align-items: center;
            background: white;
            padding: 50px;
            border-radius: 30px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.08);
        }

        .trainer-image {
            position: relative;
        }
        .trainer-image img {
            width: 100%;
            height: 300px;
            object-fit: cover;
            border-radius: 20px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }
        .experience-badge {
            position: absolute;
            bottom: -20px;
            right: -20px;
            background: var(--accent);
            color: var(--primary);
            width: 100px;
            height: 100px;
            border-radius: 50%;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            font-weight: 800;
            box-shadow: 0 10px 30px rgba(245, 158, 11, 0.4);
            border: 4px solid white;
        }
        .experience-badge span:first-child { font-size: 1.8rem; }
        .experience-badge span:last-child { font-size: 0.7rem; }

        .trainer-info h3 {
            font-size: 2rem;
            color: var(--primary);
            margin-bottom: 10px;
        }
        .trainer-info .title {
            color: var(--accent);
            font-weight: 700;
            font-size: 1.1rem;
            margin-bottom: 20px;
        }
        .trainer-info p {
            color: #555;
            line-height: 2;
            margin-bottom: 20px;
        }

        .credentials {
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
            margin-top: 25px;
        }
        .credential-item {
            display: flex;
            align-items: center;
            gap: 10px;
            background: var(--bg-light);
            padding: 12px 20px;
            border-radius: 10px;
            font-size: 0.9rem;
        }
        .credential-item i { color: var(--primary); }

        /* ===== CONTACT SECTION ===== */
        .contact-section {
            background: var(--primary);
            color: white;
            padding: 80px 5%;
            text-align: center;
        }

        .contact-content {
            max-width: 700px;
            margin: 0 auto;
        }

        .contact-section h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }
        .contact-section p {
            font-size: 1.2rem;
            opacity: 0.9;
            margin-bottom: 40px;
        }

        .whatsapp-btn {
            display: inline-flex;
            align-items: center;
            gap: 15px;
            background: #25d366;
            color: white;
            padding: 20px 50px;
            border-radius: 50px;
            text-decoration: none;
            font-size: 1.3rem;
            font-weight: 700;
            transition: all 0.3s;
            box-shadow: 0 15px 40px rgba(37, 211, 102, 0.4);
        }
        .whatsapp-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 20px 50px rgba(37, 211, 102, 0.5);
        }
        .whatsapp-btn i { font-size: 1.5rem; }

        .contact-methods {
            display: flex;
            justify-content: center;
            gap: 40px;
            margin-top: 50px;
            flex-wrap: wrap;
        }
        .contact-method {
            display: flex;
            align-items: center;
            gap: 10px;
            opacity: 0.8;
        }

        /* ===== FOOTER ===== */
        footer {
            background: #0f172a;
            color: rgba(255,255,255,0.7);
            padding: 40px 5%;
            text-align: center;
            font-size: 0.9rem;
        }
        footer a {
            color: var(--accent);
            text-decoration: none;
        }

        /* ===== ANIMATIONS ===== */
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.8s ease-out;
        }
        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* ===== RESPONSIVE ===== */
        @media (max-width: 768px) {
            nav { display: none; }
            .mobile-menu { display: block; }
            
            .hero h2 { font-size: 2rem; }
            .hero p { font-size: 1rem; }
            
            .courses-grid { grid-template-columns: 1fr; }
            
            .trainer-container {
                grid-template-columns: 1fr;
                text-align: center;
                padding: 30px;
            }
            .experience-badge {
                right: 50%;
                transform: translateX(50%);
            }
            
            .stats { margin-top: -20px; padding: 40px 20px; }
        }
    </style>
</head>
<body>

    <!-- HEADER -->
    <header>
        <a href="#" class="logo-container">
            <div class="logo-icon">
                <i class="fas fa-graduation-cap"></i>
            </div>
            <div class="logo-text">
    أكاديمية ألمهارات الإدارية Management Skills Academy</h1>
                <span>تدريب عن بعد - من اليمن إلى العالم</span>
            </div>
        </a>
        
        <nav>
            <a href="#courses">الدورات</a>
            <a href="#about">عن المدرب</a>
            <a href="#contact">تواصل معنا</a>
        </nav>
        
        <div class="mobile-menu">
            <i class="fas fa-bars"></i>
        </div>
    </header>

    <!-- HERO -->
    <section class="hero">
        <div class="hero-content">
            <div class="badge">🚀 انطلاقة جديدة 2026</div>
            <h2>طوّر مهاراتك الإدارية <span>من أي مكان</span></h2>
            <p>دورات احترافية في الإدارة والقيادة والإنتاجية، مباشرة عبر الزوم مع مدرب خبير، شهادات معتمدة، وأسعار تناسب الجميع</p>
            
            <div class="hero-buttons">
                <a href="#courses" class="btn btn-primary">
                    <i class="fas fa-rocket"></i>
                    اكتشف الدورات
                </a>
                <a href="https://wa.me/966534379054" class="btn btn-secondary" target="_blank">
                    <i class="fab fa-whatsapp"></i>
                    استشارة مجانية
                </a>
            </div>
        </div>
    </section>

    <!-- STATS -->
    <div class="stats fade-in">
        <div class="stat-item">
            <span class="stat-number">+500</span>
            <div class="stat-label">متدرب في اليمن والسعودية</div>
        </div>
        <div class="stat-item">
            <span class="stat-number">98%</span>
            <div class="stat-label">نسبة الرضا</div>
        </div>
        <div class="stat-item">
            <span class="stat-number">15+</span>
            <div class="stat-label">دورة متخصصة</div>
        </div>
        <div class="stat-item">
            <span class="stat-number">24/7</span>
            <div class="stat-label">دعم مستمر</div>
        </div>
    </div>

    <!-- COURSES -->
    <section id="courses" class="section">
        <div class="section-header fade-in">
            <h2>الدورات المتاحة</h2>
            <p>اختر من برامجنا التدريبية المصممة خصيصاً لتطوير كفاءاتك في بيئة العمل الحديثة</p>
        </div>

        <div class="courses-grid">
            <!-- Course 1 -->
            <div class="course-card fade-in">
                <div class="course-badge">الأكثر طلباً</div>
                <div class="img-container">
                    <img src="https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="إدارة الوقت">
                </div>
                <div class="card-body">
                    <div class="course-meta">
                        <span><i class="fas fa-clock"></i> 8 ساعات</span>
                        <span><i class="fas fa-video"></i> 4 جلسات</span>
                        <span><i class="fas fa-users"></i> أونلاين</span>
                    </div>
                    <h3>ماستر إدارة الوقت والإنتاجية</h3>
                    <div class="description-box">
                        تعلم أدوات عملية لتنظيم وقتك، إدارة الأولويات، التخلص من المماطلة، وزيادة إنتاجيتك 3 أضعاف
                    </div>
                    <ul class="features-list">
                        <li><i class="fas fa-check-circle"></i> نموذج Eisenhower للأولويات</li>
                        <li><i class="fas fa-check-circle"></i> تقنيات Pomodoro والتعليق العميق</li>
                        <li><i class="fas fa-check-circle"></i> أدوات رقمية مجانية</li>
                        <li><i class="fas fa-check-circle"></i> خطة تطبيق شخصية</li>
                    </ul>
                    <div class="price-row">
                        <div class="price">
                            <span>75$</span>
                            49$
                        </div>
                        <div class="seats-left">
                            <i class="fas fa-fire"></i> بقي 3 مقاعد
                        </div>
                    </div>
                    <a href="https://wa.me/966534379054?text=أرغب في التسجيل في دورة إدارة الوقت" class="btn-booking" target="_blank">
                        <i class="fab fa-whatsapp"></i>
                        سجل الآن عبر الواتساب
                    </a>
                </div>
            </div>

            <!-- Course 2 -->
            <div class="course-card fade-in">
                <div class="img-container">
                    <img src="https://images.unsplash.com/photo-1519389950473-47ba0277781c?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="القيادة الإشرافية">
                </div>
                <div class="card-body">
                    <div class="course-meta">
                        <span><i class="fas fa-clock"></i> 12 ساعة</span>
                        <span><i class="fas fa-video"></i> 6 جلسات</span>
                        <span><i class="fas fa-certificate"></i> شهادة</span>
                    </div>
                    <h3>القيادة الإشرافية الفعّالة</h3>
                    <div class="description-box">
                        للمديرين الجدد والمشرفين: تعلم كيف تدير فريقك، تحفز موظفيك، تحل النزاعات، وتبني ثقافة إيجابية
                    </div>
                    <ul class="features-list">
                        <li><i class="fas fa-check-circle"></i> أنماط القيادة Situational</li>
                        <li><i class="fas fa-check-circle"></i> إدارة الأداء والتوجيه</li>
                        <li><i class="fas fa-check-circle"></i> التواصل الفعال مع الفريق</li>
                        <li><i class="fas fa-check-circle"></i> دراسات حالة واقعية</li>
                    </ul>
                    <div class="price-row">
                        <div class="price">
                            <span>99$</span>
                            69$
                        </div>
                        <div class="seats-left" style="background: rgba(16, 185, 129, 0.1); color: var(--success);">
                            <i class="fas fa-door-open"></i> مقاعد متاحة
                        </div>
                    </div>
                    <a href="https://wa.me/966XXXXXXXXX?text=أرغب في التسجيل في دورة القيادة الإشرافية" class="btn-booking" target="_blank">
                        <i class="fab fa-whatsapp"></i>
                        سجل الآن عبر الواتساب
                    </a>
                </div>
            </div>

            <!-- Course 3 -->
            <div class="course-card fade-in">
                <div class="course-badge" style="background: var(--primary);">جديد</div>
                <div class="img-container">
                    <img src="https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="إدارة المشاريع">
                </div>
                <div class="card-body">
                    <div class="course-meta">
                        <span><i class="fas fa-clock"></i> 16 ساعة</span>
                        <span><i class="fas fa-video"></i> 8 جلسات</span>
                        <span><i class="fas fa-tasks"></i> مشروع عملي</span>
                    </div>
                    <h3>إدارة المشاريع الاحترافية (PMP تمهيدي)</h3>
                    <div class="description-box">
                        مقدمة شاملة في إدارة المشاريع: التخطيط، الجدولة، إدارة المخاطر، والتسليم الناجح مع معايير PMI
                    </div>
                    <ul class="features-list">
                        <li><i class="fas fa-check-circle"></i> منهجية Agile وWaterfall</li>
                        <li><i class="fas fa-check-circle"></i> أدوات MS Project وTrello</li>
                        <li><i class="fas fa-check-circle"></i> إدارة المخاطر والجودة</li>
                        <li><i class="fas fa-check-circle"></i> محاكاة مشروع حقيقي</li>
                    </ul>
                    <div class="price-row">
                        <div class="price">
                            <span>120$</span>
                            89$
                        </div>
                        <div class="seats-left">
                            <i class="fas fa-clock"></i> تبدأ الأحد القادم
                        </div>
                    </div>
                    <a href="https://wa.me/966534379054?text=أرغب في التسجيل في دورة إدارة المشاريع" class="btn-booking" target="_blank">
                        <i class="fab fa-whatsapp"></i>
                        سجل الآن عبر الواتساب
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- ABOUT TRAINER -->
    <section id="about" class="about-section">
        <div class="section-header fade-in" style="margin-bottom: 40px;">
            <h2>عن المدرب</h2>
        </div>
        
        <div class="trainer-container fade-in">
            <div class="trainer-image">
                <img src="https://images.unsplash.com/photo-1560250097-0b93528c311a?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="المدرب">
                <div class="experience-badge">
                    <span>+8</span>
                    <span>سنوات خبرة</span>
                </div>
            </div>
            
            <div class="trainer-info">
                <h3>[اسمك الكامل]</h3>
                <div class="title">خبير في التطوير الإداري والتدريب المؤسسي</div>
                <p>
                    مدرب معتمد بخبرة 8+ سنوات في مجال التدريب الإداري والتطوير المؤسسي. وساعدت أكثر من 500 متدرب في تطوير مهاراتهم الإدارية والقيادية.
                </p>
                <p>
                    أؤمن بالتدريب العملي القائم على النتائج، حيث أجمع بين النظريات الإدارية الحديثة والتطبيق العملي في البيئة العربية.
                </p>
                
                <div class="credentials">
                    <div class="credential-item">
                        <i class="fas fa-certificate"></i>
                        <span>شهادة PMP</span>
                    </div>
                    <div class="credential-item">
                        <i class="fas fa-award"></i>
                        <span>معتمد من CMI</span>
                    </div>
                    <div class="credential-item">
                        <i class="fas fa-briefcase"></i>
                        <span>50+ شركة</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="contact-section">
        <div class="contact-content fade-in">
            <h2>ابدأ رحلة تطويرك الآن</h2>
            <p>لديك استفسار؟ أو ترغب في تسجيل مجموعة من موظفيك؟ تواصل معي مباشرة</p>
            
            <a href="https://wa.me/966XXXXXXXXX" class="whatsapp-btn" target="_blank">
                <i class="fab fa-whatsapp"></i>
                تواصل عبر الواتساب
            </a>
            
            <div class="contact-methods">
                <div class="contact-method">
                    <i class="fas fa-envelope"></i>
                    <span>email@academy.com</span>
                </div>
                <div class="contact-method">
                    <i class="fas fa-phone"></i>
                    <span>+966 XX XXX XXXX</span>
                </div>
                <div class="contact-method">
                    <i class="fas fa-map-marker-alt"></i>
                    <span>السعودية | متاح للتدريب عن بعد</span>
                </div>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <p>© 2026 أكاديمية المهارات الإداريةManagement Skills Academy. جميع الحقوق محفوظة | صُنع بـ <i class="fas fa-heart" style="color: var(--secondary);"></i> في اليمن</p>
    </footer>

    <!-- JAVASCRIPT -->
    <script>
        // Animation on scroll
        const observerOptions = {
            threshold: 0.1,
            rootMargin: "0px 0px -50px 0px"
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));

        // Smooth scroll for navigation
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Mobile menu toggle (basic)
        const mobileMenu = document.querySelector('.mobile-menu');
        const nav = document.querySelector('nav');
        
        mobileMenu.addEventListener('click', () => {
            nav.style.display = nav.style.display === 'flex' ? 'none' : 'flex';
            nav.style.position = 'absolute';
            nav.style.top = '100%';
            nav.style.left = '0';
            nav.style.right = '0';
            nav.style.background = 'var(--primary)';
            nav.style.flexDirection = 'column';
            nav.style.padding = '20px';
            nav.style.boxShadow = '0 10px 20px rgba(0,0,0,0.2)';
        });
    </script>

</body>
</html>
