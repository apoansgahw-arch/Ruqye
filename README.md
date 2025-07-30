<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>رُقي - Ruqya | حلول تسويقية متكاملة</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #1a237e;     /* أزرق داكن فاخر */
            --secondary: #ff6d00;   /* برتقالي نابض */
            --accent: #00bcd4;      /* فيروزي لامع */
            --dark: #263238;        /* فحمي داكن */
            --light: #f5f7fa;       /* أبيض ناعم */
            --success: #4caf50;     /* أخضر للضمانات */
            --discount: #e91e63;    /* وردي للخصومات */
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #f5f7fa 0%, #e4e7eb 100%);
            color: #333;
            line-height: 1.8;
        }
        
        /* التصميم العام */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        section {
            padding: 80px 0;
        }
        
        h1, h2, h3, h4 {
            font-weight: 700;
            line-height: 1.3;
        }
        
        .en {
            font-family: 'Montserrat', 'Arial', sans-serif;
            font-weight: 700;
        }
        
        /* الهيدر */
        header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--dark) 100%);
            color: white;
            padding: 20px 0;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 2.5rem;
            font-weight: 800;
        }
        
        .logo .ar {
            color: var(--accent);
        }
        
        .logo .en {
            font-size: 1.8rem;
            color: var(--secondary);
        }
        
        /* القسم البطولي */
        .hero {
            background: linear-gradient(rgba(26, 35, 126, 0.9), rgba(38, 50, 56, 0.9)), url('https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-4.0.3&auto=format&fit=crop&w=1950&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 120px 20px;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
        }
        
        .hero h1 .en {
            font-size: 4rem;
            display: block;
            color: var(--secondary);
            margin-top: 10px;
        }
        
        .hero p {
            font-size: 1.5rem;
            max-width: 800px;
            margin: 0 auto 40px;
        }
        
        .cta-button {
            background: var(--secondary);
            color: white;
            padding: 15px 40px;
            border-radius: 50px;
            font-weight: 700;
            font-size: 1.2rem;
            text-decoration: none;
            display: inline-block;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(255, 109, 0, 0.4);
        }
        
        .cta-button:hover {
            background: #ff8a00;
            transform: translateY(-5px);
            box-shadow: 0 6px 20px rgba(255, 109, 0, 0.6);
        }
        
        /* قسم الباقات */
        .packages {
            background: var(--light);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }
        
        .section-title h2 {
            font-size: 2.8rem;
            color: var(--primary);
            position: relative;
            display: inline-block;
            padding-bottom: 15px;
        }
        
        .section-title h2:after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background: var(--accent);
        }
        
        .packages-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .package-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
            transition: transform 0.4s ease, box-shadow 0.4s ease;
            position: relative;
        }
        
        .package-card:hover {
            transform: translateY(-15px);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.15);
        }
        
        .package-header {
            padding: 25px;
            text-align: center;
            color: white;
        }
        
        .package-1 .package-header { background: linear-gradient(135deg, #4a148c 0%, #7b1fa2 100%); }
        .package-2 .package-header { background: linear-gradient(135deg, #0277bd 0%, #0288d1 100%); }
        .package-3 .package-header { background: linear-gradient(135deg, #d84315 0%, #ef6c00 100%); }
        .package-4 .package-header { background: linear-gradient(135deg, #00838f 0%, #0097a7 100%); }
        .package-5 .package-header { background: linear-gradient(135deg, #2e7d32 0%, #43a047 100%); }
        
        .package-title {
            font-size: 1.8rem;
            margin-bottom: 10px;
        }
        
        .price {
            font-size: 2.5rem;
            font-weight: 800;
            margin-bottom: 5px;
        }
        
        .original-price {
            text-decoration: line-through;
            opacity: 0.8;
            font-size: 1.2rem;
            margin-bottom: 15px;
            display: block;
        }
        
        .package-body {
            padding: 25px;
        }
        
        .features {
            list-style: none;
            margin-bottom: 25px;
        }
        
        .features li {
            padding: 10px 0;
            border-bottom: 1px dashed #eee;
            position: relative;
            padding-left: 30px;
        }
        
        .features li:before {
            content: '✓';
            color: var(--success);
            position: absolute;
            left: 0;
            font-weight: bold;
        }
        
        .guarantee {
            background: rgba(76, 175, 80, 0.1);
            border-left: 4px solid var(--success);
            padding: 15px;
            border-radius: 0 8px 8px 0;
            margin-top: 20px;
            font-weight: 600;
        }
        
        .highlight {
            background: linear-gradient(120deg, rgba(255, 109, 0, 0.1) 0%, rgba(255, 109, 0, 0.05) 100%);
            padding: 25px;
            border-radius: 15px;
            margin: 40px 0;
            text-align: center;
            border: 2px dashed var(--secondary);
        }
        
        .highlight h3 {
            color: var(--secondary);
            font-size: 2rem;
            margin-bottom: 15px;
        }
        
        /* قسم العملاء */
        .clients {
            background: linear-gradient(135deg, var(--dark) 0%, var(--primary) 100%);
            color: white;
            text-align: center;
        }
        
        .stats {
            font-size: 4rem;
            font-weight: 800;
            margin: 20px 0;
            color: var(--accent);
        }
        
        /* فريق العمل */
        .team {
            background: var(--light);
        }
        
        .team-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .department {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.06);
            text-align: center;
        }
        
        .department i {
            font-size: 3rem;
            color: var(--accent);
            margin-bottom: 20px;
        }
        
        .department h3 {
            color: var(--primary);
            margin-bottom: 15px;
        }
        
        /* التواصل */
        .contact {
            background: linear-gradient(135deg, var(--primary) 0%, var(--dark) 100%);
            color: white;
        }
        
        .contact-info {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 40px;
            margin-top: 40px;
        }
        
        .contact-item {
            text-align: center;
            flex: 1;
            min-width: 250px;
        }
        
        .contact-item i {
            font-size: 2.5rem;
            color: var(--accent);
            margin-bottom: 20px;
        }
        
        /* الفوتر */
        footer {
            background: var(--dark);
            color: white;
            text-align: center;
            padding: 30px 0;
            font-size: 1.1rem;
        }
        
        .social-links {
            margin: 20px 0;
        }
        
        .social-links a {
            display: inline-block;
            width: 50px;
            height: 50px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            line-height: 50px;
            margin: 0 10px;
            font-size: 1.3rem;
            transition: all 0.3s ease;
        }
        
        .social-links a:hover {
            background: var(--accent);
            transform: translateY(-5px);
        }
        
        /* التجاوبية */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .hero h1 .en {
                font-size: 2.8rem;
            }
            
            .section-title h2 {
                font-size: 2.2rem;
            }
            
            .stats {
                font-size: 3rem;
            }
        }
    </style>
</head>
<body>
    <!-- الهيدر -->
    <header>
        <div class="container header-content">
            <div class="logo">
                <span class="ar">رُقي</span> 
                <span class="en">Ruqya</span>
            </div>
            <div>
                <a href="#contact" class="cta-button">تواصل معنا الآن</a>
            </div>
        </div>
    </header>

    <!-- القسم البطولي -->
    <section class="hero">
        <div class="container">
            <h1>
                حلول تسويقية <span>استثنائية</span>
                <span class="en">Ruqya - Digital Excellence</span>
            </h1>
            <p>نحوِّل متابعيك إلى عملاء ومبيعات حقيقية باستراتيجيات مبتكرة ونتائج ملموسة</p>
            <a href="#packages" class="cta-button">اكتشف باقاتنا الاستثنائية</a>
        </div>
    </section>

    <!-- قسم الباقات -->
    <section id="packages" class="packages">
        <div class="container">
            <div class="section-title">
                <h2>باقاتنا التسويقية الاستثنائية</h2>
                <p>اختر الباقة المناسبة لتحقيق أهدافك التسويقية بأفضل الأسعار</p>
            </div>

            <div class="packages-container">
                <!-- الباقة 1 -->
                <div class="package-card package-1">
                    <div class="package-header">
                        <h3 class="package-title">الانطلاقة الذكية</h3>
                        <div class="price">50 ريال عُماني</div>
                        <span class="original-price">بدلاً من 150 ريال</span>
                    </div>
                    <div class="package-body">
                        <ul class="features">
                            <li>إدارة الحساب (إنستجرام + تيك توك) - شهر</li>
                            <li>10 منشورات احترافية (تصميم + كتابة محتوى)</li>
                            <li>إعلان واحد مدفوع مُستهدف + قابل للزيادة</li>
                            <li>تقرير أداء أسبوعي</li>
                            <li>إنشاء 15 ريلز احترافي</li>
                            <li>تحليل حسابات المنافسين في منطقتك</li>
                        </ul>
                        <div class="guarantee">
                            ➔ استرداد 100% من المبلغ إذا لم تكن الخدمة مفيدة
                        </div>
                    </div>
                </div>

                <!-- الباقة 2 -->
                <div class="package-card package-2">
                    <div class="package-header">
                        <h3 class="package-title">القفزة النوعية</h3>
                        <div class="price">149 ريال عُماني</div>
                        <span class="original-price">بدلاً من 300 ريال</span>
                    </div>
                    <div class="package-body">
                        <ul class="features">
                            <li>إدارة الحساب - 45 يومًا</li>
                            <li>25 منشورًا + 20 ريلز احترافية</li>
                            <li>3 إعلانات مدفوعة (تيك توك + إنستجرام) + قابلة للزيادة</li>
                            <li>تحليل المنافسين + نصائح تطوير</li>
                            <li>دعم يومي عبر الواتساب</li>
                            <li>تقرير يومي عن الحالة</li>
                            <li>استشارات مفتوحة وحلول جذرية</li>
                        </ul>
                        <div class="guarantee">
                            ➔ استرداد 50% إذا لم تزد مبيعاتك 25% خلال الشهر
                        </div>
                    </div>
                </div>

                <!-- الباقة 3 -->
                <div class="package-card package-3">
                    <div class="package-header">
                        <h3 class="package-title">التحوّل الشامل</h3>
                        <div class="price">350 ريال عُماني</div>
                        <span class="original-price">بدلاً من 549 ريال</span>
                    </div>
                    <div class="package-body">
                        <ul class="features">
                            <li>إدارة شاملة (3 منصات: إنستجرام + تيك توك + فيسبوك)</li>
                            <li>45 محتوى شهريًا (منشورات - ريلز - ستوريات)</li>
                            <li>10 إعلانات مدفوعة باستهداف متطور</li>
                            <li>فيديو دعائي احترافي (60 ثانية)</li>
                            <li>خطة تسويقية سنوية مجانية</li>
                            <li>دعم يومي عبر واتساب</li>
                            <li>استشارات مفتوحة وحلول جذرية</li>
                            <li>تحليل المنافسين الشامل</li>
                        </ul>
                        <div class="guarantee">
                            ➔ استرداد 100% إذا لم تحقق 40% زيادة في المبيعات خلال 45 يومًا
                        </div>
                    </div>
                </div>

                <!-- الباقة 4 -->
                <div class="package-card package-4">
                    <div class="package-header">
                        <h3 class="package-title">إنطلاقة ذكية</h3>
                        <div class="price">30 ريال عُماني</div>
                        <span class="original-price">بدلاً من 45 ريال</span>
                    </div>
                    <div class="package-body">
                        <ul class="features">
                            <li>إدارة الحساب (إنستجرام + تيك توك) - شهر / 24 ساعة يوميا</li>
                            <li>تنسيق إعلانات مدفوعة مستهدفة (الرسوم على العميل)</li>
                            <li>تنسيق إعلان مدفوع مخصص (الرسوم على الشركة)</li>
                            <li>تقرير أداء أسبوعي</li>
                            <li>تحليل الحساب وإعطاء حلول واستشارات</li>
                            <li>تحليل حسابات المنافسين في منطقتك</li>
                        </ul>
                        <div class="guarantee">
                            ➔ استرداد 100% من المبلغ إذا لم تكن الخدمة مفيدة
                        </div>
                        <p><strong>🔴 يمكن تعديل الباقة وإضافة خدمات أو حذفها واستبدالها</strong></p>
                    </div>
                </div>

                <!-- الباقة 5 -->
                <div class="package-card package-5">
                    <div class="package-header">
                        <h3 class="package-title">بداية الطريق خطوة</h3>
                        <div class="price">15 ريال عُماني</div>
                        <span class="original-price">بدلاً من 25 ريال</span>
                    </div>
                    <div class="package-body">
                        <ul class="features">
                            <li>إدارة الحساب (إنستجرام + تيك توك) - شهر</li>
                            <li>تنسيق إعلانات مدفوعة مخصصة</li>
                        </ul>
                        <p><strong>🔴 يمكن إضافة خدمات أخرى</strong></p>
                        <div class="guarantee">
                            <strong>هدية مع الباقة:</strong>
                            <p>✅ تقرير أداء أسبوعي</p>
                            <p>✅ تحليل الحساب وإعطاء حلول واستشارات</p>
                            <p>✅ تحليل حسابات المنافسين في منطقتك</p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="highlight">
                <h3>عروض خاصة!</h3>
                <p>تخفيض 15% على الباقة المتوسطة والمتقدمة للمشتركين الجدد</p>
                <p>هدايا إضافية للمشتركين في الباقة الصغرى</p>
            </div>
        </div>
    </section>

    <!-- قسم العملاء -->
    <section class="clients">
        <div class="container">
            <h2>ثقة عملائنا هي شهادتنا</h2>
            <div class="stats">168+</div>
            <p>عميل راضٍ حول العالم يثقون بخدماتنا التسويقية المتكاملة</p>
        </div>
    </section>

    <!-- فريق العمل -->
    <section class="team">
        <div class="container">
            <div class="section-title">
                <h2>فريق العمل الاحترافي</h2>
                <p>خبراء متخصصون يعملون معاً لتحقيق أهدافك</p>
            </div>

            <div class="team-grid">
                <div class="department">
                    <i class="fas fa-bullhorn"></i>
                    <h3>قسم التسويق</h3>
                    <p>استراتيجيات تسويقية مبتكرة تواكب أحدث الاتجاهات</p>
                </div>
                
                <div class="department">
                    <i class="fas fa-paint-brush"></i>
                    <h3>قسم التصميم</h3>
                    <p>تصميمات إبداعية تجذب الأنظار وتعبر عن هويتك</p>
                </div>
                
                <div class="department">
                    <i class="fas fa-users-cog"></i>
                    <h3>إدارة الحسابات</h3>
                    <p>إدارة احترافية لمنصات التواصل الاجتماعي على مدار الساعة</p>
                </div>
                
                <div class="department">
                    <i class="fas fa-chart-line"></i>
                    <h3>تدقيق وتحليل</h3>
                    <p>تحليل أداء دقيق وخطط تطوير قائمة على البيانات</p>
                </div>
                
                <div class="department">
                    <i class="fas fa-user-tie"></i>
                    <h3>الإدارة</h3>
                    <p>تنسيق متكامل لضمان جودة الخدمة وتحقيق الأهداف</p>
                </div>
            </div>
        </div>
    </section>

    <!-- التواصل -->
    <section id="contact" class="contact">
        <div class="container">
            <div class="section-title">
                <h2>تواصل معنا الآن</h2>
                <p>نحن جاهزون لبدء رحلتك التسويقية نحو التميز</p>
            </div>

            <div class="contact-info">
                <div class="contact-item">
                    <i class="fas fa-phone"></i>
                    <h3>هاتف</h3>
      <p>+968 77522669</p>
                </div>
                
                <div class="contact-item">
                    <i class="fas fa-envelope"></i>
                    <h3>البريد الإلكتروني</h3>
                    <p>omdasolu@gmail.com</p>
                </div>
                
                <div class="contact-item">
                    <i class="fas fa-clock"></i>
                    <h3>ساعات العمل</h3>
                    <p>24/7 على مدار الساعة</p>
                </div>
            </div>
        </div>
    </section>

    <!-- الفوتر -->
    <footer>
        <div class="container">
            <div class="logo">
                <span class="ar">رُقي</span> 
                <span class="en">Ruqya</span>
            </div>
            <p>حلول تسويقية استثنائية تحقق نتائج ملموسة</p>
            
            <div class="social-links">
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-tiktok"></i></a>
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-whatsapp"></i></a>
            </div>
            
            <p>© 2023 رُقي - Ruqya. جميع الحقوق محفوظة</p>
        </div>
    </footer>
</body>
</html>
