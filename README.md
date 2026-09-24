    body {
        position: relative;
        background-color: #ffffff;
        color: #1e293b;
        line-height: 1.6;
        min-height: 100vh;
        overflow-x: hidden;
    }

    a {
        color: inherit;
        text-decoration: none;
    }

    /* LATAR BELAKANG FOTO (FULLPAGE & TANPA BLUR) */
    .global-image-bg {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        z-index: -2;
        object-fit: cover;
        /* Memastikan foto jernih dan bebas dari efek blur */
        filter: none !important;
        -webkit-filter: none !important;
    }

    /* OVERLAY TRANSPARAN PUTIH (UNTUK KETERBACAAN TEKS) */
    .global-overlay {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(255, 255, 255, 0.70);
        z-index: -1;
    }

    /* GELEMBUNG BANYAK & DIAM (STATIONARY BUBBLES) */
    .bubbles-container {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        z-index: 0;
        pointer-events: none;
        overflow: hidden;
    }

    .bubble {
        position: absolute;
        border-radius: 50%;
    }

    .bubble-white {
        background: rgba(255, 255, 255, 0.5);
        border: 2px solid rgba(255, 255, 255, 0.95);
        box-shadow: 0 0 12px rgba(255, 255, 255, 0.6);
    }

    .bubble-black {
        background: rgba(15, 23, 42, 0.15);
        border: 2px solid rgba(15, 23, 42, 0.35);
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.12);
    }

    /* POSISI DIAM 16 GELEMBUNG */
    .b1  { top: 5%;   left: 8%;  width: 50px; height: 50px; }
    .b2  { top: 12%;  left: 82%; width: 30px; height: 30px; }
    .b3  { top: 22%;  left: 25%; width: 70px; height: 70px; }
    .b4  { top: 18%;  left: 65%; width: 40px; height: 40px; }
    .b5  { top: 35%;  left: 12%; width: 60px; height: 60px; }
    .b6  { top: 38%;  left: 88%; width: 45px; height: 45px; }
    .b7  { top: 48%;  left: 48%; width: 80px; height: 80px; }
    .b8  { top: 52%;  left: 5%;  width: 35px; height: 35px; }
    .b9  { top: 62%;  left: 78%; width: 65px; height: 65px; }
    .b10 { top: 68%;  left: 20%; width: 40px; height: 40px; }
    .b11 { top: 78%;  left: 88%; width: 55px; height: 55px; }
    .b12 { top: 82%;  left: 10%; width: 75px; height: 75px; }
    .b13 { top: 88%;  left: 60%; width: 35px; height: 35px; }
    .b14 { top: 92%;  left: 35%; width: 50px; height: 50px; }
    .b15 { top: 28%;  left: 92%; width: 25px; height: 25px; }
    .b16 { top: 74%;  left: 45%; width: 30px; height: 30px; }

    /* CONTENT WRAPPER */
    .main-wrapper {
        position: relative;
        z-index: 1;
    }

    /* HEADER BERGABUNG MENYATU (LOGO, MENU, TOMBOL & HERO SLOGAN) */
    .header-combined {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 2rem 10% 4rem;
        text-align: center;
        background: transparent;
    }

    .logo {
        font-size: 2.2rem;
        font-weight: 800;
        color: #0284c7;
        margin-bottom: 1.5rem;
    }

    .nav-links {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        list-style: none;
        gap: 1.5rem;
        font-weight: 600;
        font-size: 1.1rem;
        margin-bottom: 2rem;
    }

    .nav-links a:hover {
        color: #0284c7;
        transition: 0.3s;
    }

    .btn-contact {
        background-color: #0284c7;
        color: #ffffff;
        padding: 0.8rem 2rem;
        border-radius: 8px;
        font-weight: bold;
        font-size: 1.05rem;
        display: inline-block;
        box-shadow: 0 4px 10px rgba(2, 132, 199, 0.2);
    }

    .btn-contact:hover {
        background-color: #0369a1;
        transition: 0.3s;
    }

    .hero-text {
        margin-top: 3rem;
        max-width: 800px;
    }

    .hero-text h1 {
        font-size: 2.8rem;
        margin-bottom: 1rem;
        color: #0f172a;
        font-weight: 800;
    }

    .hero-text h1 span {
        color: #0284c7;
    }

    .hero-text p {
        color: #334155;
        max-width: 650px;
        margin: 0 auto;
        font-size: 1.15rem;
        font-weight: 500;
    }

    /* ABOUT SECTION */
    .about {
        padding: 3rem 10%;
        text-align: center;
    }

    .about-content {
        max-width: 800px;
        margin: 0 auto;
        color: #334155;
        font-size: 1.05rem;
        line-height: 1.8;
        background: rgba(255, 255, 255, 0.80);
        padding: 2rem;
        border-radius: 12px;
        border: 1px solid rgba(226, 232, 240, 0.9);
    }

    /* SERVICES SECTION */
    .services {
        padding: 4rem 10%;
        text-align: center;
    }

    .section-title {
        font-size: 2rem;
        margin-bottom: 2.5rem;
        color: #0f172a;
        position: relative;
    }

    .section-title::after {
        content: '';
        width: 50px;
        height: 3px;
        background-color: #0284c7;
        display: block;
        margin: 0.5rem auto 0;
        border-radius: 2px;
    }

    .grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
        gap: 2rem;
    }

    .card {
        background-color: rgba(255, 255, 255, 0.88);
        padding: 2rem;
        border-radius: 12px;
        border: 1px solid #e2e8f0;
        box-shadow: 0 4px 12px rgba(0, 0, 0, 0.04);
        transition: transform 0.3s, box-shadow 0.3s, border-color 0.3s;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }

    .card:hover {
        transform: translateY(-5px);
        box-shadow: 0 10px 20px rgba(0, 0, 0, 0.08);
        border-color: #0284c7;
    }

    .card h3 {
        font-size: 1.4rem;
        margin-bottom: 0.8rem;
        color: #0f172a;
    }

    .price {
        font-size: 1.8rem;
        color: #0284c7;
        font-weight: bold;
        margin: 1rem 0;
    }

    .card ul {
        list-style: none;
        text-align: left;
        margin-bottom: 2rem;
        color: #475569;
    }

    .card ul li {
        margin-bottom: 0.6rem;
    }

    .card ul li::before {
        content: "✓ ";
        color: #0284c7;
        font-weight: bold;
    }

    .btn-buy {
        display: block;
        background-color: #16a34a;
        color: #ffffff;
        padding: 0.7rem;
        border-radius: 6px;
        font-weight: bold;
        text-align: center;
    }

    .btn-buy:hover {
        background-color: #15803d;
        transition: 0.3s;
    }

    /* FOOTER */
    footer {
        background-color: rgba(255, 255, 255, 0.95);
        text-align: center;
        padding: 2rem;
        margin-top: 2rem;
        border-top: 1px solid #e2e8f0;
        color: #64748b;
        font-size: 0.9rem;
    }

    /* RESPONSIVE DESIGN UNTUK PERANGKAT MOBILE */
    @media (max-width: 768px) {
        .nav-links {
            gap: 1rem;
            font-size: 0.95rem;
        }
        .hero-text h1 {
            font-size: 2rem;
        }
    }
</style>
