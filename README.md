<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
    <title>Paulina Accesorios - Belleza y Estilo Premium</title>

    <!-- ===== SEO ===== -->
    <meta name="description" content="Paulina Accesorios - Tienda de aretes, extensiones de pestañas y accesorios de belleza. Envíos a todo Perú. Calidad premium." />
    <meta name="keywords" content="aretes, pestañas, accesorios, belleza, joyería, maquillaje, extensiones, anillos, moda, tendencias, yurimaguas" />
    <meta name="author" content="Paulina Accesorios" />
    <meta name="robots" content="index, follow" />

    <!-- ===== OPEN GRAPH ===== -->
    <meta property="og:title" content="Paulina Accesorios - Belleza y Estilo Premium ✨" />
    <meta property="og:description" content="Descubre nuestra colección exclusiva de accesorios de belleza. Aretes, pestañas, joyería y más. Envíos a todo Perú." />
    <meta property="og:type" content="website" />
    <meta property="og:locale" content="es_PE" />

    <!-- ===== TWITTER CARDS ===== -->
    <meta name="twitter:card" content="summary_large_image" />
    <meta name="twitter:title" content="Paulina Accesorios - Belleza y Estilo Premium" />
    <meta name="twitter:description" content="Accesorios de belleza de la más alta calidad. Envíos a todo Perú." />

    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;700;900&family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet" />

    <style>
        /* ============================================
           RESET Y BASE
           ============================================ */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #c2185b;
            --primary-dark: #880e4f;
            --primary-light: #f06292;
            --secondary: #6a1b4d;
            --accent: #f9a825;
            --bg-light: #fef8fb;
            --bg-dark: #1a0b1a;
            --text-light: #e8d5e8;
            --text-dark: #2d1b2e;
            --shadow: 0 8px 40px rgba(200, 120, 180, 0.12);
            --shadow-hover: 0 20px 60px rgba(194, 24, 91, 0.2);
            --radius: 30px;
            --radius-sm: 16px;
            --transition: all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
            --font-serif: 'Playfair Display', serif;
            --font-sans: 'Inter', sans-serif;
        }

        html {
            scroll-behavior: smooth;
            scroll-padding-top: 80px;
        }

        body {
            font-family: var(--font-sans);
            background: var(--bg-light);
            color: var(--text-dark);
            line-height: 1.7;
            transition: var(--transition);
            overflow-x: hidden;
        }

        /* ============================================
           MODO OSCURO
           ============================================ */
        body.dark-mode {
            --bg-light: #0a050a;
            --text-dark: #f0e8f0;
            background: #0a050a;
            color: #f0e8f0;
        }

        body.dark-mode .navbar {
            background: rgba(10, 5, 10, 0.95);
            border-bottom: 1px solid rgba(255, 182, 193, 0.05);
        }
        body.dark-mode .nav-links a {
            color: #f0e8f0;
        }
        body.dark-mode .hero {
            background: linear-gradient(135deg, #1a0b1a, #0a050a, #2d1b2e);
        }
        body.dark-mode .product-card,
        body.dark-mode .testimonial,
        body.dark-mode .tip-card,
        body.dark-mode .contact-form,
        body.dark-mode .cart-modal-content,
        body.dark-mode .notification,
        body.dark-mode .map-info,
        body.dark-mode .payment-methods,
        body.dark-mode .faq-item,
        body.dark-mode .popup-content,
        body.dark-mode .floating-cart,
        body.dark-mode .live-notification {
            background: #1a0b1a;
            border-color: rgba(255, 182, 193, 0.04);
        }
        body.dark-mode .banner,
        body.dark-mode .newsletter-section {
            background: linear-gradient(135deg, #1a0b1a, #0a050a);
        }
        body.dark-mode .banner h2,
        body.dark-mode .banner p,
        body.dark-mode .section-title,
        body.dark-mode .section-subtitle {
            color: #f0e8f0;
        }
        body.dark-mode .cart-icon,
        body.dark-mode .search-box {
            background: rgba(255, 255, 255, 0.03);
            border-color: rgba(255, 182, 193, 0.05);
        }
        body.dark-mode .search-box input,
        body.dark-mode .search-box button {
            color: #f0e8f0;
        }
        body.dark-mode .category-pills .pill {
            background: #1a0b1a;
            color: #f0e8f0;
            border-color: rgba(255, 182, 193, 0.05);
        }
        body.dark-mode .category-pills .pill.active {
            background: linear-gradient(135deg, var(--primary), var(--primary-light));
            color: #fff;
        }
        body.dark-mode .btn-secondary {
            background: rgba(255, 255, 255, 0.05);
            color: #f0e8f0;
            border-color: var(--primary);
        }
        body.dark-mode .btn-secondary:hover {
            background: var(--primary);
            color: #fff;
        }
        body.dark-mode .product-card .product-img {
            background: linear-gradient(135deg, #2d1b2e, #1a0b1a);
        }
        body.dark-mode .btn-add {
            background: rgba(255, 255, 255, 0.05);
            color: #f0e8f0;
            border-color: rgba(255, 182, 193, 0.05);
        }
        body.dark-mode .btn-add:hover {
            background: linear-gradient(135deg, var(--primary), var(--primary-light));
            color: #fff;
        }
        body.dark-mode .contact-form input,
        body.dark-mode .contact-form textarea,
        body.dark-mode .newsletter-form input,
        body.dark-mode .popup-content .popup-input input {
            background: #0a050a;
            color: #f0e8f0;
            border-color: rgba(255, 182, 193, 0.05);
        }
        body.dark-mode .timer .time-block {
            background: rgba(26, 11, 26, 0.6);
            border-color: rgba(255, 182, 193, 0.05);
        }
        body.dark-mode .hero-stats .stat {
            background: rgba(255, 255, 255, 0.03);
            border-color: rgba(255, 255, 255, 0.03);
        }
        body.dark-mode .hero-stats .stat .label {
            color: #9a7a9a;
        }
        body.dark-mode .security-badge {
            background: rgba(255, 255, 255, 0.03);
            color: #f0e8f0;
        }
        body.dark-mode .coupon-section {
            background: rgba(255, 255, 255, 0.02);
            border-color: rgba(255, 182, 193, 0.05);
        }
        body.dark-mode .coupon-section .coupon-code {
            color: var(--primary-light);
        }
        body.dark-mode .social-links .social-link:hover {
            transform: scale(1.15) translateY(-6px);
        }
        body.dark-mode .floating-cart .fc-total {
            color: var(--primary-light);
        }
        body.dark-mode .cart-total .total-price {
            color: var(--primary-light);
        }
        body.dark-mode .faq-item .faq-answer {
            color: #c9a8c9;
        }
        body.dark-mode .product-card .desc,
        body.dark-mode .product-card .seen-time,
        body.dark-mode .testimonial p,
        body.dark-mode .tip-card p,
        body.dark-mode .map-info p {
            color: #c9a8c9;
        }
        body.dark-mode .testimonial .date {
            color: #7a4a7a;
        }
        body.dark-mode .price-filter {
            background: rgba(255, 255, 255, 0.02);
            border-color: rgba(255, 182, 193, 0.03);
        }
        body.dark-mode .price-filter label {
            color: #f0e8f0;
        }
        body.dark-mode .price-filter input {
            background: #0a050a;
            color: #f0e8f0;
            border-color: rgba(255, 182, 193, 0.05);
        }
        body.dark-mode .sort-options label {
            color: #f0e8f0;
        }
        body.dark-mode .sort-options select {
            background: #0a050a;
            color: #f0e8f0;
            border-color: rgba(255, 182, 193, 0.05);
        }
        body.dark-mode .popup-content .popup-timer .time-block {
            background: #0a050a;
        }
        body.dark-mode .popup-content .popup-timer .time-block span {
            color: var(--primary-light);
        }
        body.dark-mode .popup-content .popup-timer .time-block .label {
            color: #9a7a9a;
        }
        body.dark-mode .social-section {
            background: rgba(255, 255, 255, 0.02) !important;
            border-color: rgba(255, 182, 193, 0.03) !important;
        }
        body.dark-mode .social-section p {
            color: #c9a8c9 !important;
        }

        /* ============================================
           SCROLLBAR
           ============================================ */
        ::-webkit-scrollbar {
            width: 10px;
        }
        ::-webkit-scrollbar-track {
            background: var(--bg-light);
        }
        ::-webkit-scrollbar-thumb {
            background: linear-gradient(180deg, var(--primary), var(--primary-light), var(--primary-dark));
            border-radius: 10px;
            border: 2px solid var(--bg-light);
        }
        ::-webkit-scrollbar-thumb:hover {
            background: var(--primary-dark);
        }

        /* ============================================
           PRELOADER
           ============================================ */
        .preloader {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--bg-light);
            z-index: 99999;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            transition: opacity 0.8s ease, visibility 0.8s ease;
        }
        .preloader.hidden {
            opacity: 0;
            visibility: hidden;
        }
        .preloader .loader-ring {
            position: relative;
            width: 80px;
            height: 80px;
        }
        .preloader .loader-ring .ring {
            position: absolute;
            border: 4px solid transparent;
            border-radius: 50%;
            animation: ringSpin 1.2s cubic-bezier(0.5, 0, 0.5, 1) infinite;
        }
        .preloader .loader-ring .ring:nth-child(1) {
            width: 80px;
            height: 80px;
            border-top-color: var(--primary);
            animation-delay: -0.45s;
        }
        .preloader .loader-ring .ring:nth-child(2) {
            width: 60px;
            height: 60px;
            top: 10px;
            left: 10px;
            border-top-color: var(--primary-light);
            animation-delay: -0.3s;
        }
        .preloader .loader-ring .ring:nth-child(3) {
            width: 40px;
            height: 40px;
            top: 20px;
            left: 20px;
            border-top-color: var(--accent);
            animation-delay: -0.15s;
        }
        @keyframes ringSpin {
            0% {
                transform: rotate(0deg);
            }
            100% {
                transform: rotate(360deg);
            }
        }
        .preloader .loader-text {
            margin-top: 30px;
            font-family: var(--font-serif);
            color: var(--primary);
            font-size: 1.4rem;
            letter-spacing: 4px;
            animation: pulseText 1.5s ease-in-out infinite;
        }
        @keyframes pulseText {
            0%,
            100% {
                opacity: 0.6;
            }
            50% {
                opacity: 1;
            }
        }

        /* ============================================
           ENVÍO GRATIS
           ============================================ */
        .free-shipping {
            background: linear-gradient(135deg, #2e7d32, #43a047, #2e7d32);
            background-size: 300% 300%;
            animation: gradientMove 4s ease infinite;
            color: #fff;
            text-align: center;
            padding: 0.6rem;
            font-weight: 700;
            font-size: 0.9rem;
            position: sticky;
            top: 0;
            z-index: 1001;
            letter-spacing: 0.5px;
            box-shadow: 0 2px 20px rgba(46, 125, 50, 0.2);
        }
        @keyframes gradientMove {
            0%,
            100% {
                background-position: 0% 50%;
            }
            50% {
                background-position: 100% 50%;
            }
        }
        .free-shipping .highlight {
            font-weight: 800;
            text-decoration: underline;
            text-underline-offset: 3px;
        }

        /* ============================================
           MODO OSCURO TOGGLE
           ============================================ */
        .dark-mode-toggle {
            position: fixed;
            bottom: 200px;
            right: 2rem;
            background: linear-gradient(135deg, var(--primary-dark), var(--primary), var(--primary-light));
            color: #fff;
            width: 58px;
            height: 58px;
            border-radius: 50%;
            border: none;
            font-size: 1.6rem;
            cursor: pointer;
            z-index: 999;
            box-shadow: 0 4px 30px rgba(194, 24, 91, 0.4);
            transition: var(--transition);
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .dark-mode-toggle:hover {
            transform: scale(1.12) rotate(20deg);
            box-shadow: 0 8px 50px rgba(194, 24, 91, 0.5);
        }
        @media (max-width: 750px) {
            .dark-mode-toggle {
                width: 48px;
                height: 48px;
                font-size: 1.3rem;
                bottom: 180px;
                right: 1rem;
            }
        }

        /* ============================================
           MENÚ HAMBURGUESA
           ============================================ */
        .hamburger {
            display: none;
            flex-direction: column;
            cursor: pointer;
            gap: 6px;
            padding: 5px;
            z-index: 1001;
        }
        .hamburger span {
            width: 32px;
            height: 3px;
            background: var(--text-dark);
            border-radius: 5px;
            transition: var(--transition);
        }
        body.dark-mode .hamburger span {
            background: #f0e8f0;
        }
        .hamburger.active span:nth-child(1) {
            transform: rotate(45deg) translate(6px, 7px);
        }
        .hamburger.active span:nth-child(2) {
            opacity: 0;
            transform: translateX(-15px);
        }
        .hamburger.active span:nth-child(3) {
            transform: rotate(-45deg) translate(6px, -7px);
        }

        .mobile-menu {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(255, 255, 255, 0.98);
            backdrop-filter: blur(30px);
            z-index: 1000;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 2.5rem;
        }
        body.dark-mode .mobile-menu {
            background: rgba(10, 5, 10, 0.98);
        }
        .mobile-menu.open {
            display: flex;
            animation: fadeInMobile 0.4s ease;
        }
        @keyframes fadeInMobile {
            from {
                opacity: 0;
                transform: scale(0.95) translateY(20px);
            }
            to {
                opacity: 1;
                transform: scale(1) translateY(0);
            }
        }
        .mobile-menu a {
            font-size: 2rem;
            text-decoration: none;
            color: var(--text-dark);
            font-weight: 700;
            transition: var(--transition);
            font-family: var(--font-serif);
            letter-spacing: 1px;
        }
        body.dark-mode .mobile-menu a {
            color: #f0e8f0;
        }
        .mobile-menu a:hover {
            color: var(--primary);
            transform: translateX(10px) scale(1.05);
        }

        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            .hamburger {
                display: flex;
            }
        }

        /* ============================================
           NAVBAR
           ============================================ */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0.8rem 5%;
            background: rgba(255, 255, 255, 0.92);
            backdrop-filter: blur(25px);
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 40px rgba(200, 120, 180, 0.06);
            border-bottom: 1px solid rgba(255, 182, 193, 0.06);
            flex-wrap: wrap;
            gap: 0.5rem;
            transition: var(--transition);
        }
        .logo {
            font-family: var(--font-serif);
            font-size: 2rem;
            font-weight: 900;
            background: linear-gradient(135deg, var(--primary-dark), var(--primary), var(--primary-light), var(--accent));
            -webkit-background-clip: text;
            background-clip: text;
            -webkit-text-fill-color: transparent;
            color: transparent;
            cursor: pointer;
            letter-spacing: -0.5px;
            transition: var(--transition);
        }
        .logo:hover {
            transform: scale(1.03);
        }
        .nav-links {
            display: flex;
            gap: 2.5rem;
            list-style: none;
            font-weight: 600;
            flex-wrap: wrap;
        }
        .nav-links a {
            text-decoration: none;
            color: var(--text-dark);
            font-size: 0.95rem;
            transition: var(--transition);
            position: relative;
        }
        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -4px;
            left: 0;
            width: 0;
            height: 3px;
            background: linear-gradient(90deg, var(--primary), var(--primary-light), var(--accent));
            transition: var(--transition);
            border-radius: 10px;
        }
        .nav-links a:hover::after {
            width: 100%;
        }
        .nav-links a:hover {
            color: var(--primary);
            transform: translateY(-2px);
        }
        .nav-right {
            display: flex;
            align-items: center;
            gap: 1.5rem;
            flex-wrap: wrap;
        }

        /* ===== BUSCADOR ===== */
        .search-box {
            display: flex;
            align-items: center;
            gap: 0.3rem;
            background: rgba(214, 51, 132, 0.04);
            border-radius: 50px;
            padding: 0.2rem 0.5rem 0.2rem 1.2rem;
            border: 1.5px solid rgba(214, 51, 132, 0.06);
            transition: var(--transition);
        }
        .search-box:focus-within {
            border-color: var(--primary);
            box-shadow: 0 0 0 5px rgba(194, 24, 91, 0.06);
            transform: scale(1.02);
        }
        .search-box input {
            border: none;
            background: transparent;
            padding: 0.5rem 0;
            font-size: 0.85rem;
            font-family: var(--font-sans);
            color: var(--text-dark);
            outline: none;
            width: 150px;
            font-weight: 400;
        }
        .search-box input::placeholder {
            color: #aaa;
            font-weight: 300;
        }
        .search-box button {
            background: none;
            border: none;
            font-size: 1.2rem;
            cursor: pointer;
            padding: 0.3rem 0.6rem;
            color: var(--text-dark);
            transition: var(--transition);
        }
        .search-box button:hover {
            color: var(--primary);
            transform: scale(1.15);
        }
        @media (max-width: 480px) {
            .search-box input {
                width: 100px;
                font-size: 0.75rem;
            }
            .search-box {
                padding: 0.1rem 0.3rem 0.1rem 0.6rem;
            }
            .search-box button {
                font-size: 1rem;
            }
        }

        /* ===== CARRITO ===== */
        .cart-icon {
            font-size: 1.5rem;
            cursor: pointer;
            transition: var(--transition);
            background: linear-gradient(135deg, #fce4ec, #f8e8f0);
            padding: 0.4rem 1.2rem;
            border-radius: 50px;
            border: 1.5px solid rgba(214, 51, 132, 0.06);
            display: flex;
            align-items: center;
            gap: 0.4rem;
            font-weight: 600;
        }
        .cart-icon:hover {
            transform: scale(1.08);
            box-shadow: 0 4px 25px rgba(214, 51, 132, 0.12);
            border-color: var(--primary);
        }
        .cart-count {
            background: linear-gradient(135deg, var(--primary), var(--primary-light));
            color: #fff;
            border-radius: 50%;
            padding: 0.05rem 0.5rem;
            font-size: 0.7rem;
            font-weight: 700;
            min-width: 22px;
            text-align: center;
        }

        /* ============================================
           HERO
           ============================================ */
        .hero {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: space-between;
            padding: 4.5rem 5% 5.5rem;
            background: linear-gradient(135deg, #fce4ec 0%, #f8e8f0 20%, #f3e5f5 40%, #e8eaf6 60%, #fce4ec 80%, #f8e8f0 100%);
            background-size: 400% 400%;
            animation: heroGradient 12s ease infinite;
            border-radius: 0 0 90px 90px;
            margin: 0 1.5rem 2.5rem;
            position: relative;
            overflow: hidden;
            transition: var(--transition);
        }
        @keyframes heroGradient {
            0%,
            100% {
                background-position: 0% 50%;
            }
            25% {
                background-position: 50% 0%;
            }
            50% {
                background-position: 100% 50%;
            }
            75% {
                background-position: 50% 100%;
            }
        }
        .hero::before {
            content: '✨';
            font-size: 20rem;
            position: absolute;
            right: -5rem;
            bottom: -6rem;
            opacity: 0.04;
            transform: rotate(15deg);
            animation: floatHero 7s ease-in-out infinite;
        }
        .hero::after {
            content: '🌸';
            font-size: 10rem;
            position: absolute;
            left: 1rem;
            top: 0.5rem;
            opacity: 0.05;
            animation: floatHero 9s ease-in-out infinite reverse;
        }
        @keyframes floatHero {
            0%,
            100% {
                transform: translateY(0) rotate(0deg) scale(1);
            }
            50% {
                transform: translateY(-30px) rotate(10deg) scale(1.05);
            }
        }
        .hero-text {
            flex: 1 1 450px;
            z-index: 2;
        }
        .hero-text .brand-tag {
            font-size: 0.85rem;
            font-weight: 700;
            color: var(--primary);
            background: rgba(214, 51, 132, 0.08);
            padding: 0.4rem 1.8rem;
            border-radius: 50px;
            display: inline-block;
            margin-bottom: 1rem;
            letter-spacing: 3px;
            text-transform: uppercase;
            border: 1px solid rgba(214, 51, 132, 0.08);
            backdrop-filter: blur(8px);
        }
        .hero-text h1 {
            font-family: var(--font-serif);
            font-size: 4.2rem;
            line-height: 1.05;
            background: linear-gradient(135deg, #2d1b2e, var(--primary-dark), var(--primary), var(--primary-light), var(--accent));
            -webkit-background-clip: text;
            background-clip: text;
            -webkit-text-fill-color: transparent;
            color: transparent;
            margin-bottom: 0.8rem;
            animation: shimmerText 5s ease-in-out infinite;
        }
        .hero-text h1 .highlight {
            background: linear-gradient(135deg, var(--accent), var(--primary-light), var(--primary), var(--primary-dark));
            -webkit-background-clip: text;
            background-clip: text;
            -webkit-text-fill-color: transparent;
            color: transparent;
        }
        .hero-text p {
            font-size: 1.2rem;
            color: #4a2c4a;
            max-width: 520px;
            margin-bottom: 2rem;
            font-weight: 300;
            line-height: 1.8;
        }
        body.dark-mode .hero-text p {
            color: #c9a8c9;
        }

        .hero-stats {
            display: flex;
            gap: 2rem;
            margin-top: 1.5rem;
            flex-wrap: wrap;
        }
        .hero-stats .stat {
            text-align: center;
            background: rgba(255, 255, 255, 0.3);
            backdrop-filter: blur(12px);
            padding: 0.8rem 1.8rem;
            border-radius: var(--radius-sm);
            border: 1px solid rgba(255, 255, 255, 0.15);
            transition: var(--transition);
        }
        .hero-stats .stat:hover {
            transform: translateY(-6px);
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.04);
        }
        .hero-stats .stat .number {
            font-size: 2.2rem;
            font-weight: 800;
            color: var(--primary);
            display: block;
            font-family: var(--font-serif);
        }
        .hero-stats .stat .label {
            font-size: 0.8rem;
            color: #7a4a7a;
            font-weight: 500;
        }
        body.dark-mode .hero-stats .stat {
            background: rgba(255, 255, 255, 0.02);
            border-color: rgba(255, 255, 255, 0.02);
        }
        body.dark-mode .hero-stats .stat .label {
            color: #9a7a9a;
        }

        .btn-primary {
            display: inline-block;
            padding: 1rem 4rem;
            background: linear-gradient(135deg, var(--primary-dark), var(--primary), var(--primary-light));
            color: #fff;
            border: none;
            border-radius: 50px;
            font-weight: 700;
            font-size: 1rem;
            text-decoration: none;
            box-shadow: 0 8px 40px rgba(194, 24, 91, 0.3);
            transition: var(--transition);
            cursor: pointer;
            position: relative;
            overflow: hidden;
            letter-spacing: 0.5px;
        }
        .btn-primary::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.15), transparent);
            transition: var(--transition);
        }
        .btn-primary:hover::before {
            left: 100%;
        }
        .btn-primary:hover {
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 14px 60px rgba(194, 24, 91, 0.4);
        }

        .btn-secondary {
            display: inline-block;
            padding: 1rem 3.2rem;
            background: rgba(255, 255, 255, 0.5);
            backdrop-filter: blur(12px);
            color: var(--secondary);
            border: 2px solid var(--primary);
            border-radius: 50px;
            font-weight: 700;
            font-size: 1rem;
            text-decoration: none;
            transition: var(--transition);
            margin-left: 1rem;
            letter-spacing: 0.5px;
        }
        .btn-secondary:hover {
            background: var(--primary);
            color: #fff;
            border-color: var(--primary);
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 8px 35px rgba(194, 24, 91, 0.15);
        }

        .hero-image {
            flex: 1 1 320px;
            text-align: center;
            z-index: 2;
            font-size: 9rem;
            filter: drop-shadow(0 30px 80px rgba(194, 24, 91, 0.1));
        }
        .hero-image span {
            display: inline-block;
            animation: floatHeroImage 7s ease-in-out infinite;
        }
        @keyframes floatHeroImage {
            0%,
            100% {
                transform: translateY(0) rotate(-3deg) scale(1);
            }
            50% {
                transform: translateY(-30px) rotate(3deg) scale(1.05);
            }
        }

        @media (max-width: 750px) {
            .hero-text h1 {
                font-size: 2.8rem;
            }
            .hero {
                padding: 2.5rem 1.5rem 3.5rem;
                border-radius: 0 0 50px 50px;
                margin: 0 0.8rem 1.5rem;
            }
            .btn-secondary {
                margin-left: 0;
                margin-top: 0.6rem;
            }
            .hero-image {
                font-size: 5.5rem;
            }
            .hero-stats {
                gap: 1rem;
            }
            .hero-stats .stat .number {
                font-size: 1.6rem;
            }
            .hero-stats .stat {
                padding: 0.5rem 1.2rem;
            }
        }
        @media (max-width: 480px) {
            .hero-text h1 {
                font-size: 2.2rem;
            }
            .hero-text .brand-tag {
                font-size: 0.7rem;
                padding: 0.2rem 1rem;
            }
            .hero-text p {
                font-size: 1rem;
            }
            .hero-image {
                font-size: 4.5rem;
            }
            .btn-primary,
            .btn-secondary {
                padding: 0.7rem 2rem;
                font-size: 0.9rem;
            }
        }

        /* ============================================
           SECCIONES
           ============================================ */
        .section {
            padding: 4.5rem 5%;
            max-width: 1400px;
            margin: 0 auto;
            animation: fadeInSection 0.8s ease;
        }
        @keyframes fadeInSection {
            from {
                opacity: 0;
                transform: translateY(40px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        .section-title {
            font-family: var(--font-serif);
            font-size: 3rem;
            text-align: center;
            margin-bottom: 0.3rem;
            color: var(--text-dark);
            transition: var(--transition);
            font-weight: 700;
        }
        .section-title .accent {
            color: var(--primary);
            position: relative;
        }
        .section-title .accent::after {
            content: '';
            position: absolute;
            bottom: 2px;
            left: 0;
            width: 100%;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), var(--primary-light), var(--accent));
            border-radius: 10px;
            opacity: 0.2;
        }
        .section-subtitle {
            text-align: center;
            color: #7a4a7a;
            font-weight: 300;
            margin-bottom: 3.5rem;
            font-size: 1.15rem;
            transition: var(--transition);
            letter-spacing: 0.5px;
        }
        body.dark-mode .section-subtitle {
            color: #c9a8c9;
        }
        @media (max-width: 750px) {
            .section {
                padding: 2.5rem 1.5rem;
            }
            .section-title {
                font-size: 2.2rem;
            }
        }
        @media (max-width: 480px) {
            .section-title {
                font-size: 1.8rem;
            }
            .section-subtitle {
                font-size: 0.95rem;
            }
        }

        /* ============================================
           CATEGORÍAS
           ============================================ */
        .category-pills {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 0.8rem;
            margin-bottom: 2.5rem;
        }
        .category-pills .pill {
            padding: 0.7rem 2.2rem;
            border-radius: 50px;
            background: #fff;
            border: 1.5px solid rgba(214, 51, 132, 0.06);
            font-weight: 600;
            font-size: 0.9rem;
            color: var(--text-dark);
            cursor: pointer;
            transition: var(--transition);
            font-family: var(--font-sans);
        }
        .category-pills .pill:hover {
            transform: translateY(-4px);
            box-shadow: 0 4px 20px rgba(194, 24, 91, 0.06);
        }
        .category-pills .pill.active {
            background: linear-gradient(135deg, var(--primary), var(--primary-light));
            color: #fff;
            border-color: transparent;
            box-shadow: 0 4px 30px rgba(194, 24, 91, 0.2);
        }

        /* ============================================
           FILTRO PRECIO
           ============================================ */
        .price-filter {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 1rem;
            flex-wrap: wrap;
            margin-bottom: 2rem;
            padding: 1.2rem 2rem;
            background: rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(12px);
            border-radius: var(--radius-sm);
            border: 1px solid rgba(255, 182, 193, 0.04);
        }
        body.dark-mode .price-filter {
            background: rgba(255, 255, 255, 0.02);
            border-color: rgba(255, 182, 193, 0.02);
        }
        .price-filter label {
            font-weight: 600;
            color: var(--text-dark);
        }
        body.dark-mode .price-filter label {
            color: #f0e8f0;
        }
        .price-filter input {
            width: 120px;
            padding: 0.5rem 1.2rem;
            border: 1.5px solid rgba(214, 51, 132, 0.06);
            border-radius: 12px;
            font-family: var(--font-sans);
            font-size: 0.9rem;
            background: #fff;
            transition: var(--transition);
            font-weight: 500;
        }
        body.dark-mode .price-filter input {
            background: #0a050a;
            color: #f0e8f0;
            border-color: rgba(255, 182, 193, 0.03);
        }
        .price-filter input:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 5px rgba(194, 24, 91, 0.04);
        }
        .price-filter .btn-primary {
            padding: 0.5rem 2rem;
            font-size: 0.9rem;
        }
        .price-filter .btn-secondary {
            padding: 0.5rem 2rem;
            font-size: 0.9rem;
            margin: 0;
        }

        /* ============================================
           ORDENAR
           ============================================ */
        .sort-options {
            display: flex;
            align-items: center;
            justify-content: flex-end;
            gap: 0.8rem;
            margin-bottom: 1.5rem;
        }
        .sort-options label {
            font-weight: 500;
            color: var(--text-dark);
        }
        body.dark-mode .sort-options label {
            color: #f0e8f0;
        }
        .sort-options select {
            padding: 0.5rem 2rem;
            border: 1.5px solid rgba(214, 51, 132, 0.06);
            border-radius: 12px;
            font-family: var(--font-sans);
            font-size: 0.9rem;
            background: #fff;
            cursor: pointer;
            transition: var(--transition);
            font-weight: 500;
            appearance: none;
            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='12' viewBox='0 0 12 12'%3E%3Cpath fill='%23c2185b' d='M6 8L1 3h10z'/%3E%3C/svg%3E");
            background-repeat: no-repeat;
            background-position: right 1rem center;
            padding-right: 2.8rem;
        }
        body.dark-mode .sort-options select {
            background: #0a050a;
            color: #f0e8f0;
            border-color: rgba(255, 182, 193, 0.03);
            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='12' viewBox='0 0 12 12'%3E%3Cpath fill='%23f06292' d='M6 8L1 3h10z'/%3E%3C/svg%3E");
        }
        .sort-options select:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 5px rgba(194, 24, 91, 0.04);
        }
        @media (max-width: 480px) {
            .sort-options {
                justify-content: center;
            }
        }

        /* ============================================
           PRODUCTOS
           ============================================ */
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2.5rem;
        }
        .product-card {
            background: #ffffff;
            border-radius: var(--radius);
            padding: 2.2rem 1.5rem 2rem;
            text-align: center;
            box-shadow: var(--shadow);
            transition: var(--transition);
            border: 1px solid rgba(255, 182, 193, 0.04);
            position: relative;
            animation: fadeInUp 0.7s ease forwards;
        }
        .product-card:nth-child(1) {
            animation-delay: 0.05s;
        }
        .product-card:nth-child(2) {
            animation-delay: 0.1s;
        }
        .product-card:nth-child(3) {
            animation-delay: 0.15s;
        }
        .product-card:nth-child(4) {
            animation-delay: 0.2s;
        }
        .product-card:nth-child(5) {
            animation-delay: 0.25s;
        }
        .product-card:nth-child(6) {
            animation-delay: 0.3s;
        }
        .product-card:nth-child(7) {
            animation-delay: 0.35s;
        }
        .product-card:nth-child(8) {
            animation-delay: 0.4s;
        }
        .product-card:nth-child(9) {
            animation-delay: 0.45s;
        }
        .product-card:nth-child(10) {
            animation-delay: 0.5s;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(50px) scale(0.95);
            }
            to {
                opacity: 1;
                transform: translateY(0) scale(1);
            }
        }
        .product-card:hover {
            transform: translateY(-18px) scale(1.02);
            box-shadow: var(--shadow-hover);
            border-color: rgba(194, 24, 91, 0.08);
        }
        .product-card .product-img {
            font-size: 5rem;
            display: block;
            background: linear-gradient(135deg, #fce4ec, #f8e8f0);
            border-radius: 50%;
            width: 110px;
            height: 110px;
            line-height: 110px;
            margin: 0 auto 0.8rem;
            box-shadow: 0 4px 25px rgba(200, 120, 180, 0.06);
            overflow: hidden;
            cursor: pointer;
            transition: var(--transition);
            position: relative;
        }
        .product-card .product-img::after {
            content: '🔍';
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%) scale(0);
            font-size: 2.2rem;
            background: rgba(0, 0, 0, 0.3);
            backdrop-filter: blur(4px);
            border-radius: 50%;
            width: 55px;
            height: 55px;
            line-height: 55px;
            transition: var(--transition);
        }
        .product-card .product-img:hover::after {
            transform: translate(-50%, -50%) scale(1);
        }
        .product-card .product-img:hover {
            transform: scale(1.06);
            box-shadow: 0 8px 35px rgba(194, 24, 91, 0.08);
        }
        .product-card .product-img img {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            object-fit: cover;
        }
        .product-card .badge {
            position: absolute;
            top: 18px;
            right: 18px;
            background: linear-gradient(135deg, var(--primary-light), var(--primary));
            color: #fff;
            font-size: 0.65rem;
            font-weight: 700;
            padding: 0.2rem 1.4rem;
            border-radius: 50px;
            text-transform: uppercase;
            z-index: 1;
            letter-spacing: 0.5px;
            box-shadow: 0 4px 20px rgba(194, 24, 91, 0.15);
        }
        .product-card .badge.sale {
            background: linear-gradient(135deg, #ff6f00, #f9a825);
            box-shadow: 0 4px 20px rgba(249, 168, 37, 0.25);
        }
        .product-card .badge.stock {
            background: linear-gradient(135deg, #2e7d32, #43a047);
            box-shadow: 0 4px 20px rgba(46, 125, 50, 0.25);
            font-size: 0.55rem;
        }
        .product-card .badge.discount {
            background: linear-gradient(135deg, #e53935, #ef5350);
            box-shadow: 0 4px 20px rgba(229, 57, 53, 0.25);
            font-size: 0.7rem;
            top: 70px;
            right: 18px;
        }
        .product-card .badge.hot {
            background: linear-gradient(135deg, #d32f2f, #e53935);
            animation: pulseBadge 1.5s infinite;
            box-shadow: 0 4px 25px rgba(211, 47, 47, 0.3);
        }
        @keyframes pulseBadge {
            0%,
            100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.08);
            }
        }
        .product-card .badge.new {
            background: linear-gradient(135deg, #1565c0, #1e88e5);
            box-shadow: 0 4px 20px rgba(21, 101, 192, 0.25);
        }
        .product-card .badge.premium {
            background: linear-gradient(135deg, #6a1b4d, #9c27b0);
            box-shadow: 0 4px 20px rgba(156, 39, 176, 0.25);
        }
        .product-card .buyers-count {
            font-size: 0.8rem;
            color: #2e7d32;
            font-weight: 600;
            margin-top: -0.2rem;
            margin-bottom: 0.3rem;
        }
        body.dark-mode .product-card .buyers-count {
            color: #66bb6a;
        }
        .product-card .seen-time {
            font-size: 0.7rem;
            color: #aaa;
            margin-bottom: 0.3rem;
            font-weight: 400;
        }
        body.dark-mode .product-card .seen-time {
            color: #7a4a7a;
        }
        .product-card h3 {
            font-family: var(--font-serif);
            font-size: 1.3rem;
            color: var(--text-dark);
            margin-bottom: 0.2rem;
            transition: var(--transition);
        }
        body.dark-mode .product-card h3 {
            color: #f0e8f0;
        }
        .product-card .desc {
            font-size: 0.85rem;
            color: #7a4a7a;
            font-weight: 300;
            margin-bottom: 0.6rem;
            transition: var(--transition);
        }
        body.dark-mode .product-card .desc {
            color: #c9a8c9;
        }
        .product-card .price {
            font-size: 1.8rem;
            font-weight: 800;
            color: var(--primary);
            margin-bottom: 1rem;
            display: block;
            font-family: var(--font-serif);
        }
        body.dark-mode .product-card .price {
            color: var(--primary-light);
        }
        .product-card .price .old {
            font-size: 1rem;
            color: #aaa;
            text-decoration: line-through;
            font-weight: 400;
            margin-left: 0.5rem;
        }
        .product-card .price .discount-percent {
            font-size: 0.85rem;
            color: #e53935;
            font-weight: 700;
            margin-left: 0.5rem;
            background: rgba(229, 57, 53, 0.06);
            padding: 0.1rem 0.8rem;
            border-radius: 20px;
        }
        .product-card .stock-info {
            font-size: 0.75rem;
            color: #2e7d32;
            margin-bottom: 0.5rem;
            font-weight: 600;
        }
        body.dark-mode .product-card .stock-info {
            color: #66bb6a;
        }
        .product-card .stock-info.low {
            color: #e53935;
            animation: pulseBadge 1.5s infinite;
        }
        body.dark-mode .product-card .stock-info.low {
            color: #ef5350;
        }
        .btn-add {
            background: linear-gradient(135deg, #fce4ec, #f8e8f0);
            border: none;
            padding: 0.8rem 2.8rem;
            border-radius: 50px;
            font-weight: 700;
            color: var(--secondary);
            cursor: pointer;
            transition: var(--transition);
            font-size: 0.9rem;
            border: 1.5px solid rgba(194, 24, 91, 0.04);
            font-family: var(--font-sans);
        }
        body.dark-mode .btn-add {
            background: rgba(255, 255, 255, 0.03);
            color: #f0e8f0;
            border-color: rgba(255, 182, 193, 0.03);
        }
        .btn-add:hover {
            background: linear-gradient(135deg, var(--primary), var(--primary-light));
            color: #fff;
            box-shadow: 0 8px 35px rgba(194, 24, 91, 0.2);
            transform: translateY(-4px);
        }
        .btn-add:disabled {
            opacity: 0.4;
            cursor: not-allowed;
            transform: none !important;
        }

        @media (max-width: 750px) {
            .product-card .product-img {
                width: 90px;
                height: 90px;
                line-height: 90px;
                font-size: 4rem;
            }
            .product-grid {
                gap: 1.5rem;
                grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
            }
        }
        @media (max-width: 480px) {
            .product-card {
                padding: 1.2rem 0.8rem;
            }
            .product-card .product-img {
                width: 75px;
                height: 75px;
                line-height: 75px;
                font-size: 3.2rem;
            }
            .product-card .price {
                font-size: 1.4rem;
            }
            .product-card h3 {
                font-size: 1.1rem;
            }
        }

        /* ============================================
           CARRUSEL
           ============================================ */
        .featured-carousel {
            position: relative;
            overflow: hidden;
            margin: 0 -1rem;
            padding: 0 1rem;
        }
        .featured-carousel .carousel-track {
            display: flex;
            gap: 1.8rem;
            transition: transform 0.6s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }
        .featured-carousel .carousel-track .product-card {
            min-width: 280px;
            flex-shrink: 0;
        }
        .carousel-btn {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            background: rgba(255, 255, 255, 0.85);
            backdrop-filter: blur(15px);
            border: none;
            font-size: 2.5rem;
            padding: 0.6rem 1.4rem;
            border-radius: 50%;
            cursor: pointer;
            transition: var(--transition);
            color: var(--primary);
            box-shadow: 0 4px 25px rgba(0, 0, 0, 0.04);
            z-index: 2;
        }
        .carousel-btn:hover {
            background: var(--primary);
            color: #fff;
            transform: translateY(-50%) scale(1.08);
        }
        .carousel-btn.prev {
            left: 0.5rem;
        }
        .carousel-btn.next {
            right: 0.5rem;
        }
        body.dark-mode .carousel-btn {
            background: rgba(26, 11, 26, 0.85);
            color: #f0e8f0;
        }
        body.dark-mode .carousel-btn:hover {
            background: var(--primary);
            color: #fff;
        }
        @media (max-width: 600px) {
            .featured-carousel .carousel-track .product-card {
                min-width: 210px;
            }
            .carousel-btn {
                font-size: 1.8rem;
                padding: 0.3rem 0.9rem;
            }
        }

        /* ============================================
           SLIDER
           ============================================ */
        .slider-container {
            position: relative;
            max-width: 1000px;
            margin: 0 auto 2.5rem;
            border-radius: var(--radius);
            overflow: hidden;
            box-shadow: 0 10px 60px rgba(200, 120, 180, 0.06);
        }
        .slider {
            display: flex;
            transition: transform 0.7s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }
        .slider-slide {
            min-width: 100%;
            height: 480px;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            background-size: cover;
            background-position: center;
        }
        .slider-slide .slide-text {
            position: absolute;
            bottom: 2.5rem;
            left: 50%;
            transform: translateX(-50%);
            background: rgba(0, 0, 0, 0.4);
            backdrop-filter: blur(15px);
            color: #fff;
            padding: 0.6rem 3rem;
            border-radius: 50px;
            font-weight: 600;
            font-size: 1.1rem;
            letter-spacing: 1px;
        }
        .slider-slide .slide-emoji {
            font-size: 10rem;
            filter: drop-shadow(0 10px 40px rgba(0, 0, 0, 0.05));
        }
        .slider-btn {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            background: rgba(255, 255, 255, 0.85);
            backdrop-filter: blur(15px);
            border: none;
            font-size: 2.5rem;
            padding: 0.6rem 1.4rem;
            border-radius: 50%;
            cursor: pointer;
            transition: var(--transition);
            color: var(--primary);
            box-shadow: 0 4px 25px rgba(0, 0, 0, 0.04);
        }
        .slider-btn:hover {
            background: var(--primary);
            color: #fff;
            transform: translateY(-50%) scale(1.08);
        }
        .slider-btn.prev {
            left: 1.2rem;
        }
        .slider-btn.next {
            right: 1.2rem;
        }
        .slider-dots {
            display: flex;
            justify-content: center;
            gap: 0.6rem;
            margin-top: 1.2rem;
        }
        .slider-dots .dot {
            width: 16px;
            height: 16px;
            border-radius: 50%;
            background: #ddd;
            cursor: pointer;
            transition: var(--transition);
            border: none;
        }
        .slider-dots .dot.active {
            background: var(--primary);
            transform: scale(1.2);
            box-shadow: 0 4px 20px rgba(194, 24, 91, 0.15);
        }
        body.dark-mode .slider-dots .dot {
            background: #3d2b3e;
        }
        @media (max-width: 750px) {
            .slider-slide {
                height: 320px;
            }
            .slider-slide .slide-emoji {
                font-size: 7rem !important;
            }
            .slider-slide .slide-text {
                font-size: 0.9rem;
                padding: 0.4rem 1.8rem;
            }
            .slider-btn {
                font-size: 1.8rem;
                padding: 0.4rem 1rem;
            }
        }
        @media (max-width: 480px) {
            .slider-slide {
                height: 240px;
            }
            .slider-slide .slide-emoji {
                font-size: 5rem !important;
            }
            .slider-slide .slide-text {
                font-size: 0.7rem;
                padding: 0.3rem 1.2rem;
                bottom: 1.5rem;
            }
        }

        /* ============================================
           OFERTA RELÁMPAGO
           ============================================ */
        .flash-sale {
            background: linear-gradient(135deg, #d32f2f, #e53935, #c2185b, #880e4f, #6a1b4d);
            background-size: 400% 400%;
            animation: flashGradient 5s ease infinite;
            border-radius: var(--radius);
            padding: 3.5rem 4rem;
            margin: 2rem auto;
            text-align: center;
            color: #fff;
            position: relative;
            overflow: hidden;
            box-shadow: 0 10px 50px rgba(211, 47, 47, 0.25);
        }
        @keyframes flashGradient {
            0%,
            100% {
                background-position: 0% 50%;
            }
            25% {
                background-position: 50% 0%;
            }
            50% {
                background-position: 100% 50%;
            }
            75% {
                background-position: 50% 100%;
            }
        }
        .flash-sale::before {
            content: '⚡';
            font-size: 15rem;
            position: absolute;
            right: -3rem;
            bottom: -5rem;
            opacity: 0.04;
            animation: floatFlash 4s ease-in-out infinite;
        }
        @keyframes floatFlash {
            0%,
            100% {
                transform: translateY(0) rotate(-10deg) scale(1);
            }
            50% {
                transform: translateY(-20px) rotate(10deg) scale(1.05);
            }
        }
        .flash-sale h2 {
            font-family: var(--font-serif);
            font-size: 2.8rem;
            margin-bottom: 0.3rem;
            text-shadow: 0 2px 30px rgba(0, 0, 0, 0.1);
            position: relative;
            z-index: 1;
        }
        .flash-sale p {
            opacity: 0.9;
            margin-bottom: 1.5rem;
            font-size: 1.15rem;
            position: relative;
            z-index: 1;
        }
        .flash-sale .flash-timer {
            display: flex;
            gap: 1.2rem;
            justify-content: center;
            font-size: 2.8rem;
            font-weight: 700;
            margin-bottom: 1.5rem;
            font-family: var(--font-serif);
            position: relative;
            z-index: 1;
        }
        .flash-sale .flash-timer .time-block {
            background: rgba(255, 255, 255, 0.08);
            backdrop-filter: blur(15px);
            padding: 0.4rem 1.8rem;
            border-radius: var(--radius-sm);
            min-width: 90px;
            border: 1px solid rgba(255, 255, 255, 0.04);
        }
        .flash-sale .flash-timer .time-label {
            font-size: 0.65rem;
            text-transform: uppercase;
            opacity: 0.6;
            display: block;
            font-weight: 400;
            letter-spacing: 2px;
        }
        .flash-sale .flash-product {
            background: rgba(255, 255, 255, 0.06);
            backdrop-filter: blur(10px);
            border-radius: var(--radius-sm);
            padding: 1.8rem;
            max-width: 340px;
            margin: 0 auto;
            border: 1px solid rgba(255, 255, 255, 0.04);
            position: relative;
            z-index: 1;
        }
        .flash-sale .flash-product .flash-emoji {
            font-size: 5rem;
            display: block;
        }
        .flash-sale .flash-product h3 {
            font-family: var(--font-serif);
            font-size: 1.5rem;
            margin: 0.2rem 0;
        }
        .flash-sale .flash-product .flash-price {
            font-size: 2.2rem;
            font-weight: 800;
        }
        .flash-sale .flash-product .flash-price .old {
            font-size: 1.2rem;
            text-decoration: line-through;
            opacity: 0.4;
            margin-left: 0.5rem;
        }
        @media (max-width: 750px) {
            .flash-sale {
                padding: 2rem 1.5rem;
                border-radius: var(--radius-sm);
            }
            .flash-sale .flash-timer {
                font-size: 2rem;
                gap: 0.8rem;
            }
            .flash-sale .flash-timer .time-block {
                min-width: 65px;
                padding: 0.3rem 1.2rem;
            }
            .flash-sale h2 {
                font-size: 2rem;
            }
        }
        @media (max-width: 480px) {
            .flash-sale .flash-timer {
                font-size: 1.4rem;
                gap: 0.5rem;
            }
            .flash-sale .flash-timer .time-block {
                min-width: 50px;
                padding: 0.2rem 0.8rem;
            }
            .flash-sale .flash-product .flash-price {
                font-size: 1.6rem;
            }
            .flash-sale h2 {
                font-size: 1.6rem;
            }
        }

        /* ============================================
           NOTIFICACIONES EN VIVO
           ============================================ */
        .live-notification {
            position: fixed;
            bottom: 90px;
            left: 2rem;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            padding: 0.8rem 2rem;
            border-radius: var(--radius-sm);
            box-shadow: 0 8px 50px rgba(0, 0, 0, 0.06);
            border-left: 4px solid #25D366;
            z-index: 998;
            transform: translateX(-120%);
            transition: transform 0.6s cubic-bezier(0.34, 1.56, 0.64, 1);
            max-width: 340px;
            font-size: 0.9rem;
        }
        body.dark-mode .live-notification {
            background: rgba(26, 11, 26, 0.95);
            color: #f0e8f0;
        }
        .live-notification.show {
            transform: translateX(0);
        }
        .live-notification .ln-name {
            font-weight: 700;
            color: var(--primary);
        }
        body.dark-mode .live-notification .ln-name {
            color: var(--primary-light);
        }
        .live-notification .ln-product {
            font-weight: 600;
        }
        .live-notification .ln-time {
            font-size: 0.7rem;
            color: #aaa;
            display: block;
            margin-top: 0.2rem;
        }
        body.dark-mode .live-notification .ln-time {
            color: #7a4a7a;
        }
        .live-notification .ln-emoji {
            margin-right: 0.3rem;
        }
        @media (max-width: 750px) {
            .live-notification {
                left: 1rem;
                right: 1rem;
                max-width: none;
                bottom: 80px;
                padding: 0.6rem 1.2rem;
                font-size: 0.8rem;
            }
        }

        /* ============================================
           CONFETTI
           ============================================ */
        .confetti-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 9999;
            overflow: hidden;
        }
        .confetti {
            position: absolute;
            width: 14px;
            height: 14px;
            border-radius: 2px;
            animation: confettiFall linear forwards;
        }
        .confetti.circle {
            border-radius: 50%;
        }
        .confetti.star {
            clip-path: polygon(50% 0%, 61% 35%, 98% 35%, 68% 57%, 79% 91%, 50% 70%, 21% 91%, 32% 57%, 2% 35%, 39% 35%);
            border-radius: 0;
        }
        .confetti.heart {
            clip-path: path(
                "M50 90 C30 70 0 50 0 30 C0 10 20 0 35 15 L50 30 L65 15 C80 0 100 10 100 30 C100 50 70 70 50 90Z"
            );
            border-radius: 0;
        }
        @keyframes confettiFall {
            0% {
                transform: translateY(-20px) rotate(0deg) scale(0);
                opacity: 1;
            }
            100% {
                transform: translateY(110vh) rotate(720deg) scale(1);
                opacity: 0;
            }
        }

        /* ============================================
           LIGHTBOX
           ============================================ */
        .lightbox {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.92);
            backdrop-filter: blur(30px);
            z-index: 6000;
            align-items: center;
            justify-content: center;
            cursor: pointer;
        }
        .lightbox.show {
            display: flex;
            animation: fadeInLightbox 0.5s ease;
        }
        @keyframes fadeInLightbox {
            from {
                opacity: 0;
                transform: scale(0.9);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }
        .lightbox .lightbox-content {
            font-size: 14rem;
            text-align: center;
            animation: zoomIn 0.5s ease;
            cursor: default;
            position: relative;
        }
        .lightbox .lightbox-content .lb-emoji {
            display: block;
            filter: drop-shadow(0 30px 80px rgba(0, 0, 0, 0.2));
        }
        .lightbox .lightbox-content .lb-name {
            font-family: var(--font-serif);
            color: #fff;
            font-size: 1.8rem;
            margin-top: 1rem;
            letter-spacing: 2px;
        }
        .lightbox .lightbox-content .lb-price {
            color: var(--primary-light);
            font-size: 1.4rem;
            font-weight: 700;
            margin-top: 0.3rem;
        }
        .lightbox .lightbox-content img {
            max-width: 80%;
            max-height: 80vh;
            border-radius: 20px;
            box-shadow: 0 30px 100px rgba(0, 0, 0, 0.4);
        }
        .lightbox .lightbox-close {
            position: absolute;
            top: 2.5rem;
            right: 4rem;
            font-size: 4rem;
            color: #fff;
            cursor: pointer;
            transition: var(--transition);
            opacity: 0.5;
        }
        .lightbox .lightbox-close:hover {
            opacity: 1;
            transform: rotate(90deg) scale(1.1);
        }
        @keyframes zoomIn {
            from {
                transform: scale(0.6) rotate(-5deg);
                opacity: 0;
            }
            to {
                transform: scale(1) rotate(0deg);
                opacity: 1;
            }
        }
        @media (max-width: 750px) {
            .lightbox .lightbox-content {
                font-size: 8rem;
            }
            .lightbox .lightbox-close {
                top: 1.5rem;
                right: 2rem;
                font-size: 3rem;
            }
            .lightbox .lightbox-content .lb-name {
                font-size: 1.2rem;
            }
        }
        @media (max-width: 480px) {
            .lightbox .lightbox-content {
                font-size: 6rem;
            }
            .lightbox .lightbox-close {
                top: 1rem;
                right: 1.5rem;
                font-size: 2.5rem;
            }
        }

        /* ============================================
           FAQ
           ============================================ */
        .faq-grid {
            max-width: 800px;
            margin: 0 auto;
        }
        .faq-item {
            background: #fff;
            border-radius: var(--radius-sm);
            padding: 1.2rem 2rem;
            margin-bottom: 0.8rem;
            border: 1px solid rgba(255, 182, 193, 0.04);
            cursor: pointer;
            transition: var(--transition);
            box-shadow: 0 2px 15px rgba(0, 0, 0, 0.01);
        }
        body.dark-mode .faq-item {
            background: #1a0b1a;
            border-color: rgba(255, 182, 193, 0.02);
        }
        .faq-item:hover {
            border-color: rgba(194, 24, 91, 0.08);
            transform: translateX(5px);
            box-shadow: 0 4px 25px rgba(0, 0, 0, 0.02);
        }
        .faq-item .faq-question {
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-weight: 700;
            font-size: 1.05rem;
        }
        .faq-item .faq-question .icon {
            transition: var(--transition);
            font-size: 1.4rem;
            color: var(--primary);
        }
        .faq-item.open .faq-question .icon {
            transform: rotate(180deg);
        }
        .faq-item .faq-answer {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.4s ease, padding 0.4s ease;
            color: #7a4a7a;
            font-weight: 400;
            line-height: 1.8;
        }
        body.dark-mode .faq-item .faq-answer {
            color: #c9a8c9;
        }
        .faq-item.open .faq-answer {
            max-height: 300px;
            padding-top: 0.8rem;
        }

        /* ============================================
           CARRITO FLOTANTE
           ============================================ */
        .floating-cart {
            position: fixed;
            bottom: 150px;
            right: 2rem;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-radius: 50px;
            padding: 0.8rem 1.8rem;
            box-shadow: 0 8px 50px rgba(0, 0, 0, 0.06);
            border: 1px solid rgba(255, 182, 193, 0.04);
            z-index: 998;
            display: flex;
            align-items: center;
            gap: 0.8rem;
            cursor: pointer;
            transition: var(--transition);
            font-weight: 600;
            font-size: 0.95rem;
        }
        body.dark-mode .floating-cart {
            background: rgba(26, 11, 26, 0.95);
            border-color: rgba(255, 182, 193, 0.02);
            color: #f0e8f0;
        }
        .floating-cart:hover {
            transform: scale(1.06) translateY(-4px);
            box-shadow: 0 12px 60px rgba(0, 0, 0, 0.06);
        }
        .floating-cart .fc-icon {
            font-size: 1.8rem;
        }
        .floating-cart .fc-count {
            background: linear-gradient(135deg, var(--primary), var(--primary-light));
            color: #fff;
            border-radius: 50%;
            padding: 0.05rem 0.5rem;
            font-size: 0.7rem;
            font-weight: 700;
            min-width: 24px;
            text-align: center;
        }
        .floating-cart .fc-total {
            color: var(--primary);
            font-weight: 800;
        }
        body.dark-mode .floating-cart .fc-total {
            color: var(--primary-light);
        }
        @media (max-width: 750px) {
            .floating-cart {
                bottom: 130px;
                right: 1rem;
                padding: 0.4rem 1.2rem;
                font-size: 0.8rem;
            }
            .floating-cart .fc-icon {
                font-size: 1.4rem;
            }
        }
        @media (max-width: 480px) {
            .floating-cart {
                bottom: 110px;
                right: 0.8rem;
                padding: 0.3rem 0.8rem;
                font-size: 0.7rem;
                gap: 0.4rem;
            }
            .floating-cart .fc-icon {
                font-size: 1.2rem;
            }
        }

        /* ============================================
           BANNER
           ============================================ */
        .banner {
            background: linear-gradient(135deg, #fce4ec, #f3e5f5, #e8eaf6);
            border-radius: var(--radius);
            padding: 4.5rem 4rem;
            margin: 2rem auto;
            text-align: center;
            border: 1px solid rgba(255, 182, 193, 0.04);
            position: relative;
            overflow: hidden;
            transition: var(--transition);
            box-shadow: 0 4px 40px rgba(200, 120, 180, 0.03);
        }
        body.dark-mode .banner {
            background: linear-gradient(135deg, #1a0b1a, #0a050a);
            border-color: rgba(255, 182, 193, 0.02);
        }
        .banner::before {
            content: '💎';
            font-size: 12rem;
            position: absolute;
            right: -3rem;
            bottom: -4rem;
            opacity: 0.03;
            animation: floatBanner 5s ease-in-out infinite;
        }
        @keyframes floatBanner {
            0%,
            100% {
                transform: translateY(0) rotate(-5deg) scale(1);
            }
            50% {
                transform: translateY(-20px) rotate(5deg) scale(1.03);
            }
        }
        .banner h2 {
            font-family: var(--font-serif);
            font-size: 2.8rem;
            color: var(--text-dark);
            transition: var(--transition);
        }
        body.dark-mode .banner h2 {
            color: #f0e8f0;
        }
        .banner h2 .highlight {
            color: var(--primary);
            position: relative;
        }
        body.dark-mode .banner h2 .highlight {
            color: var(--primary-light);
        }
        .banner h2 .highlight::after {
            content: '';
            position: absolute;
            bottom: 2px;
            left: 0;
            width: 100%;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), var(--primary-light), var(--accent));
            border-radius: 10px;
            opacity: 0.2;
        }
        .banner p {
            font-size: 1.15rem;
            color: #4a2c4a;
            max-width: 580px;
            margin: 0.5rem auto 1.5rem;
            transition: var(--transition);
        }
        body.dark-mode .banner p {
            color: #c9a8c9;
        }
        .timer {
            display: flex;
            gap: 1.2rem;
            justify-content: center;
            font-size: 3rem;
            font-weight: 700;
            color: var(--primary);
            margin: 1rem 0 1.5rem;
            font-family: var(--font-serif);
            flex-wrap: wrap;
        }
        body.dark-mode .timer {
            color: var(--primary-light);
        }
        .timer .time-block {
            background: rgba(255, 255, 255, 0.4);
            backdrop-filter: blur(15px);
            padding: 0.4rem 1.8rem;
            border-radius: var(--radius-sm);
            min-width: 90px;
            border: 1px solid rgba(194, 24, 91, 0.04);
            transition: var(--transition);
        }
        body.dark-mode .timer .time-block {
            background: rgba(26, 11, 26, 0.4);
            border-color: rgba(255, 182, 193, 0.02);
        }
        .timer .time-label {
            font-size: 0.65rem;
            text-transform: uppercase;
            color: #7a4a7a;
            display: block;
            font-weight: 400;
            letter-spacing: 2px;
        }
        body.dark-mode .timer .time-label {
            color: #9a7a9a;
        }
        @media (max-width: 750px) {
            .banner {
                padding: 2.5rem 1.5rem;
                border-radius: var(--radius-sm);
            }
            .banner h2 {
                font-size: 2rem;
            }
            .timer {
                font-size: 2.2rem;
                gap: 0.8rem;
            }
            .timer .time-block {
                min-width: 65px;
                padding: 0.3rem 1.2rem;
            }
        }
        @media (max-width: 480px) {
            .banner h2 {
                font-size: 1.5rem;
            }
            .banner p {
                font-size: 0.95rem;
            }
            .timer {
                font-size: 1.6rem;
            }
            .timer .time-block {
                min-width: 50px;
                padding: 0.2rem 0.8rem;
            }
        }

        /* ============================================
           TESTIMONIOS
           ============================================ */
        .testimonials {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 1rem;
        }
        .testimonial {
            background: #fff;
            border-radius: var(--radius);
            padding: 2.2rem 2rem;
            box-shadow: 0 4px 30px rgba(0, 0, 0, 0.01);
            border: 1px solid rgba(255, 182, 193, 0.04);
            transition: var(--transition);
            position: relative;
        }
        body.dark-mode .testimonial {
            background: #1a0b1a;
            border-color: rgba(255, 182, 193, 0.02);
        }
        .testimonial::before {
            content: '"';
            font-family: var(--font-serif);
            font-size: 5rem;
            position: absolute;
            top: -0.8rem;
            left: 0.5rem;
            color: rgba(194, 24, 91, 0.04);
        }
        .testimonial:hover {
            border-color: rgba(194, 24, 91, 0.06);
            transform: translateY(-8px);
            box-shadow: 0 8px 50px rgba(0, 0, 0, 0.02);
        }
        .testimonial .stars {
            color: #f9a825;
            font-size: 1.2rem;
            letter-spacing: 4px;
        }
        .testimonial p {
            font-style: italic;
            color: #4a2c4a;
            font-size: 0.95rem;
            margin: 0.5rem 0;
            transition: var(--transition);
        }
        body.dark-mode .testimonial p {
            color: #c9a8c9;
        }
        .testimonial .name {
            font-weight: 700;
            color: var(--primary);
        }
        body.dark-mode .testimonial .name {
            color: var(--primary-light);
        }
        .testimonial .date {
            font-size: 0.75rem;
            color: #aaa;
        }
        body.dark-mode .testimonial .date {
            color: #7a4a7a;
        }

        /* ============================================
           TIPS
           ============================================ */
        .tips-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(270px, 1fr));
            gap: 2rem;
        }
        .tip-card {
            background: #fff;
            border-radius: var(--radius);
            padding: 2.2rem 2rem;
            box-shadow: 0 4px 30px rgba(0, 0, 0, 0.01);
            border: 1px solid rgba(255, 182, 193, 0.04);
            text-align: center;
            transition: var(--transition);
        }
        body.dark-mode .tip-card {
            background: #1a0b1a;
            border-color: rgba(255, 182, 193, 0.02);
        }
        .tip-card:hover {
            transform: translateY(-8px);
            border-color: rgba(194, 24, 91, 0.06);
            box-shadow: 0 8px 50px rgba(0, 0, 0, 0.02);
        }
        .tip-card .tip-icon {
            font-size: 4.5rem;
            display: block;
            margin-bottom: 0.5rem;
        }
        .tip-card h3 {
            font-family: var(--font-serif);
            color: var(--text-dark);
            margin-bottom: 0.3rem;
            transition: var(--transition);
        }
        body.dark-mode .tip-card h3 {
            color: #f0e8f0;
        }
        .tip-card p {
            color: #7a4a7a;
            font-size: 0.95rem;
            transition: var(--transition);
        }
        body.dark-mode .tip-card p {
            color: #c9a8c9;
        }

        /* ============================================
           CONTACTO
           ============================================ */
        .contact-form {
            max-width: 680px;
            margin: 0 auto;
            background: #fff;
            padding: 3.5rem;
            border-radius: var(--radius);
            box-shadow: 0 8px 50px rgba(200, 120, 180, 0.02);
            border: 1px solid rgba(255, 182, 193, 0.04);
            transition: var(--transition);
        }
        body.dark-mode .contact-form {
            background: #1a0b1a;
            border-color: rgba(255, 182, 193, 0.02);
        }
        .contact-form .form-group {
            margin-bottom: 2rem;
        }
        .contact-form label {
            display: block;
            font-weight: 600;
            color: var(--text-dark);
            margin-bottom: 0.4rem;
            transition: var(--transition);
        }
        body.dark-mode .contact-form label {
            color: #f0e8f0;
        }
        .contact-form input,
        .contact-form textarea {
            width: 100%;
            padding: 1rem 1.8rem;
            border: 1.5px solid rgba(214, 51, 132, 0.04);
            border-radius: var(--radius-sm);
            font-family: var(--font-sans);
            font-size: 1rem;
            transition: var(--transition);
            background: var(--bg-light);
            font-weight: 400;
        }
        body.dark-mode .contact-form input,
        body.dark-mode .contact-form textarea {
            background: #0a050a;
            color: #f0e8f0;
            border-color: rgba(255, 182, 193, 0.02);
        }
        .contact-form input:focus,
        .contact-form textarea:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 6px rgba(194, 24, 91, 0.03);
        }
        .contact-form textarea {
            resize: vertical;
            min-height: 150px;
        }
        .contact-form .btn-primary {
            width: 100%;
            text-align: center;
        }

        /* ============================================
           NEWSLETTER
           ============================================ */
        .newsletter-section {
            background: linear-gradient(135deg, #fce4ec, #f8e8f0);
            border-radius: var(--radius);
            padding: 4rem 3.5rem;
            text-align: center;
            transition: var(--transition);
        }
        body.dark-mode .newsletter-section {
            background: linear-gradient(135deg, #1a0b1a, #0a050a);
        }
        .newsletter-form {
            max-width: 480px;
            margin: 0 auto;
            display: flex;
            gap: 0.8rem;
            flex-wrap: wrap;
            justify-content: center;
        }
        .newsletter-form input {
            flex: 1;
            min-width: 200px;
            padding: 1rem 1.8rem;
            border: 1.5px solid rgba(214, 51, 132, 0.04);
            border-radius: 50px;
            font-size: 1rem;
            background: #fff;
            font-family: var(--font-sans);
            transition: var(--transition);
        }
        body.dark-mode .newsletter-form input {
            background: #0a050a;
            color: #f0e8f0;
            border-color: rgba(255, 182, 193, 0.02);
        }
        .newsletter-form input:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 6px rgba(194, 24, 91, 0.03);
        }
        .newsletter-form .btn-primary {
            padding: 1rem 3rem;
        }

        /* ============================================
           MAPA
           ============================================ */
        .map-container {
            border-radius: var(--radius);
            overflow: hidden;
            box-shadow: 0 4px 40px rgba(0, 0, 0, 0.02);
        }
        .map-container iframe {
            width: 100%;
            height: 400px;
            border: 0;
        }
        .map-info {
            text-align: center;
            padding: 2.2rem;
            background: #fff;
            border-radius: var(--radius);
            box-shadow: 0 4px 40px rgba(0, 0, 0, 0.02);
            margin-top: 1.5rem;
            border: 1px solid rgba(255, 182, 193, 0.04);
            transition: var(--transition);
        }
        body.dark-mode .map-info {
            background: #1a0b1a;
            border-color: rgba(255, 182, 193, 0.02);
        }
        .map-info .map-icon {
            font-size: 4rem;
            display: block;
            margin-bottom: 0.5rem;
        }
        .map-info h3 {
            font-family: var(--font-serif);
            color: var(--text-dark);
            font-size: 1.5rem;
            transition: var(--transition);
        }
        body.dark-mode .map-info h3 {
            color: #f0e8f0;
        }
        .map-info p {
            color: #7a4a7a;
            margin-bottom: 1rem;
            transition: var(--transition);
        }
        body.dark-mode .map-info p {
            color: #c9a8c9;
        }
        .map-buttons {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
        }
        .map-buttons .btn-primary,
        .map-buttons .btn-secondary {
            padding: 0.8rem 2.5rem;
            display: inline-block;
            text-decoration: none;
        }

        /* ============================================
           FORMAS DE PAGO
           ============================================ */
        .payment-methods {
            display: flex;
            flex-wrap: wrap;
            gap: 1.5rem;
            justify-content: center;
            padding: 2.2rem;
            background: #fff;
            border-radius: var(--radius);
            border: 1px solid rgba(255, 182, 193, 0.04);
            margin-top: 1.5rem;
            transition: var(--transition);
        }
        body.dark-mode .payment-methods {
            background: #1a0b1a;
            border-color: rgba(255, 182, 193, 0.02);
        }
        .payment-methods .payment-item {
            text-align: center;
            padding: 0.8rem 1.8rem;
            background: rgba(214, 51, 132, 0.02);
            border-radius: var(--radius-sm);
            min-width: 100px;
            transition: var(--transition);
            border: 1px solid transparent;
        }
        .payment-methods .payment-item:hover {
            transform: translateY(-6px);
            border-color: rgba(194, 24, 91, 0.06);
            background: rgba(214, 51, 132, 0.04);
        }
        .payment-methods .payment-item .icon {
            font-size: 2.5rem;
            display: block;
        }
        .payment-methods .payment-item .name {
            font-size: 0.8rem;
            color: #7a4a7a;
            font-weight: 600;
        }
        body.dark-mode .payment-methods .payment-item .name {
            color: #c9a8c9;
        }

        /* ============================================
           REDES SOCIALES - VERSIÓN DEFINITIVA CON ÍCONOS VISIBLES
           ============================================ */
        .social-section {
            margin-top: 2.5rem;
            text-align: center;
            padding: 2rem;
            background: rgba(255, 255, 255, 0.4);
            border-radius: var(--radius);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: var(--transition);
        }
        body.dark-mode .social-section {
            background: rgba(255, 255, 255, 0.02);
            border-color: rgba(255, 182, 193, 0.02);
        }
        .social-section .social-title {
            color: #7a4a7a;
            margin-bottom: 1.2rem;
            font-weight: 700;
            font-size: 1.1rem;
            letter-spacing: 1px;
        }
        body.dark-mode .social-section .social-title {
            color: #c9a8c9;
        }

        .social-links {
            display: flex;
            gap: 1.2rem;
            justify-content: center;
            flex-wrap: wrap;
        }
        .social-links .social-link {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 0.3rem;
            padding: 0.8rem 1.5rem;
            border-radius: 16px;
            text-decoration: none;
            transition: var(--transition);
            color: #fff;
            min-width: 80px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.06);
        }
        .social-links .social-link .social-name {
            font-size: 0.7rem;
            font-weight: 600;
            opacity: 0.9;
        }
        .social-links .social-link:hover {
            transform: translateY(-8px) scale(1.05);
            box-shadow: 0 8px 35px rgba(0, 0, 0, 0.12);
        }
        .social-links .social-link svg {
            width: 30px;
            height: 30px;
            fill: #fff;
        }
        .social-links .social-link.instagram {
            background: linear-gradient(135deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888);
        }
        .social-links .social-link.tiktok {
            background: linear-gradient(135deg, #000000, #25f4ee, #fe2c55);
        }
        .social-links .social-link.facebook {
            background: #1877f2;
        }
        .social-links .social-link.whatsapp {
            background: #25D366;
        }
        .social-links .social-link.whatsapp:hover {
            background: #1da851;
        }

        @media (max-width: 480px) {
            .social-links .social-link {
                padding: 0.5rem 1rem;
                min-width: 60px;
            }
            .social-links .social-link svg {
                width: 24px;
                height: 24px;
            }
            .social-links .social-link .social-name {
                font-size: 0.6rem;
            }
            .social-section {
                padding: 1.5rem 1rem;
            }
        }

        /* ============================================
           CUPÓN
           ============================================ */
        .coupon-section {
            margin-top: 1.5rem;
            padding: 1.8rem;
            background: rgba(214, 51, 132, 0.02);
            border-radius: var(--radius-sm);
            border: 2px dashed var(--primary);
            text-align: center;
            max-width: 650px;
            margin-left: auto;
            margin-right: auto;
            transition: var(--transition);
        }
        body.dark-mode .coupon-section {
            background: rgba(255, 255, 255, 0.01);
            border-color: rgba(255, 182, 193, 0.04);
        }
        .coupon-section .coupon-code {
            font-size: 2.2rem;
            font-weight: 800;
            color: var(--primary);
            letter-spacing: 5px;
            font-family: var(--font-serif);
            background: rgba(194, 24, 91, 0.03);
            padding: 0.2rem 2rem;
            border-radius: 12px;
            display: inline-block;
        }
        body.dark-mode .coupon-section .coupon-code {
            color: var(--primary-light);
        }
        .coupon-section p {
            font-size: 0.95rem;
            color: #7a4a7a;
        }
        body.dark-mode .coupon-section p {
            color: #c9a8c9;
        }

        /* ============================================
           SELLO DE SEGURIDAD
           ============================================ */
        .security-badge {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 0.8rem;
            padding: 0.6rem 2.5rem;
            background: rgba(214, 51, 132, 0.02);
            border-radius: 50px;
            margin: 1rem auto;
            max-width: 500px;
            font-size: 0.9rem;
            color: var(--text-dark);
            border: 1px solid rgba(214, 51, 132, 0.02);
            transition: var(--transition);
        }
        body.dark-mode .security-badge {
            color: #f0e8f0;
            background: rgba(255, 255, 255, 0.01);
            border-color: rgba(255, 182, 193, 0.02);
        }
        .security-badge .shield {
            font-size: 2rem;
            animation: pulseShield 2.5s ease-in-out infinite;
        }
        @keyframes pulseShield {
            0%,
            100% {
                transform: scale(1) rotate(0deg);
            }
            50% {
                transform: scale(1.1) rotate(5deg);
            }
        }

        /* ============================================
           POP-UP
           ============================================ */
        .popup-overlay {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.75);
            backdrop-filter: blur(30px);
            z-index: 5000;
            align-items: center;
            justify-content: center;
            animation: fadeInPopup 0.5s ease;
        }
        .popup-overlay.show {
            display: flex;
        }
        @keyframes fadeInPopup {
            from {
                opacity: 0;
                transform: scale(0.9);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }
        .popup-content {
            background: #fff;
            border-radius: var(--radius);
            padding: 4rem 3.5rem;
            max-width: 500px;
            width: 90%;
            text-align: center;
            position: relative;
            box-shadow: 0 40px 100px rgba(0, 0, 0, 0.15);
            animation: slideUpPopup 0.6s ease;
        }
        @keyframes slideUpPopup {
            from {
                transform: translateY(80px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }
        body.dark-mode .popup-content {
            background: #1a0b1a;
        }
        .popup-content .popup-close {
            position: absolute;
            top: 1rem;
            right: 1.5rem;
            font-size: 2.2rem;
            cursor: pointer;
            color: #aaa;
            transition: var(--transition);
            background: none;
            border: none;
        }
        .popup-content .popup-close:hover {
            color: var(--primary);
            transform: rotate(90deg) scale(1.1);
        }
        .popup-content .popup-icon {
            font-size: 6rem;
            display: block;
            margin-bottom: 0.5rem;
        }
        .popup-content h2 {
            font-family: var(--font-serif);
            color: var(--text-dark);
            margin-bottom: 0.5rem;
            font-size: 2rem;
        }
        body.dark-mode .popup-content h2 {
            color: #f0e8f0;
        }
        .popup-content p {
            color: #7a4a7a;
            margin-bottom: 1.5rem;
        }
        body.dark-mode .popup-content p {
            color: #c9a8c9;
        }
        .popup-content .popup-timer {
            display: flex;
            gap: 0.8rem;
            justify-content: center;
            margin-bottom: 1.5rem;
        }
        .popup-content .popup-timer .time-block {
            background: #fce4ec;
            padding: 0.5rem 1.2rem;
            border-radius: 12px;
            min-width: 60px;
        }
        body.dark-mode .popup-content .popup-timer .time-block {
            background: #0a050a;
        }
        .popup-content .popup-timer .time-block span {
            font-size: 2.2rem;
            font-weight: 800;
            color: var(--primary);
            display: block;
            font-family: var(--font-serif);
        }
        body.dark-mode .popup-content .popup-timer .time-block span {
            color: var(--primary-light);
        }
        .popup-content .popup-timer .time-block .label {
            font-size: 0.6rem;
            text-transform: uppercase;
            color: #7a4a7a;
        }
        body.dark-mode .popup-content .popup-timer .time-block .label {
            color: #9a7a9a;
        }
        .popup-content .popup-input {
            display: flex;
            gap: 0.8rem;
            flex-wrap: wrap;
            justify-content: center;
        }
        .popup-content .popup-input input {
            flex: 1;
            min-width: 170px;
            padding: 1rem 1.8rem;
            border: 1.5px solid rgba(214, 51, 132, 0.04);
            border-radius: 50px;
            font-family: var(--font-sans);
            font-size: 1rem;
            background: var(--bg-light);
            transition: var(--transition);
        }
        body.dark-mode .popup-content .popup-input input {
            background: #0a050a;
            color: #f0e8f0;
            border-color: rgba(255, 182, 193, 0.02);
        }
        .popup-content .popup-input input:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 6px rgba(194, 24, 91, 0.03);
        }
        .popup-content .popup-input .btn-primary {
            padding: 1rem 3rem;
        }

        @media (max-width: 750px) {
            .popup-content {
                padding: 2.5rem 1.8rem;
            }
            .popup-content .popup-timer .time-block {
                min-width: 50px;
                padding: 0.3rem 0.8rem;
            }
            .popup-content .popup-timer .time-block span {
                font-size: 1.8rem;
            }
            .popup-content h2 {
                font-size: 1.6rem;
            }
            .popup-content .popup-icon {
                font-size: 4rem;
            }
        }
        @media (max-width: 480px) {
            .popup-content .popup-input {
                flex-direction: column;
            }
            .popup-content .popup-input input {
                min-width: auto;
            }
            .popup-content .popup-input .btn-primary {
                width: 100%;
            }
            .popup-content {
                padding: 2rem 1.2rem;
            }
        }

        /* ============================================
           CARRITO MODAL
           ============================================ */
        .cart-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            backdrop-filter: blur(25px);
            z-index: 2000;
            align-items: center;
            justify-content: center;
        }
        .cart-modal.show {
            display: flex;
            animation: fadeInModal 0.3s ease;
        }
        @keyframes fadeInModal {
            from {
                opacity: 0;
                transform: scale(0.95);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }
        .cart-modal-content {
            background: #fff;
            border-radius: var(--radius);
            padding: 3rem 3.5rem;
            max-width: 550px;
            width: 90%;
            max-height: 80vh;
            overflow-y: auto;
            position: relative;
            animation: slideUpModal 0.4s ease;
            transition: var(--transition);
        }
        @keyframes slideUpModal {
            from {
                transform: translateY(60px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }
        body.dark-mode .cart-modal-content {
            background: #1a0b1a;
        }
        .cart-modal-content .close-cart {
            position: absolute;
            top: 1rem;
            right: 1.5rem;
            font-size: 2.2rem;
            cursor: pointer;
            color: #aaa;
            transition: var(--transition);
            background: none;
            border: none;
        }
        .cart-modal-content .close-cart:hover {
            color: var(--primary);
            transform: rotate(90deg) scale(1.1);
        }
        .cart-modal-content h2 {
            font-family: var(--font-serif);
            color: var(--text-dark);
            margin-bottom: 1.5rem;
            font-size: 2rem;
        }
        body.dark-mode .cart-modal-content h2 {
            color: #f0e8f0;
        }
        .cart-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0.8rem 0;
            border-bottom: 1px solid rgba(255, 182, 193, 0.04);
            transition: var(--transition);
        }
        body.dark-mode .cart-item {
            border-color: rgba(255, 182, 193, 0.02);
        }
        .cart-item .cart-item-info {
            display: flex;
            flex-direction: column;
        }
        .cart-item .cart-item-name {
            font-weight: 600;
            color: var(--text-dark);
            transition: var(--transition);
        }
        body.dark-mode .cart-item .cart-item-name {
            color: #f0e8f0;
        }
        .cart-item .cart-item-price {
            color: var(--primary);
            font-weight: 700;
        }
        body.dark-mode .cart-item .cart-item-price {
            color: var(--primary-light);
        }
        .cart-item .cart-item-remove {
            background: none;
            border: none;
            color: #e74c3c;
            cursor: pointer;
            font-size: 1.4rem;
            transition: var(--transition);
        }
        .cart-item .cart-item-remove:hover {
            transform: scale(1.2);
        }
        .cart-total {
            display: flex;
            justify-content: space-between;
            font-size: 1.4rem;
            font-weight: 800;
            padding: 1rem 0;
            border-top: 2px solid rgba(255, 182, 193, 0.04);
            margin-top: 0.5rem;
            transition: var(--transition);
        }
        body.dark-mode .cart-total {
            border-color: rgba(255, 182, 193, 0.02);
        }
        .cart-total .total-price {
            color: var(--primary);
        }
        body.dark-mode .cart-total .total-price {
            color: var(--primary-light);
        }
        .cart-empty {
            text-align: center;
            color: #7a4a7a;
            padding: 2.5rem 0;
            font-size: 1.1rem;
        }
        body.dark-mode .cart-empty {
            color: #c9a8c9;
        }
        .cart-modal-content .btn-primary {
            width: 100%;
            text-align: center;
            margin-top: 1rem;
        }
        .cart-summary {
            display: none;
            background: rgba(214, 51, 132, 0.02);
            padding: 1rem 1.5rem;
            border-radius: var(--radius-sm);
            margin-bottom: 1rem;
            text-align: center;
            border: 1px solid rgba(214, 51, 132, 0.02);
        }
        .cart-summary p {
            font-weight: 700;
            color: var(--primary);
        }
        body.dark-mode .cart-summary p {
            color: var(--primary-light);
        }
        .cart-summary .summary-text {
            font-size: 0.9rem;
            color: #7a4a7a;
        }
        body.dark-mode .cart-summary .summary-text {
            color: #c9a8c9;
        }

        @media (max-width: 480px) {
            .cart-modal-content {
                padding: 1.8rem;
            }
            .cart-modal-content h2 {
                font-size: 1.5rem;
            }
        }

        /* ============================================
           NOTIFICACIÓN
           ============================================ */
        .notification {
            position: fixed;
            top: 5.5rem;
            right: 2rem;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            padding: 1rem 2.5rem;
            border-radius: var(--radius-sm);
            box-shadow: 0 8px 50px rgba(0, 0, 0, 0.04);
            border-left: 4px solid var(--primary);
            transform: translateX(120%);
            transition: transform 0.5s cubic-bezier(0.34, 1.56, 0.64, 1);
            z-index: 3000;
            font-weight: 600;
            font-size: 0.95rem;
            display: flex;
            align-items: center;
            gap: 0.8rem;
        }
        body.dark-mode .notification {
            background: rgba(26, 11, 26, 0.95);
            color: #f0e8f0;
        }
        .notification.show {
            transform: translateX(0);
        }
        .notification .notif-icon {
            font-size: 1.6rem;
        }

        @media (max-width: 750px) {
            .notification {
                right: 1rem;
                left: 1rem;
                padding: 0.8rem 1.5rem;
                font-size: 0.85rem;
                top: 4.5rem;
            }
        }

        /* ============================================
           WHATSAPP FLOTANTE
           ============================================ */
        .whatsapp-float {
            position: fixed;
            bottom: 2.5rem;
            right: 2.5rem;
            background: #25D366;
            color: #fff;
            width: 70px;
            height: 70px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            text-decoration: none;
            box-shadow: 0 8px 50px rgba(37, 211, 102, 0.3);
            transition: var(--transition);
            z-index: 999;
            animation: pulseWhatsapp 2.5s infinite;
        }
        .whatsapp-float:hover {
            transform: scale(1.1) rotate(-5deg);
            box-shadow: 0 12px 70px rgba(37, 211, 102, 0.4);
        }
        @keyframes pulseWhatsapp {
            0%,
            100% {
                box-shadow: 0 8px 50px rgba(37, 211, 102, 0.3);
            }
            50% {
                box-shadow: 0 8px 70px rgba(37, 211, 102, 0.5);
            }
        }
        @media (max-width: 750px) {
            .whatsapp-float {
                width: 60px;
                height: 60px;
                font-size: 2.5rem;
                bottom: 1.5rem;
                right: 1.5rem;
            }
        }
        @media (max-width: 480px) {
            .whatsapp-float {
                width: 55px;
                height: 55px;
                font-size: 2.2rem;
                bottom: 1.2rem;
                right: 1.2rem;
            }
        }

        /* ============================================
           VOLVER ARRIBA
           ============================================ */
        .btn-back-top {
            position: fixed;
            bottom: 85px;
            right: 2.5rem;
            background: linear-gradient(135deg, var(--primary-dark), var(--primary), var(--primary-light));
            color: #fff;
            width: 58px;
            height: 58px;
            border-radius: 50%;
            display: none;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            text-decoration: none;
            box-shadow: 0 4px 35px rgba(194, 24, 91, 0.25);
            z-index: 999;
            transition: var(--transition);
            border: none;
            cursor: pointer;
        }
        .btn-back-top:hover {
            transform: translateY(-8px) scale(1.05);
            box-shadow: 0 8px 60px rgba(194, 24, 91, 0.35);
        }
        @media (max-width: 750px) {
            .btn-back-top {
                width: 48px;
                height: 48px;
                font-size: 1.5rem;
                bottom: 75px;
                right: 1.2rem;
            }
        }
        @media (max-width: 480px) {
            .btn-back-top {
                width: 42px;
                height: 42px;
                font-size: 1.3rem;
                bottom: 70px;
                right: 1rem;
            }
        }

        /* ============================================
           COMPARTIR
           ============================================ */
        .share-btn {
            position: fixed;
            bottom: 280px;
            right: 2.5rem;
            background: linear-gradient(135deg, #1a73e8, #4285f4, #1a73e8);
            background-size: 200% 200%;
            animation: shimmerShare 3s ease infinite;
            color: #fff;
            width: 58px;
            height: 58px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.8rem;
            text-decoration: none;
            box-shadow: 0 4px 35px rgba(26, 115, 232, 0.25);
            z-index: 999;
            transition: var(--transition);
            border: none;
            cursor: pointer;
        }
        @keyframes shimmerShare {
            0%,
            100% {
                background-position: 0% 50%;
            }
            50% {
                background-position: 100% 50%;
            }
        }
        .share-btn:hover {
            transform: translateY(-8px) scale(1.05);
            box-shadow: 0 8px 60px rgba(26, 115, 232, 0.35);
        }
        @media (max-width: 750px) {
            .share-btn {
                width: 48px;
                height: 48px;
                font-size: 1.5rem;
                bottom: 240px;
                right: 1.2rem;
            }
        }
        @media (max-width: 480px) {
            .share-btn {
                width: 42px;
                height: 42px;
                font-size: 1.3rem;
                bottom: 210px;
                right: 1rem;
            }
        }

        /* ============================================
           FOOTER
           ============================================ */
        footer {
            background: linear-gradient(135deg, #0a050a, #1a0b1a, #0a050a);
            color: #e8d5e8;
            padding: 4.5rem 5% 2.5rem;
            border-radius: 90px 90px 0 0;
            margin-top: 4.5rem;
            position: relative;
            overflow: hidden;
        }
        footer::before {
            content: '✦';
            font-size: 15rem;
            position: absolute;
            right: -4rem;
            bottom: -5rem;
            opacity: 0.02;
            transform: rotate(20deg);
        }
        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 3rem;
            max-width: 1200px;
            margin: 0 auto;
            position: relative;
            z-index: 1;
        }
        .footer-grid h4 {
            font-family: var(--font-serif);
            color: #f8e8f0;
            margin-bottom: 0.8rem;
            font-size: 1.3rem;
            font-weight: 700;
        }
        .footer-grid a {
            display: block;
            color: #c9a8c9;
            text-decoration: none;
            font-size: 0.9rem;
            margin-bottom: 0.5rem;
            transition: var(--transition);
            font-weight: 400;
        }
        .footer-grid a:hover {
            color: var(--primary-light);
            transform: translateX(8px);
        }
        .payment-icons {
            display: flex;
            gap: 1rem;
            font-size: 2.8rem;
            flex-wrap: wrap;
        }
        .footer-bottom {
            text-align: center;
            border-top: 1px solid rgba(255, 255, 255, 0.03);
            padding-top: 2.5rem;
            margin-top: 3rem;
            font-size: 0.85rem;
            color: #9a7a9a;
            position: relative;
            z-index: 1;
        }
        .footer-bottom .heart {
            color: var(--primary-light);
            display: inline-block;
            animation: pulseHeart 1.8s ease-in-out infinite;
        }
        @keyframes pulseHeart {
            0%,
            100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.3);
            }
        }

        @media (max-width: 750px) {
            footer {
                border-radius: 50px 50px 0 0;
                padding: 3rem 1.5rem 1.5rem;
            }
            .footer-grid {
                gap: 2rem;
            }
            .payment-icons {
                font-size: 2.2rem;
            }
        }
        @media (max-width: 480px) {
            .footer-grid {
                grid-template-columns: 1fr 1fr;
                gap: 1.5rem;
            }
            .payment-icons {
                font-size: 1.8rem;
            }
            .footer-grid h4 {
                font-size: 1.1rem;
            }
            .footer-grid a {
                font-size: 0.8rem;
            }
        }
    </style>
</head>
<body>

    <!-- ===== PRELOADER ===== -->
    <div class="preloader" id="preloader">
        <div class="loader-ring">
            <div class="ring"></div>
            <div class="ring"></div>
            <div class="ring"></div>
        </div>
        <div class="loader-text">✦ Paulina ✦ Accesorios ✦</div>
    </div>

    <!-- ===== ENVÍO GRATIS ===== -->
    <div class="free-shipping">
        🚚 <span class="highlight">Envío gratis</span> en compras mayores a S/50 · 🎁 <span class="highlight">10% OFF</span> con código PAULINA10 · 🇵🇪 Envíos a todo Perú
    </div>

    <!-- ===== POP-UP ===== -->
    <div class="popup-overlay" id="popupOferta">
        <div class="popup-content">
            <button class="popup-close" id="popupClose">✕</button>
            <span class="popup-icon">🎉</span>
            <h2>¡Oferta Exclusiva!</h2>
            <p>Suscríbete y recibe <strong>10% de descuento</strong> en tu primera compra + <strong>envío gratis</strong></p>
            <div class="popup-timer">
                <div class="time-block">
                    <span id="popupHoras">00</span>
                    <span class="label">Horas</span>
                </div>
                <span style="font-size: 2.2rem; color: var(--primary); font-weight: 700;">:</span>
                <div class="time-block">
                    <span id="popupMinutos">00</span>
                    <span class="label">Minutos</span>
                </div>
                <span style="font-size: 2.2rem; color: var(--primary); font-weight: 700;">:</span>
                <div class="time-block">
                    <span id="popupSegundos">00</span>
                    <span class="label">Segundos</span>
                </div>
            </div>
            <form class="popup-input" id="popupForm">
                <input type="email" placeholder="Tu correo electrónico" required />
                <button type="submit" class="btn-primary">🎁 ¡Quiero mi descuento!</button>
            </form>
            <p style="font-size: 0.8rem; margin-top: 1.2rem; opacity: 0.5;">No compartimos tu correo · Puedes cancelar cuando quieras</p>
        </div>
    </div>

    <!-- ===== NOTIFICACIÓN ===== -->
    <div class="notification" id="notification">
        <span class="notif-icon">✅</span>
        <span id="notificationText">Producto agregado al carrito</span>
    </div>

    <!-- ===== NOTIFICACIÓN EN VIVO ===== -->
    <div class="live-notification" id="liveNotification">
        <span class="ln-emoji">🛍️</span>
        <span class="ln-name" id="lnName">María</span> compró <span class="ln-product" id="lnProduct">Aretes Bohemios</span>
        <span class="ln-time" id="lnTime">hace 2 minutos</span>
    </div>

    <!-- ===== MENÚ HAMBURGUESA ===== -->
    <div class="hamburger" id="hamburger">
        <span></span>
        <span></span>
        <span></span>
    </div>
    <div class="mobile-menu" id="mobileMenu">
        <a href="#inicio">✨ Inicio</a>
        <a href="#productos">🛍️ Productos</a>
        <a href="#ofertas">🔥 Ofertas</a>
        <a href="#testimonios">💬 Testimonios</a>
        <a href="#contacto">📩 Contacto</a>
        <a href="#" id="mobileClose" style="font-size:1.2rem; opacity:0.6;">✕ Cerrar</a>
    </div>

    <!-- ===== LIGHTBOX ===== -->
    <div class="lightbox" id="lightbox">
        <span class="lightbox-close" id="lightboxClose">✕</span>
        <div class="lightbox-content" id="lightboxContent">
            <span class="lb-emoji">📿</span>
            <span class="lb-name">Aretes Bohemios</span>
            <span class="lb-price">$25.00</span>
        </div>
    </div>

    <!-- ===== NAVBAR ===== -->
    <nav class="navbar">
        <div class="logo">✦ Paulina ✦ Accesorios</div>
        <ul class="nav-links">
            <li><a href="#inicio">Inicio</a></li>
            <li><a href="#productos">Productos</a></li>
            <li><a href="#ofertas">Ofertas</a></li>
            <li><a href="#testimonios">Testimonios</a></li>
            <li><a href="#contacto">Contacto</a></li>
        </ul>
        <div class="nav-right">
            <div class="search-box">
                <input type="text" id="searchInput" placeholder="Buscar productos..." />
                <button id="searchBtn">🔍</button>
            </div>
            <div class="cart-icon" id="cartIcon">
                🛍️ <span class="cart-count" id="cartCount">0</span>
            </div>
        </div>
    </nav>

    <!-- ===== HERO ===== -->
    <section class="hero" id="inicio">
        <div class="hero-text">
            <div class="brand-tag">✦ Colección 2025 ✦</div>
            <h1>Belleza que <br /><span class="highlight">brilla con estilo</span></h1>
            <p>Descubre nuestra colección exclusiva de aretes artesanales, extensiones de pestañas y accesorios diseñados para realzar tu esencia única. Calidad premium y envíos a todo Perú.</p>
            <div class="hero-stats">
                <div class="stat">
                    <span class="number" id="visitCount">0</span>
                    <span class="label">Visitas</span>
                </div>
                <div class="stat">
                    <span class="number">+500</span>
                    <span class="label">Clientas felices</span>
                </div>
                <div class="stat">
                    <span class="number">⭐ 4.9</span>
                    <span class="label">Calificación</span>
                </div>
                <div class="stat">
                    <span class="number">🇵🇪</span>
                    <span class="label">Envíos a todo Perú</span>
                </div>
            </div>
            <div style="margin-top: 2rem;">
                <a href="#productos" class="btn-primary">✨ Ver colección</a>
                <a href="#ofertas" class="btn-secondary">🔥 Ofertas</a>
            </div>
        </div>
        <div class="hero-image">
            <span>💎</span>
        </div>
    </section>

    <!-- ===== SLIDER ===== -->
    <section class="section">
        <h2 class="section-title">✨ <span class="accent">Lo más destacado</span></h2>
        <p class="section-subtitle">Descubre nuestras colecciones especiales de esta temporada</p>
        <div class="slider-container">
            <div class="slider" id="slider">
                <div class="slider-slide" style="background: linear-gradient(135deg, #fce4ec, #f8e8f0);">
                    <span class="slide-emoji">📿</span>
                    <span class="slide-text">✨ Aretes artesanales · Hechos a mano</span>
                </div>
                <div class="slider-slide" style="background: linear-gradient(135deg, #f8e8f0, #f3e5f5);">
                    <span class="slide-emoji">👁️</span>
                    <span class="slide-text">🌸 Extensiones de pestañas · Volumen premium</span>
                </div>
                <div class="slider-slide" style="background: linear-gradient(135deg, #f3e5f5, #e8eaf6);">
                    <span class="slide-emoji">💍</span>
                    <span class="slide-text">💎 Joyería fina · Elegancia y estilo</span>
                </div>
                <div class="slider-slide" style="background: linear-gradient(135deg, #e8eaf6, #fce4ec);">
                    <span class="slide-emoji">💄</span>
                    <span class="slide-text">🌟 Maquillaje profesional · Calidad premium</span>
                </div>
            </div>
            <button class="slider-btn prev" id="sliderPrev">❮</button>
            <button class="slider-btn next" id="sliderNext">❯</button>
        </div>
        <div class="slider-dots" id="sliderDots"></div>
    </section>

    <!-- ===== CARRUSEL DE PRODUCTOS DESTACADOS ===== -->
    <section class="section">
        <h2 class="section-title">🏆 <span class="accent">Productos destacados</span></h2>
        <p class="section-subtitle">Los favoritos de esta temporada que no puedes dejar pasar</p>
        <div class="featured-carousel">
            <button class="carousel-btn prev" id="carouselPrev">❮</button>
            <div class="carousel-track" id="carouselTrack">
                <!-- Se carga con JavaScript -->
            </div>
            <button class="carousel-btn next" id="carouselNext">❯</button>
        </div>
    </section>

    <!-- ===== OFERTA RELÁMPAGO ===== -->
    <section class="section" id="ofertas">
        <div class="flash-sale">
            <h2>⚡ Oferta Relámpago</h2>
            <p>¡Solo por tiempo limitado! Aprovecha este descuento especial antes de que termine</p>
            <div class="flash-timer">
                <div class="time-block">
                    <span id="flashHoras">00</span>
                    <span class="time-label">Horas</span>
                </div>
                <span>:</span>
                <div class="time-block">
                    <span id="flashMinutos">00</span>
                    <span class="time-label">Minutos</span>
                </div>
                <span>:</span>
                <div class="time-block">
                    <span id="flashSegundos">00</span>
                    <span class="time-label">Segundos</span>
                </div>
            </div>
            <div class="flash-product">
                <span class="flash-emoji">👁️</span>
                <h3>Extensiones de Pestañas</h3>
                <div class="flash-price">
                    $35.00 <span class="old">$60.00</span>
                </div>
                <div style="margin-top: 0.5rem; font-size: 0.9rem; opacity: 0.7;">🔥 ¡Solo quedan 5 unidades!</div>
                <a href="#productos" class="btn-primary" style="margin-top: 1rem; padding: 0.8rem 3rem; font-size: 0.95rem;">🔥 Aprovechar oferta</a>
            </div>
        </div>
    </section>

    <!-- ===== MÁS VENDIDOS ===== -->
    <section class="section">
        <h2 class="section-title">🏆 <span class="accent">Más vendidos</span></h2>
        <p class="section-subtitle">Lo que nuestras clientas más aman y recomiendan</p>
        <div class="product-grid" id="masVendidos"></div>
    </section>

    <!-- ===== PRODUCTOS ===== -->
    <section class="section" id="productos">
        <h2 class="section-title">Nuestros <span class="accent">productos</span></h2>
        <p class="section-subtitle">Lo mejor para ti, en cada detalle y ocasión</p>

        <!-- FILTRO DE PRECIO -->
        <div class="price-filter">
            <label>💰 Precio:</label>
            <input type="number" id="priceMin" placeholder="Mín" min="0" />
            <span>a</span>
            <input type="number" id="priceMax" placeholder="Máx" min="0" />
            <button class="btn-primary" id="filterPrice">Filtrar</button>
            <button class="btn-secondary" id="clearFilter" style="padding:0.5rem 2rem;font-size:0.9rem;margin:0;">Limpiar</button>
        </div>

        <!-- ORDENAR -->
        <div class="sort-options">
            <label>Ordenar por:</label>
            <select id="sortSelect">
                <option value="default">Relevancia</option>
                <option value="price-asc">Precio: menor a mayor</option>
                <option value="price-desc">Precio: mayor a menor</option>
                <option value="name">Nombre A-Z</option>
                <option value="popular">Más populares</option>
            </select>
        </div>

        <div class="category-pills" id="categoryPills">
            <span class="pill active" data-category="todos">✨ Todos</span>
            <span class="pill" data-category="aretes">📿 Aretes</span>
            <span class="pill" data-category="pestanas">👁️ Pestañas</span>
            <span class="pill" data-category="anillos">💍 Anillos</span>
            <span class="pill" data-category="maquillaje">💄 Maquillaje</span>
        </div>

        <div class="product-grid" id="productGrid"></div>
    </section>

    <!-- ===== BANNER OFERTAS ===== -->
    <section class="section">
        <div class="banner">
            <h2>🌸 <span class="highlight">2x1</span> en extensiones de pestañas</h2>
            <p>Lleva dos pares por el precio de uno. ¡Solo por tiempo limitado! Aprovecha esta oportunidad única.</p>
            <div class="timer">
                <div class="time-block">
                    <span id="horas">00</span>
                    <span class="time-label">Horas</span>
                </div>
                <span>:</span>
                <div class="time-block">
                    <span id="minutos">00</span>
                    <span class="time-label">Minutos</span>
                </div>
                <span>:</span>
                <div class="time-block">
                    <span id="segundos">00</span>
                    <span class="time-label">Segundos</span>
                </div>
            </div>
            <a href="#productos" class="btn-primary">🔥 Aprovechar oferta</a>
        </div>
    </section>

    <!-- ===== FORMAS DE PAGO ===== -->
    <section class="section">
        <h2 class="section-title">💳 <span class="accent">Formas de pago</span></h2>
        <p class="section-subtitle">Elige la que más te convenga y compra con total confianza</p>
        <div class="payment-methods">
            <div class="payment-item"><span class="icon">📱</span><span class="name">Yape</span></div>
            <div class="payment-item"><span class="icon">📱</span><span class="name">Plin</span></div>
            <div class="payment-item"><span class="icon">🏦</span><span class="name">Transferencia</span></div>
            <div class="payment-item"><span class="icon">💵</span><span class="name">Efectivo</span></div>
            <div class="payment-item"><span class="icon">💳</span><span class="name">Tarjeta</span></div>
            <div class="payment-item"><span class="icon">📦</span><span class="name">Contraentrega</span></div>
        </div>
        <div class="security-badge">
            <span class="shield">🛡️</span>
            <span>Compra 100% segura · Tus datos están protegidos · Envíos a todo Perú</span>
        </div>
    </section>

    <!-- ===== TESTIMONIOS Y REDES SOCIALES ===== -->
    <section class="section" id="testimonios">
        <h2 class="section-title">💬 Lo que dicen <span class="accent">nuestras clientas</span></h2>
        <p class="section-subtitle">La opinión de quienes ya brillan con Paulina Accesorios</p>
        <div class="testimonials" id="testimonials"></div>

        <!-- ===== REDES SOCIALES - VERSIÓN DEFINITIVA ===== -->
        <div class="social-section">
            <p class="social-title">🌟 Síguenos en redes sociales</p>
            <div class="social-links">
                <!-- Instagram -->
                <a href="#" class="social-link instagram" target="_blank" title="Instagram">
                    <svg viewBox="0 0 24 24" fill="white">
                        <rect x="2" y="2" width="20" height="20" rx="5" ry="5"/>
                        <circle cx="12" cy="12" r="5"/>
                        <circle cx="17.5" cy="6.5" r="1.5"/>
                    </svg>
                    <span class="social-name">Instagram</span>
                </a>
                <!-- TikTok -->
                <a href="#" class="social-link tiktok" target="_blank" title="TikTok">
                    <svg viewBox="0 0 24 24" fill="white">
                        <path d="M16.6 5.82s.51.5 0 0A4.27 4.27 0 0 1 15.54 3h-3.09v12.4a2.59 2.59 0 0 1-2.59 2.5c-1.42 0-2.6-1.16-2.6-2.6 0-1.45 1.18-2.6 2.6-2.6.26 0 .51.04.75.12v-3.1a5.62 5.62 0 0 0-4.89.36 5.62 5.62 0 0 0-2.1 2.1 5.62 5.62 0 0 0-.36 4.89 5.62 5.62 0 0 0 2.1 2.1 5.62 5.62 0 0 0 4.89.36 5.62 5.62 0 0 0 2.1-2.1 5.62 5.62 0 0 0 .36-4.89l.1-1.2V3h3.09a4.27 4.27 0 0 0 1.06 2.82z"/>
                    </svg>
                    <span class="social-name">TikTok</span>
                </a>
                <!-- Facebook -->
                <a href="#" class="social-link facebook" target="_blank" title="Facebook">
                    <svg viewBox="0 0 24 24" fill="white">
                        <path d="M24 12.07C24 5.41 18.63 0 12 0S0 5.4 0 12.07C0 18.1 4.39 23.1 10.13 24v-8.44H7.08v-3.49h3.05V9.41c0-3.02 1.8-4.7 4.54-4.7 1.31 0 2.68.23 2.68.23v2.96h-1.51c-1.49 0-1.95.93-1.95 1.88v2.26h3.32l-.53 3.48h-2.8V24C19.62 23.1 24 18.1 24 12.07z"/>
                    </svg>
                    <span class="social-name">Facebook</span>
                </a>
                <!-- WhatsApp -->
                <a href="https://wa.me/51923861016" class="social-link whatsapp" target="_blank" title="WhatsApp">
                    <svg viewBox="0 0 24 24" fill="white">
                        <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347z"/>
                        <path d="M12 0C5.373 0 0 5.373 0 12c0 2.317.656 4.487 1.801 6.35L0 24l5.65-1.801C7.513 23.344 9.683 24 12 24c6.627 0 12-5.373 12-12S18.627 0 12 0zm0 22c-2.083 0-4.006-.666-5.588-1.8l-.398-.238-3.148 1.002 1.002-3.148-.238-.398A9.894 9.894 0 0 1 2 12C2 6.477 6.477 2 12 2s10 4.477 10 10-4.477 10-10 10z"/>
                    </svg>
                    <span class="social-name">WhatsApp</span>
                </a>
            </div>
            <p style="margin-top: 1rem; font-size: 0.8rem; opacity: 0.5; color: #7a4a7a;">
                📲 Síguenos y entérate de todas nuestras promociones
            </p>
        </div>
    </section>

    <!-- ===== CONSEJOS DE BELLEZA ===== -->
    <section class="section">
        <h2 class="section-title">💡 <span class="accent">Consejos de belleza</span></h2>
        <p class="section-subtitle">Tips profesionales para lucir espectacular en cualquier ocasión</p>
        <div class="tips-grid" id="tipsGrid"></div>
    </section>

    <!-- ===== FAQ ===== -->
    <section class="section">
        <h2 class="section-title">❓ <span class="accent">Preguntas frecuentes</span></h2>
        <p class="section-subtitle">Resolvemos todas tus dudas para que compres con total confianza</p>
        <div class="faq-grid" id="faqGrid">
            <div class="faq-item">
                <div class="faq-question">
                    <span>📦 ¿Cuánto tiempo tardan los envíos?</span>
                    <span class="icon">▼</span>
                </div>
                <div class="faq-answer">Los envíos tardan entre 2 a 4 días hábiles dependiendo de tu ubicación. En Lima es de 24 a 48 horas. Tenemos envíos a todo el Perú.</div>
            </div>
            <div class="faq-item">
                <div class="faq-question">
                    <span>💳 ¿Qué métodos de pago aceptan?</span>
                    <span class="icon">▼</span>
                </div>
                <div class="faq-answer">Aceptamos Yape, Plin, transferencia bancaria, efectivo, tarjetas de crédito/débito y contraentrega. ¡Tú eliges!</div>
            </div>
            <div class="faq-item">
                <div class="faq-question">
                    <span>🔄 ¿Puedo cambiar o devolver un producto?</span>
                    <span class="icon">▼</span>
                </div>
                <div class="faq-answer">Sí, tienes hasta 7 días después de recibir tu pedido para solicitar un cambio o devolución sin costo adicional. Tu satisfacción es nuestra prioridad.</div>
            </div>
            <div class="faq-item">
                <div class="faq-question">
                    <span>📍 ¿Tienen tienda física?</span>
                    <span class="icon">▼</span>
                </div>
                <div class="faq-answer">Sí, estamos en Francisco Bardales 705, Yurimaguas. ¡Te esperamos con los brazos abiertos! Horario: Lunes a Sábado 9am - 8pm.</div>
            </div>
            <div class="faq-item">
                <div class="faq-question">
                    <span>🎁 ¿Tienen promociones o descuentos?</span>
                    <span class="icon">▼</span>
                </div>
                <div class="faq-answer">¡Sí! Usa el código <strong>PAULINA10</strong> para obtener un 10% de descuento en tu primera compra. Además, tenemos ofertas constantes y promociones especiales.</div>
            </div>
        </div>
    </section>

    <!-- ===== CUPÓN Y CONTACTO ===== -->
    <section class="section" id="contacto">
        <h2 class="section-title">📩 <span class="accent">Contáctanos</span></h2>
        <p class="section-subtitle">¿Tienes dudas? Escríbenos y te respondemos en menos de 24 horas</p>

        <div class="coupon-section">
            <p>🎁 Usa este cupón en tu próxima compra</p>
            <div class="coupon-code">PAULINA10</div>
            <p style="font-size: 0.85rem;">10% de descuento en tu primera compra · Válido por tiempo limitado · Envíos a todo Perú</p>
        </div>

        <form class="contact-form" id="contactForm" style="margin-top: 2rem;">
            <div class="form-group">
                <label for="nombre">👤 Nombre completo</label>
                <input type="text" id="nombre" placeholder="Ej: María Pérez" required />
            </div>
            <div class="form-group">
                <label for="email">📧 Correo electrónico</label>
                <input type="email" id="email" placeholder="Ej: maria@email.com" required />
            </div>
            <div class="form-group">
                <label for="mensaje">💬 Mensaje</label>
                <textarea id="mensaje" placeholder="Cuéntanos qué necesitas, estaremos encantados de ayudarte..." required></textarea>
            </div>
            <button type="submit" class="btn-primary">📨 Enviar mensaje</button>
        </form>
    </section>

    <!-- ===== MAPA ===== -->
    <section class="section">
        <h2 class="section-title">📍 <span class="accent">Visítanos</span></h2>
        <p class="section-subtitle">Francisco Bardales 705 - Yurimaguas · Te esperamos con los brazos abiertos</p>
        <div class="map-container">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3965.789!2d-76.123456!3d-5.901234!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x91c1f0f0f0f0f0f0%3A0x0f0f0f0f0f0f0f0f!2sFrancisco%20Bardales%20705%2C%20Yurimaguas%2016501!5e0!3m2!1ses!2spe!4v1234567890" width="100%" height="400" style="border:0;" allowfullscreen="" loading="lazy" title="Paulina Accesorios - Francisco Bardales 705, Yurimaguas"></iframe>
        </div>
        <div class="map-info">
            <span class="map-icon">📍</span>
            <h3>Francisco Bardales 705</h3>
            <p>Yurimaguas 16501 · Horario: Lunes a Sábado 9am - 8pm</p>
            <div class="map-buttons">
                <a href="https://www.google.com/maps/dir/?api=1&destination=Francisco+Bardales+705+Yurimaguas+Peru" target="_blank" class="btn-primary">🗺️ Google Maps</a>
                <a href="https://waze.com/ul?q=Francisco+Bardales+705+Yurimaguas+Peru&navigate=yes" target="_blank" class="btn-secondary">🚗 Waze</a>
                <a href="https://wa.me/51923861016?text=Hola%20Paulina%2C%20quiero%20saber%20la%20ubicaci%C3%B3n%20de%20la%20tienda" target="_blank" class="btn-secondary">💬 WhatsApp</a>
            </div>
        </div>
    </section>

    <!-- ===== NEWSLETTER ===== -->
    <section class="section">
        <div class="newsletter-section">
            <h2 class="section-title">📧 <span class="accent">Suscríbete</span></h2>
            <p class="section-subtitle">Recibe ofertas exclusivas, novedades y promociones especiales directamente en tu correo</p>
            <form class="newsletter-form" id="newsletterForm">
                <input type="email" placeholder="Tu correo electrónico" required />
                <button type="submit" class="btn-primary">📨 Suscribirme</button>
            </form>
            <p style="margin-top: 1.2rem; font-size: 0.85rem; opacity: 0.5;">No compartimos tu correo · Puedes cancelar cuando quieras</p>
        </div>
    </section>

    <!-- ===== CARRITO MODAL ===== -->
    <div class="cart-modal" id="cartModal">
        <div class="cart-modal-content">
            <button class="close-cart" id="closeCart">✕</button>
            <h2>🛍️ Tu carrito</h2>
            <div class="cart-summary" id="cartSummary">
                <p>📋 Resumen de tu compra</p>
                <div class="summary-text" id="cartSummaryText"></div>
            </div>
            <div id="cartItems"><div class="cart-empty">🛒 Tu carrito está vacío<br><span style="font-size:0.8rem;opacity:0.5;">¡Empieza a comprar!</span></div></div>
            <div class="cart-total">
                <span>Total:</span>
                <span class="total-price" id="cartTotal">$0.00</span>
            </div>
            <button class="btn-primary" id="checkoutBtn">✅ Finalizar compra</button>
        </div>
    </div>

    <!-- ===== CARRITO FLOTANTE ===== -->
    <div class="floating-cart" id="floatingCart">
        <span class="fc-icon">🛍️</span>
        <span class="fc-count" id="fcCount">0</span>
        <span class="fc-total" id="fcTotal">$0.00</span>
    </div>

    <!-- ===== WHATSAPP FLOTANTE ===== -->
    <a href="https://wa.me/51923861016?text=Hola%20Paulina%20Accesorios%2C%20me%20interesa%20un%20producto%20y%20quiero%20m%C3%A1s%20informaci%C3%B3n%20sobre%20stock%20y%20env%C3%ADos" class="whatsapp-float" target="_blank" rel="noopener">💬</a>

    <!-- ===== MODO OSCURO ===== -->
    <button class="dark-mode-toggle" id="darkModeToggle" title="Cambiar modo oscuro">🌙</button>

    <!-- ===== COMPARTIR ===== -->
    <button class="share-btn" id="shareBtn" title="Compartir tienda">📤</button>

    <!-- ===== VOLVER ARRIBA ===== -->
    <button class="btn-back-top" id="backTopBtn" title="Volver arriba">↑</button>

    <!-- ===== CONFETTI ===== -->
    <div class="confetti-container" id="confettiContainer"></div>

    <!-- ===== FOOTER ===== -->
    <footer>
        <div class="footer-grid">
            <div>
                <h4>✦ Paulina Accesorios</h4>
                <a href="#">Sobre nosotros</a>
                <a href="#">Política de cambios</a>
                <a href="#">Términos y condiciones</a>
                <a href="#">Libro de reclamaciones</a>
            </div>
            <div>
                <h4>📞 Ayuda</h4>
                <a href="#">Preguntas frecuentes</a>
                <a href="#">Envíos y entregas</a>
                <a href="#">Devoluciones</a>
                <a href="#">Contacto</a>
            </div>
            <div>
                <h4>📱 Síguenos</h4>
                <a href="#">Instagram</a>
                <a href="#">Facebook</a>
                <a href="#">TikTok</a>
            </div>
            <div>
                <h4>💳 Formas de pago</h4>
                <div class="payment-icons">
                    <span>💳</span>
                    <span>📱</span>
                    <span>🏦</span>
                    <span>💵</span>
                </div>
                <div style="margin-top: 0.5rem; font-size: 0.8rem; opacity: 0.5;">Yape · Plin · Transferencia · Efectivo</div>
            </div>
        </div>
        <div class="footer-bottom">
            &copy; 2025 Paulina Accesorios · Hecho con <span class="heart">💖</span> para mujeres que brillan · 🇵🇪 Perú · Todos los derechos reservados
        </div>
    </footer>


    <!-- ============================================
    JAVASCRIPT
    ============================================ -->
    <script>
        // ============================================
        // DATOS
        // ============================================

        const productos = [
            { id: 1, nombre: 'Aretes Bohemios', categoria: 'aretes', descripcion: 'Hechos a mano con piedras naturales semi-preciosas, ideales para cualquier ocasión',
                precio: 25.00, precio_old: null, badge: '⭐ Top', emoji: '📿', stock: 8, compradores: 134 },
            { id: 5, nombre: 'Aretes de Perla', categoria: 'aretes', descripcion: 'Perlas naturales cultivadas con acabado dorado de 18k',
                precio: 38.00, precio_old: null, badge: '✨ Especial', emoji: '📿', stock: 12, compradores: 89 },
            { id: 2, nombre: 'Extensiones de Pestañas', categoria: 'pestanas',
                descripcion: 'Efecto volumen premium, duración de 4 a 6 semanas, ideales para cualquier ocasión',
                precio: 45.00, precio_old: 60.00, badge: '🔥 Oferta', emoji: '👁️', stock: 5, compradores: 256 },
            { id: 6, nombre: 'Pestañas Magnéticas', categoria: 'pestanas', descripcion: 'Fáciles de poner y quitar, sin necesidad de pegamento, reutilizables',
                precio: 55.00, precio_old: 75.00, badge: '🔥 2x1', emoji: '👁️', stock: 3, compradores: 178 },
            { id: 3, nombre: 'Anillo Flor de Loto', categoria: 'anillos', descripcion: 'Acero quirúrgico con baño de oro 18k y piedra natural',
                precio: 18.00, precio_old: null, badge: '💖 Favorito', emoji: '💍', stock: 15, compradores: 312 },
            { id: 7, nombre: 'Anillo de Compromiso', categoria: 'anillos', descripcion: 'Zirconia cúbica con baño de plata 925, elegante y duradero',
                precio: 65.00, precio_old: null, badge: '💎 Premium', emoji: '💍', stock: 4, compradores: 67 },
            { id: 9, nombre: 'Collar de Perlas', categoria: 'anillos', descripcion: 'Perlas cultivadas con cierre de plata 925, largo 45cm',
                precio: 42.00, precio_old: null, badge: '✨ Nuevo', emoji: '📿', stock: 7, compradores: 45 },
            { id: 4, nombre: 'Set de Brochas', categoria: 'maquillaje', descripcion: '5 piezas de brochas profesionales con cerdas hipoalergénicas',
                precio: 32.00, precio_old: null, badge: '🌸 Nuevo', emoji: '💄', stock: 10, compradores: 98 },
            { id: 8, nombre: 'Paleta de Sombras', categoria: 'maquillaje', descripcion: '12 tonos entre mate y shimmer, pigmentación intensa y duradera',
                precio: 28.00, precio_old: null, badge: '⭐ Top', emoji: '💄', stock: 6, compradores: 167 },
            { id: 10, nombre: 'Kit de Uñas', categoria: 'maquillaje',
                descripcion: 'Esmaltes semipermanentes + lámpara LED profesional para secado rápido',
                precio: 55.00, precio_old: null, badge: '⭐ Top', emoji: '💅', stock: 9, compradores: 123 }
        ];

        const masVendidosIds = [1, 2, 3, 4];
        const destacadosIds = [2, 3, 5, 8, 9, 10];

        const testimonios = [
            { nombre: 'Valeria M.', texto: 'Las extensiones de pestañas son increíbles, me duraron más de un mes y se ven tan naturales. ¡Las recomiendo totalmente!',
                estrellas: 5, fecha: '15/06/2025' },
            { nombre: 'Sofía R.', texto: 'Los aretes son hermosos y muy ligeros, los uso todos los días. La calidad es excelente y el diseño es único.',
                estrellas: 5, fecha: '10/06/2025' },
            { nombre: 'Camila G.', texto: 'El servicio es excelente, el empaque es súper bonito y todo llega perfecto. Sin duda compraré nuevamente.',
                estrellas: 5, fecha: '05/06/2025' },
            { nombre: 'Lucía M.', texto: 'Las pestañas magnéticas me cambiaron la vida, súper fáciles de poner y se ven divinas. ¡Me encantaron!',
                estrellas: 4, fecha: '01/06/2025' }
        ];

        const tips = [
            { icono: '👁️', titulo: 'Cómo cuidar tus extensiones',
                descripcion: 'Lava con shampoo suave, cepilla con cuidado y evita dormir boca abajo. Usa un cepillo especial para pestañas. Mantenimiento cada 3 semanas.' },
            { icono: '💍', titulo: 'Combina tus aretes',
                descripcion: 'Aretes grandes con ropa sencilla, aretes pequeños con estampados llamativos. La regla de oro: menos es más. Elige según tu estilo personal.' },
            { icono: '✨', titulo: 'Brilla con estilo',
                descripcion: 'Menos es más: elige un accesorio fuerte y combínalo con sutileza. Deja que una pieza hable por ti. La elegancia está en los detalles.' },
            { icono: '💄', titulo: 'Maquillaje duradero',
                descripcion: 'Usa prebase y sella con spray fijador para que dure todo el día. Hidrata bien tu piel antes del maquillaje. El skincare es la base de todo.' }
        ];

        const nombresClientes = ['María', 'Ana', 'Laura', 'Sofía', 'Valeria', 'Camila', 'Lucía', 'Paula', 'Elena', 'Gabriela',
            'Daniela', 'Andrea', 'Isabel', 'Carolina', 'Fernanda', 'Patricia', 'Rosa', 'Carmen', 'Teresa', 'Marta'
        ];


        // ============================================
        // VARIABLES GLOBALES
        // ============================================

        let cart = [];
        let notificationTimeout = null;
        let visitCount = parseInt(localStorage.getItem('visitas')) || 0;


        // ============================================
        // FUNCIONES UTILITARIAS
        // ============================================

        function mostrarNotificacion(mensaje, icono = '✅') {
            const notification = document.getElementById('notification');
            const text = document.getElementById('notificationText');
            if (!notification || !text) return;
            text.textContent = mensaje;
            document.querySelector('.notification .notif-icon').textContent = icono;
            notification.classList.add('show');
            if (notificationTimeout) clearTimeout(notificationTimeout);
            notificationTimeout = setTimeout(() => {
                notification.classList.remove('show');
            }, 3000);
        }

        function calcularDescuento(precio, precio_old) {
            if (!precio_old) return null;
            return Math.round(((precio_old - precio) / precio_old) * 100);
        }

        function generarTiempoVisto() {
            const minutos = Math.floor(Math.random() * 15) + 1;
            return `hace ${minutos} ${minutos === 1 ? 'minuto' : 'minutos'}`;
        }

        function generarNombreAleatorio() {
            return nombresClientes[Math.floor(Math.random() * nombresClientes.length)];
        }

        function lanzarConfetti() {
            const container = document.getElementById('confettiContainer');
            const colors = ['#c2185b', '#d63384', '#f06292', '#f9a825', '#43a047', '#1a73e8', '#ff6f00', '#e53935', '#9c27b0',
                '#00bcd4', '#ff5722', '#4caf50'
            ];
            const shapes = ['', 'circle', 'star', 'heart'];
            for (let i = 0; i < 120; i++) {
                const confetti = document.createElement('div');
                const shape = shapes[Math.floor(Math.random() * shapes.length)];
                confetti.className = 'confetti' + (shape ? ' ' + shape : '');
                confetti.style.left = Math.random() * 100 + '%';
                confetti.style.top = '-15px';
                confetti.style.background = colors[Math.floor(Math.random() * colors.length)];
                confetti.style.width = (Math.random() * 12 + 4) + 'px';
                confetti.style.height = (Math.random() * 12 + 4) + 'px';
                confetti.style.animationDuration = (Math.random() * 3 + 2) + 's';
                confetti.style.animationDelay = (Math.random() * 0.8) + 's';
                confetti.style.transform = `rotate(${Math.random() * 360}deg)`;
                container.appendChild(confetti);
                setTimeout(() => confetti.remove(), 5000);
            }
        }


        // ============================================
        // RENDERIZAR PRODUCTOS
        // ============================================

        function renderizarProductos(containerId, productosArray, limit = null, isCarousel = false) {
            const container = document.getElementById(containerId);
            if (!container) return;

            const items = limit ? productosArray.slice(0, limit) : productosArray;

            let html = '';
            items.forEach(producto => {
                const badgeClass = producto.precio_old ? 'sale' : '';
                const precioOldHtml = producto.precio_old ? `<span class="old">$${producto.precio_old.toFixed(2)}</span>` :
                    '';
                const descuento = calcularDescuento(producto.precio, producto.precio_old);
                const descuentoHtml = descuento ? `<span class="discount-percent">-${descuento}%</span>` : '';
                const stockHtml = producto.stock <= 3 ?
                    `<span class="stock-info low">⚠️ ¡Solo quedan ${producto.stock} unidades!</span>` :
                    `<span class="stock-info">✅ En stock (${producto.stock} disponibles)</span>`;
                const badgeHot = producto.stock <= 3 ? 'hot' : '';
                const badgeNew = producto.id >= 9 ? 'new' : '';
                const badgePremium = producto.precio >= 50 ? 'premium' : '';

                html += `
                    <div class="product-card" data-category="${producto.categoria}" data-nombre="${producto.nombre.toLowerCase()}" data-precio="${producto.precio}" data-id="${producto.id}" data-popular="${producto.compradores}">
                        <span class="badge ${badgeClass} ${badgeHot} ${badgeNew} ${badgePremium}">${producto.badge}</span>
                        ${descuento ? `<span class="badge discount">-${descuento}%</span>` : ''}
                        ${producto.stock <= 3 ? `<span class="badge stock">🔥 ¡Últimas unidades!</span>` : ''}
                        ${producto.precio >= 50 ? `<span class="badge premium">💎 Premium</span>` : ''}
                        <div class="product-img" data-emoji="${producto.emoji}" data-nombre="${producto.nombre}" data-precio="${producto.precio}" onclick="abrirLightbox('${producto.emoji}', '${producto.nombre}', '${producto.precio}')">${producto.emoji}</div>
                        <div class="buyers-count">👥 ${producto.compradores} personas lo compraron</div>
                        <div class="seen-time">👁️ ${generarTiempoVisto()}</div>
                        <h3>${producto.nombre}</h3>
                        <p class="desc">${producto.descripcion}</p>
                        ${stockHtml}
                        <span class="price">$${producto.precio.toFixed(2)} ${precioOldHtml} ${descuentoHtml}</span>
                        <button class="btn-add" data-id="${producto.id}" data-nombre="${producto.nombre}" data-precio="${producto.precio}" ${producto.stock === 0 ? 'disabled style="opacity:0.4;cursor:not-allowed;"' : ''}>
                            ${producto.stock === 0 ? '❌ Agotado' : '🛒 Añadir al carrito'}
                        </button>
                    </div>
                `;
            });

            if (isCarousel) {
                container.innerHTML = html;
            } else {
                container.innerHTML = html;
            }
        }


        // ============================================
        // LIGHTBOX
        // ============================================

        function abrirLightbox(emoji, nombre, precio) {
            const lightbox = document.getElementById('lightbox');
            const content = document.getElementById('lightboxContent');
            content.innerHTML = `
                <span class="lb-emoji">${emoji}</span>
                <span class="lb-name">${nombre}</span>
                <span class="lb-price">$${parseFloat(precio).toFixed(2)}</span>
            `;
            lightbox.classList.add('show');
            document.body.style.overflow = 'hidden';
        }

        document.getElementById('lightboxClose').addEventListener('click', () => {
            document.getElementById('lightbox').classList.remove('show');
            document.body.style.overflow = '';
        });
        document.getElementById('lightbox').addEventListener('click', (e) => {
            if (e.target === e.currentTarget) {
                document.getElementById('lightbox').classList.remove('show');
                document.body.style.overflow = '';
            }
        });


        // ============================================
        // CARRUSEL
        // ============================================

        function iniciarCarousel() {
            const track = document.getElementById('carouselTrack');
            const prevBtn = document.getElementById('carouselPrev');
            const nextBtn = document.getElementById('carouselNext');
            if (!track) return;

            const destacados = productos.filter(p => destacadosIds.includes(p.id));
            renderizarProductos('carouselTrack', destacados, null, true);

            let currentIndex = 0;
            const items = document.querySelectorAll('#carouselTrack .product-card');
            const itemWidth = items.length > 0 ? items[0].offsetWidth + 28 : 290;
            const visibleItems = Math.floor(track.parentElement.offsetWidth / itemWidth) || 1;
            const maxIndex = Math.max(0, items.length - visibleItems);

            function updateCarousel() {
                if (items.length === 0) return;
                const offset = currentIndex * (itemWidth);
                track.style.transform = `translateX(-${offset}px)`;
            }

            prevBtn.addEventListener('click', () => {
                if (currentIndex > 0) {
                    currentIndex--;
                    updateCarousel();
                }
            });

            nextBtn.addEventListener('click', () => {
                if (currentIndex < maxIndex) {
                    currentIndex++;
                    updateCarousel();
                }
            });

            window.addEventListener('resize', () => {
                const newVisible = Math.floor(track.parentElement.offsetWidth / itemWidth) || 1;
                const newMax = Math.max(0, items.length - newVisible);
                if (currentIndex > newMax) {
                    currentIndex = newMax;
                    updateCarousel();
                }
            });
        }


        // ============================================
        // RENDERIZAR TESTIMONIOS
        // ============================================

        function renderizarTestimonios() {
            const container = document.getElementById('testimonials');
            if (!container) return;
            let html = '';
            testimonios.forEach(t => {
                const estrellas = '★'.repeat(t.estrellas) + '☆'.repeat(5 - t.estrellas);
                html += `
                    <div class="testimonial">
                        <div class="stars">${estrellas}</div>
                        <p>"${t.texto}"</p>
                        <p class="name">— ${t.nombre}</p>
                        <span class="date">📅 ${t.fecha}</span>
                    </div>
                `;
            });
            container.innerHTML = html;
        }


        // ============================================
        // RENDERIZAR TIPS
        // ============================================

        function renderizarTips() {
            const container = document.getElementById('tipsGrid');
            if (!container) return;
            let html = '';
            tips.forEach(tip => {
                html += `
                    <div class="tip-card">
                        <span class="tip-icon">${tip.icono}</span>
                        <h3>${tip.titulo}</h3>
                        <p>${tip.descripcion}</p>
                    </div>
                `;
            });
            container.innerHTML = html;
        }


        // ============================================
        // NOTIFICACIONES EN VIVO
        // ============================================

        function iniciarNotificacionesVivo() {
            const el = document.getElementById('liveNotification');
            const nameEl = document.getElementById('lnName');
            const productEl = document.getElementById('lnProduct');
            const timeEl = document.getElementById('lnTime');

            const productosNombres = productos.map(p => p.nombre);

            function mostrarNotificacionVivo() {
                const nombre = generarNombreAleatorio();
                const producto = productosNombres[Math.floor(Math.random() * productosNombres.length)];
                const minutos = Math.floor(Math.random() * 15) + 1;
                nameEl.textContent = nombre;
                productEl.textContent = producto;
                timeEl.textContent = `hace ${minutos} ${minutos === 1 ? 'minuto' : 'minutos'}`;
                el.classList.add('show');
                setTimeout(() => {
                    el.classList.remove('show');
                }, 4500);
            }

            setTimeout(mostrarNotificacionVivo, 3000);
            setInterval(mostrarNotificacionVivo, Math.random() * 6000 + 8000);
        }


        // ============================================
        // BUSCADOR
        // ============================================

        function iniciarBuscador() {
            const input = document.getElementById('searchInput');
            const btn = document.getElementById('searchBtn');
            const products = document.querySelectorAll('#productGrid .product-card');

            function buscar() {
                const termino = input.value.toLowerCase().trim();
                products.forEach(product => {
                    const nombre = product.dataset.nombre || '';
                    if (nombre.includes(termino) || termino === '') {
                        product.style.display = 'block';
                    } else {
                        product.style.display = 'none';
                    }
                });
                document.querySelectorAll('.pill').forEach(p => p.classList.remove('active'));
                document.querySelector('.pill[data-category="todos"]').classList.add('active');
            }

            input.addEventListener('keyup', buscar);
            btn.addEventListener('click', buscar);
        }


        // ============================================
        // FILTRO DE PRECIO
        // ============================================

        function iniciarFiltroPrecio() {
            const btn = document.getElementById('filterPrice');
            const clearBtn = document.getElementById('clearFilter');
            const minInput = document.getElementById('priceMin');
            const maxInput = document.getElementById('priceMax');
            const products = document.querySelectorAll('#productGrid .product-card');

            btn.addEventListener('click', () => {
                const min = parseFloat(minInput.value) || 0;
                const max = parseFloat(maxInput.value) || Infinity;
                products.forEach(product => {
                    const precio = parseFloat(product.dataset.precio) || 0;
                    if (precio >= min && precio <= max) {
                        product.style.display = 'block';
                    } else {
                        product.style.display = 'none';
                    }
                });
            });

            clearBtn.addEventListener('click', () => {
                minInput.value = '';
                maxInput.value = '';
                products.forEach(product => {
                    product.style.display = 'block';
                });
            });
        }


        // ============================================
        // ORDENAR PRODUCTOS
        // ============================================

        function iniciarOrdenar() {
            const select = document.getElementById('sortSelect');
            const grid = document.getElementById('productGrid');

            select.addEventListener('change', () => {
                const products = Array.from(grid.querySelectorAll('.product-card'));
                const value = select.value;

                products.sort((a, b) => {
                    const nameA = a.dataset.nombre || '';
                    const nameB = b.dataset.nombre || '';
                    const priceA = parseFloat(a.dataset.precio) || 0;
                    const priceB = parseFloat(b.dataset.precio) || 0;
                    const popularA = parseInt(a.dataset.popular) || 0;
                    const popularB = parseInt(b.dataset.popular) || 0;

                    switch (value) {
                        case 'price-asc':
                            return priceA - priceB;
                        case 'price-desc':
                            return priceB - priceA;
                        case 'name':
                            return nameA.localeCompare(nameB);
                        case 'popular':
                            return popularB - popularA;
                        default:
                            return 0;
                    }
                });

                products.forEach(product => grid.appendChild(product));
            });
        }


        // ============================================
        // FILTRO POR CATEGORÍA
        // ============================================

        function iniciarFiltro() {
            const pills = document.querySelectorAll('.pill');
            const products = document.querySelectorAll('#productGrid .product-card');

            pills.forEach(pill => {
                pill.addEventListener('click', function() {
                    pills.forEach(p => p.classList.remove('active'));
                    this.classList.add('active');
                    const category = this.dataset.category;
                    document.getElementById('searchInput').value = '';
                    products.forEach(product => {
                        if (category === 'todos' || product.dataset.category === category) {
                            product.style.display = 'block';
                        } else {
                            product.style.display = 'none';
                        }
                    });
                });
            });
        }


        // ============================================
        // TIMERS
        // ============================================

        function iniciarTimer(idHoras, idMinutos, idSegundos, horas = 24) {
            const horasEl = document.getElementById(idHoras);
            const minutosEl = document.getElementById(idMinutos);
            const segundosEl = document.getElementById(idSegundos);
            if (!horasEl || !minutosEl || !segundosEl) return;

            const target = new Date();
            target.setHours(target.getHours() + horas);

            const timer = setInterval(() => {
                const now = new Date();
                const diff = target - now;
                if (diff <= 0) {
                    clearInterval(timer);
                    horasEl.textContent = '00';
                    minutosEl.textContent = '00';
                    segundosEl.textContent = '00';
                    return;
                }
                const h = Math.floor(diff / (1000 * 60 * 60));
                const m = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
                const s = Math.floor((diff % (1000 * 60)) / 1000);
                horasEl.textContent = String(h).padStart(2, '0');
                minutosEl.textContent = String(m).padStart(2, '0');
                segundosEl.textContent = String(s).padStart(2, '0');
            }, 1000);
        }


        // ============================================
        // SLIDER
        // ============================================

        function iniciarSlider() {
            const slider = document.getElementById('slider');
            const slides = document.querySelectorAll('.slider-slide');
            const prevBtn = document.getElementById('sliderPrev');
            const nextBtn = document.getElementById('sliderNext');
            const dotsContainer = document.getElementById('sliderDots');
            if (!slider || slides.length === 0) return;

            let currentSlide = 0;
            const totalSlides = slides.length;

            dotsContainer.innerHTML = '';
            slides.forEach((_, index) => {
                const dot = document.createElement('button');
                dot.classList.add('dot');
                if (index === 0) dot.classList.add('active');
                dot.dataset.index = index;
                dot.addEventListener('click', () => goToSlide(index));
                dotsContainer.appendChild(dot);
            });

            const dots = document.querySelectorAll('.dot');

            function goToSlide(index) {
                if (index < 0) index = totalSlides - 1;
                if (index >= totalSlides) index = 0;
                currentSlide = index;
                slider.style.transform = `translateX(-${currentSlide * 100}%)`;
                dots.forEach(d => d.classList.remove('active'));
                dots[currentSlide].classList.add('active');
            }

            prevBtn.addEventListener('click', () => goToSlide(currentSlide - 1));
            nextBtn.addEventListener('click', () => goToSlide(currentSlide + 1));

            let autoSlide = setInterval(() => goToSlide(currentSlide + 1), 6000);
            const container = document.querySelector('.slider-container');
            container.addEventListener('mouseenter', () => clearInterval(autoSlide));
            container.addEventListener('mouseleave', () => {
                autoSlide = setInterval(() => goToSlide(currentSlide + 1), 6000);
            });
        }


        // ============================================
        // CARRITO
        // ============================================

        function iniciarCarrito() {
            const cartCount = document.getElementById('cartCount');
            const cartItems = document.getElementById('cartItems');
            const cartTotal = document.getElementById('cartTotal');
            const cartModal = document.getElementById('cartModal');
            const cartIcon = document.getElementById('cartIcon');
            const closeCart = document.getElementById('closeCart');
            const checkoutBtn = document.getElementById('checkoutBtn');
            const cartSummary = document.getElementById('cartSummary');
            const cartSummaryText = document.getElementById('cartSummaryText');
            const fcCount = document.getElementById('fcCount');
            const fcTotal = document.getElementById('fcTotal');
            const floatingCart = document.getElementById('floatingCart');

            cartIcon.addEventListener('click', () => {
                cartModal.classList.add('show');
                renderCart();
                document.body.style.overflow = 'hidden';
            });

            floatingCart.addEventListener('click', () => {
                cartModal.classList.add('show');
                renderCart();
                document.body.style.overflow = 'hidden';
            });

            closeCart.addEventListener('click', () => {
                cartModal.classList.remove('show');
                document.body.style.overflow = '';
            });

            cartModal.addEventListener('click', (e) => {
                if (e.target === cartModal) {
                    cartModal.classList.remove('show');
                    document.body.style.overflow = '';
                }
            });

            document.addEventListener('click', function(e) {
                if (e.target.classList.contains('btn-add')) {
                    const nombre = e.target.dataset.nombre;
                    const precio = parseFloat(e.target.dataset.precio);
                    const existing = cart.find(item => item.nombre === nombre);
                    if (existing) {
                        existing.cantidad += 1;
                    } else {
                        cart.push({ nombre, precio, cantidad: 1 });
                    }
                    actualizarContador();
                    mostrarNotificacion(`✅ ${nombre} agregado al carrito`, '🛍️');
                    lanzarConfetti();
                    renderCart();
                }
            });

            function actualizarContador() {
                const total = cart.reduce((sum, item) => sum + item.cantidad, 0);
                const totalPrecio = cart.reduce((sum, item) => sum + (item.precio * item.cantidad), 0);
                cartCount.textContent = total;
                fcCount.textContent = total;
                fcTotal.textContent = `$${totalPrecio.toFixed(2)}`;
                if (total > 0) {
                    floatingCart.style.display = 'flex';
                } else {
                    floatingCart.style.display = 'none';
                }
            }

            function renderCart() {
                if (cart.length === 0) {
                    cartItems.innerHTML =
                        '<div class="cart-empty">🛒 Tu carrito está vacío<br><span style="font-size:0.8rem;opacity:0.5;">¡Empieza a comprar y llena tu carrito!</span></div>';
                    cartTotal.textContent = '$0.00';
                    cartSummary.style.display = 'none';
                    return;
                }

                cartSummary.style.display = 'block';
                let resumenText = '';
                cart.forEach(item => {
                    resumenText += `${item.nombre} x${item.cantidad}, `;
                });
                cartSummaryText.textContent = resumenText.slice(0, -2);

                let html = '';
                let total = 0;
                cart.forEach((item, index) => {
                    const subtotal = item.precio * item.cantidad;
                    total += subtotal;
                    html += `
                        <div class="cart-item">
                            <div class="cart-item-info">
                                <span class="cart-item-name">${item.nombre} × ${item.cantidad}</span>
                                <span class="cart-item-price">$${subtotal.toFixed(2)}</span>
                            </div>
                            <button class="cart-item-remove" data-index="${index}">✕</button>
                        </div>
                    `;
                });
                cartItems.innerHTML = html;
                cartTotal.textContent = `$${total.toFixed(2)}`;

                document.querySelectorAll('.cart-item-remove').forEach(btn => {
                    btn.addEventListener('click', function() {
                        const index = parseInt(this.dataset.index);
                        cart.splice(index, 1);
                        actualizarContador();
                        renderCart();
                        if (cart.length === 0) {
                            cartModal.classList.remove('show');
                            document.body.style.overflow = '';
                        }
                    });
                });
            }

            // FINALIZAR COMPRA
            checkoutBtn.addEventListener('click', function() {
                if (cart.length === 0) {
                    mostrarNotificacion('⚠️ Tu carrito está vacío', '⚠️');
                    return;
                }

                let mensaje = '✨ ¡Hola Paulina! ✨%0A%0A';
                mensaje += '📦 Quiero hacer el siguiente pedido:%0A%0A';
                let total = 0;
                cart.forEach(item => {
                    const subtotal = item.precio * item.cantidad;
                    total += subtotal;
                    mensaje += `✅ ${item.nombre}  x  ${item.cantidad}  =  $${subtotal.toFixed(2)}%0A`;
                });
                mensaje += `%0A━━━━━━━━━━━━━━━━━━━━━━%0A`;
                mensaje += `💰 TOTAL: $${total.toFixed(2)}%0A`;
                mensaje += `━━━━━━━━━━━━━━━━━━━━━━%0A%0A`;
                mensaje += `📍 ¿Cómo puedo pagar? (Yape, Plin, Transferencia)%0A`;
                mensaje += `📦 ¿Tienes stock disponible?%0A`;
                mensaje += `🚚 ¿El envío es a todo Perú?%0A%0A`;
                mensaje += `💖 ¡Gracias! Espero tu respuesta.`;

                const phone = '51923861016';
                const url = `https://wa.me/${phone}?text=${mensaje}`;
                window.open(url, '_blank');

                cart = [];
                actualizarContador();
                renderCart();
                cartModal.classList.remove('show');
                document.body.style.overflow = '';
                mostrarNotificacion('✅ Pedido enviado por WhatsApp', '📨');
            });
        }


        // ============================================
        // CONTACTO
        // ============================================

        function iniciarContacto() {
            const form = document.getElementById('contactForm');
            if (!form) return;
            form.addEventListener('submit', function(e) {
                e.preventDefault();
                const nombre = document.getElementById('nombre').value;
                const email = document.getElementById('email').value;
                const mensaje = document.getElementById('mensaje').value;

                const whatsappMessage =
                    `✨ Hola Paulina ✨%0A%0A👤 Soy ${nombre}%0A📧 Mi correo es: ${email}%0A%0A📩 Mensaje:%0A${mensaje}%0A%0A📍 ¿Podrías darme más información sobre tu catálogo y precios?`;

                const phone = '51923861016';
                const url = `https://wa.me/${phone}?text=${whatsappMessage}`;
                window.open(url, '_blank');
                mostrarNotificacion('✅ Mensaje enviado por WhatsApp', '📨');
                this.reset();
            });
        }


        // ============================================
        // FAQ
        // ============================================

        function iniciarFAQ() {
            document.querySelectorAll('.faq-item').forEach(item => {
                item.addEventListener('click', function() {
                    this.classList.toggle('open');
                });
            });
        }


        // ============================================
        // NEWSLETTER
        // ============================================

        function iniciarNewsletter() {
            const form = document.getElementById('newsletterForm');
            if (!form) return;
            form.addEventListener('submit', function(e) {
                e.preventDefault();
                const email = this.querySelector('input').value;
                mostrarNotificacion(`✅ ${email} suscrito con éxito`, '📧');
                this.reset();
            });
        }


        // ============================================
        // POP-UP
        // ============================================

        function iniciarPopup() {
            const overlay = document.getElementById('popupOferta');
            const closeBtn = document.getElementById('popupClose');
            const form = document.getElementById('popupForm');

            const yaVisto = sessionStorage.getItem('popupVisto');
            if (!yaVisto) {
                setTimeout(() => {
                    overlay.classList.add('show');
                    document.body.style.overflow = 'hidden';
                }, 8000);
            }

            closeBtn.addEventListener('click', () => {
                overlay.classList.remove('show');
                document.body.style.overflow = '';
                sessionStorage.setItem('popupVisto', 'true');
            });

            overlay.addEventListener('click', (e) => {
                if (e.target === overlay) {
                    overlay.classList.remove('show');
                    document.body.style.overflow = '';
                    sessionStorage.setItem('popupVisto', 'true');
                }
            });

            form.addEventListener('submit', function(e) {
                e.preventDefault();
                const email = this.querySelector('input').value;
                mostrarNotificacion(`✅ ${email} - ¡Descuento aplicado! Revisa tu correo.`, '🎉');
                overlay.classList.remove('show');
                document.body.style.overflow = '';
                sessionStorage.setItem('popupVisto', 'true');
                this.reset();
            });
        }


        // ============================================
        // MODO OSCURO
        // ============================================

        function iniciarModoOscuro() {
            const btn = document.getElementById('darkModeToggle');
            if (!btn) return;

            const modo = localStorage.getItem('modoOscuro') || 'false';
            if (modo === 'true') {
                document.body.classList.add('dark-mode');
                btn.textContent = '☀️';
            }

            btn.addEventListener('click', () => {
                document.body.classList.toggle('dark-mode');
                const isDark = document.body.classList.contains('dark-mode');
                btn.textContent = isDark ? '☀️' : '🌙';
                localStorage.setItem('modoOscuro', isDark);
            });
        }


        // ============================================
        // COMPARTIR
        // ============================================

        function iniciarCompartir() {
            const btn = document.getElementById('shareBtn');
            if (!btn) return;
            btn.addEventListener('click', () => {
                if (navigator.share) {
                    navigator.share({
                        title: 'Paulina Accesorios ✨',
                        text: 'Descubre los mejores accesorios de belleza en Paulina Accesorios. Envíos a todo Perú 🇵🇪',
                        url: window.location.href
                    }).catch(() => {});
                } else {
                    navigator.clipboard.writeText(window.location.href).then(() => {
                        mostrarNotificacion('✅ Enlace copiado al portapapeles', '📤');
                    }).catch(() => {
                        mostrarNotificacion('📤 Comparte: ' + window.location.href, '📤');
                    });
                }
            });
        }


        // ============================================
        // CONTADOR DE VISITAS
        // ============================================

        function iniciarContadorVisitas() {
            visitCount++;
            localStorage.setItem('visitas', visitCount);
            const el = document.getElementById('visitCount');
            if (el) el.textContent = visitCount;
        }


        // ============================================
        // BACK TO TOP
        // ============================================

        function iniciarBackTop() {
            const btn = document.getElementById('backTopBtn');
            if (!btn) return;
            window.addEventListener('scroll', () => {
                if (window.scrollY > 500) {
                    btn.style.display = 'flex';
                } else {
                    btn.style.display = 'none';
                }
            });
            btn.addEventListener('click', () => {
                window.scrollTo({ top: 0, behavior: 'smooth' });
            });
        }


        // ============================================
        // MENÚ HAMBURGUESA
        // ============================================

        function iniciarMenuHamburguesa() {
            const hamburger = document.getElementById('hamburger');
            const menu = document.getElementById('mobileMenu');
            const closeBtn = document.getElementById('mobileClose');

            hamburger.addEventListener('click', () => {
                hamburger.classList.toggle('active');
                menu.classList.toggle('open');
                document.body.style.overflow = menu.classList.contains('open') ? 'hidden' : '';
            });

            closeBtn.addEventListener('click', () => {
                hamburger.classList.remove('active');
                menu.classList.remove('open');
                document.body.style.overflow = '';
            });

            menu.querySelectorAll('a').forEach(link => {
                link.addEventListener('click', () => {
                    hamburger.classList.remove('active');
                    menu.classList.remove('open');
                    document.body.style.overflow = '';
                });
            });
        }


        // ============================================
        // PRELOADER
        // ============================================

        function iniciarPreloader() {
            const preloader = document.getElementById('preloader');
            window.addEventListener('load', () => {
                setTimeout(() => {
                    preloader.classList.add('hidden');
                }, 1000);
            });
        }


        // ============================================
        // INICIALIZAR TODO
        // ============================================

        document.addEventListener('DOMContentLoaded', function() {
            const masVendidos = productos.filter(p => masVendidosIds.includes(p.id));
            renderizarProductos('masVendidos', masVendidos);
            renderizarProductos('productGrid', productos);
            renderizarTestimonios();
            renderizarTips();

            iniciarCarousel();
            iniciarContadorVisitas();
            iniciarModoOscuro();
            iniciarCompartir();
            iniciarSlider();
            iniciarTimer('horas', 'minutos', 'segundos', 24);
            iniciarTimer('flashHoras', 'flashMinutos', 'flashSegundos', 2);
            iniciarTimer('popupHoras', 'popupMinutos', 'popupSegundos', 2);
            iniciarPopup();
            iniciarFiltro();
            iniciarFiltroPrecio();
            iniciarOrdenar();
            iniciarCarrito();
            iniciarContacto();
            iniciarNewsletter();
            iniciarBackTop();
            iniciarBuscador();
            iniciarMenuHamburguesa();
            iniciarFAQ();
            iniciarNotificacionesVivo();
            iniciarPreloader();

            console.log('✨ Paulina Accesorios - Versión Final con Íconos Reales ✨');
            console.log(`📦 ${productos.length} productos cargados`);
            console.log(`👀 ${visitCount} visitas totales`);
            console.log('📱 Redes: Instagram, TikTok, Facebook, WhatsApp');
            console.log('🎨 Íconos corregidos y visibles');
        });
    </script>

</body>
</html>
