<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>متجر الاشتراكات الرقمية</title>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --bg-color: #0f0f13;
            --card-bg: #1c1c24;
            --primary-color: #e50914; /* لون نتفليكس كمثال */
            --text-color: #ffffff;
            --text-muted: #a0a0b0;
            --whatsapp-color: #25D366;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Cairo', sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
        }

        header {
            text-align: center;
            padding: 60px 20px;
            background: linear-gradient(to bottom, #14141a, var(--bg-color));
            border-bottom: 1px solid #2a2a35;
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        header p {
            color: var(--text-muted);
            font-size: 1.2rem;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        /* شبكة المنتجات */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 25px;
        }

        /* تصميم الكارت */
        .card {
            background-color: var(--card-bg);
            border-radius: 15px;
            padding: 25px;
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: 1px solid #2a2a35;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.5);
            border-color: var(--primary-color);
        }

        .service-icon {
            font-size: 3rem;
            margin-bottom: 15px;
            color: var(--text-color);
        }

        .netflix-icon { color: #e50914; }
        .spotify-icon { color: #1DB954; }
        .youtube-icon { color: #FF0000; }
        .amazon-icon { color: #FF9900; }

        .card h3 {
            font-size: 1.5rem;
            margin-bottom: 10px;
        }

        .price {
            font-size: 1.8rem;
            font-weight: 800;
            color: var(--primary-color);
            margin-bottom: 5px;
        }

        .price span {
            font-size: 1rem;
            color: var(--text-muted);
            font-weight: 400;
        }

        .features {
            list-style: none;
            margin: 15px 0;
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        .features li {
            margin-bottom: 8px;
        }

        .btn-whatsapp {
            display: inline-block;
            width: 100%;
            background-color: var(--whatsapp-color);
            color: white;
            text-decoration: none;
            padding: 12px;
            border-radius: 8px;
            font-weight: bold;
            font-size: 1.1rem;
            transition: background 0.3s;
            margin-top: 10px;
        }

        .btn-whatsapp i {
            margin-left: 8px;
        }

        .btn-whatsapp:hover {
            background-color: #1ebe57;
        }

        /* زر واتساب العائم للمساعدة العامة */
        .floating-whatsapp {
            position: fixed;
            bottom: 30px;
            left: 30px;
            background-color: var(--whatsapp-color);
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            box-shadow: 0 4px 10px rgba(0,0,0,0.3);
            text-decoration: none;
            z-index: 1000;
            transition: transform 0.3s;
        }

        .floating-whatsapp:hover {
            transform: scale(1.1);
        }
    </style>
</head>
<body>

    <header>
        <h1>متجر الاشتراكات الرقمية</h1>
        <p>أفضل أسعار الاشتراكات لأكثر من 50 خدمة عالمية والتسليم فوري</p>
    </header>

    <div class="container">
        <div class="services-grid">
            
            <div class="card">
                <i class="fa-brands fa-neos service-icon netflix-icon"></i>
                <h3>اشتراك نتفليكس</h3>
                <div class="price">40<span> درهم / شهر</span></div>
                <ul class="features">
                    <li>باقة 4K Ultra HD</li>
                    <li>ملف شخصي خاص بك</li>
                    <li>ضمان كامل المدة</li>
                </ul>
                <a href="https://wa.me/21260040895?text=أهلاً، أريد طلب اشتراك نتفليكس" class="btn-whatsapp" target="_blank">
                    <i class="fa-brands fa-whatsapp"></i> اطلب الآن
                </a>
            </div>

            <div class="card">
                <i class="fa-brands fa-youtube service-icon youtube-icon"></i>
                <h3>يوتيوب بريميوم</h3>
                <div class="price">25<span> درهم / شهر</span></div>
                <ul class="features">
                    <li>بدون إعلانات مزعجة</li>
                    <li>تشغيل في الخلفية</li>
                    <li>تفعيل على حسابك الشخصي</li>
                </ul>
                <a href="https://wa.me/212660040895?text=أهلاً، أريد طلب اشتراك يوتيوب بريميوم" class="btn-whatsapp" target="_blank">
                    <i class="fa-brands fa-whatsapp"></i> اطلب الآن
                </a>
            </div>

            <div class="card">
                <i class="fa-brands fa-spotify service-icon spotify-icon"></i>
                <h3>سبوتيفاي بريميوم</h3>
                <div class="price">20<span> درهم / شهر</span></div>
                <ul class="features">
                    <li>استماع بدون إنترنت</li>
                    <li>بدون إعلانات</li>
                    <li>تفعيل على حسابك</li>
                </ul>
                <a href="https://wa.me/212660040895?text=أهلاً، أريد طلب اشتراك سبوتيفاي" class="btn-whatsapp" target="_blank">
                    <i class="fa-brands fa-whatsapp"></i> اطلب الآن
                </a>
            </div>

            <div class="card">
                <i class="fa-brands fa-amazon service-icon amazon-icon"></i>
                <h3>أمازون برايم فيديو</h3>
                <div class="price">30<span> درهم / شهر</span></div>
                <ul class="features">
                    <li>أفلام ومسلسلات حصرية</li>
                    <li>جودة عالية 4K</li>
                    <li>ضمان ذهبي</li>
                </ul>
                <a href="https://wa.me/212660040895?text=أهلاً، أريد طلب اشتراك أمازون برايم" class="btn-whatsapp" target="_blank">
                    <i class="fa-brands fa-whatsapp"></i> اطلب الآن
                </a>
            </div>

            </div>
    </div>

    <a href="https://wa.me/212660040895?text=أهلاً، لدي استفسار بخصوص الاشتراكات" class="floating-whatsapp" target="_blank">
        <i class="fa-brands fa-whatsapp"></i>
    </a>

</body>
</html>
