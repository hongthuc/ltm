<!-- Website: ltm.com - CÔNG TY TNHH THƯƠNG MẠI VÀ DỊCH VỤ L.T.M -->
<!-- Cấu trúc chuẩn Flatsome UX Builder (Section > Row > Col > Box) dễ dàng thiết kế lại -->
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0">
    <title>LTM.COM - Công Ty TNHH Thương Mại Và Dịch Vụ L.T.M | Gạch Ốp Lát & Thiết Bị Nhà Tắm Cao Cấp Đà Nẵng</title>
    <meta name="description" content="CÔNG TY TNHH THƯƠNG MẠI VÀ DỊCH VỤ L.T.M (ltm.com) chuyên phân phối Gạch ốp lát cao cấp Đà Nẵng: gạch men, gạch hoa, gạch gỗ, gạch khổ lớn, gạch trang trí cao cấp, thiết bị nhà tắm nhập khẩu. Địa chỉ: 28 Lương Trúc Đàm, Thanh Khê, Đà Nẵng. Hotline: 0914.191.825.">

    <!-- Open Graph / Thumbnail là ảnh Logo khi gửi link trang web -->
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://ltm.com/">
    <meta property="og:site_name" content="ltm.com - CÔNG TY TNHH THƯƠNG MẠI VÀ DỊCH VỤ L.T.M">
    <meta property="og:title" content="CÔNG TY TNHH THƯƠNG MẠI VÀ DỊCH VỤ L.T.M - Gạch Ốp Lát Cao Cấp Đà Nẵng">
    <meta property="og:description" content="Chuyên gạch men, gạch hoa, gạch gỗ, gạch trang trí cao cấp và thiết bị nhà tắm nhập khẩu tại 28 Lương Trúc Đàm, Thanh Khê, Đà Nẵng. ĐT: 0914.191.825">
    <meta property="og:image" content="https://lh3.googleusercontent.com/d/1657a_RNzOWwdZGeDnC2P_1sW2SUH5Jia">
    <meta property="og:image:alt" content="Logo CÔNG TY TNHH THƯƠNG MẠI VÀ DỊCH VỤ L.T.M">
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:image" content="https://lh3.googleusercontent.com/d/1657a_RNzOWwdZGeDnC2P_1sW2SUH5Jia">
    <link rel="icon" href="https://lh3.googleusercontent.com/d/1657a_RNzOWwdZGeDnC2P_1sW2SUH5Jia">

    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>

    <!-- Google Fonts: Inter & Montserrat chuẩn Flatsome -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">

    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        ltm: {
                            primary: '#12355b',    /* Màu xanh đậm sang trọng đồng bộ tông thương hiệu */
                            secondary: '#1d4e89',  /* Xanh thương hiệu phụ */
                            gold: '#c58b2b',       /* Vàng đồng điểm nhấn */
                            sale: '#d26e4b',       /* Màu đỏ cam giảm giá chuẩn Flatsome */
                            light: '#f7f8fa'
                        }
                    }
                }
            }
        }
    </script>

    <style>
        /* Chống tràn viền và chống lệch phải tuyệt đối trên mọi thiết bị */
        *, *::before, *::after {
            box-sizing: border-box;
        }
        html, body {
            width: 100%;
            max-width: 100%;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc;
            color: #1e293b;
            scroll-behavior: smooth;
        }

        /* Khung giao diện chuẩn: 95% trên máy tính, căn giữa tuyệt đối */
        .flatsome-container {
            width: 96%;
            max-width: 96%;
            margin-left: auto;
            margin-right: auto;
        }
        @media (min-width: 1024px) {
            .flatsome-container {
                width: 95%;
                max-width: 95%;
                margin-left: auto;
                margin-right: auto;
            }
        }

        /* Tối ưu tên danh mục trên máy tính: viết liền trên 1 hàng, chữ nhỏ gọn, không xuống dòng trong từng tên danh mục */
        .desktop-cat-nav {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: center;
            gap: 2px 6px;
        }
        .desktop-cat-item {
            white-space: nowrap;
            font-size: 12px;
            font-weight: 600;
            letter-spacing: 0.01em;
            padding: 7px 9px;
            line-height: 1.2;
            transition: all 0.2s ease;
        }
        @media (min-width: 1280px) {
            .desktop-cat-item {
                font-size: 12.5px;
                padding: 8px 11px;
            }
        }

        /* Dropdown menu chuẩn Flatsome */
        .cat-dropdown-parent:hover .cat-dropdown-menu {
            opacity: 1;
            visibility: visible;
            transform: translateY(0);
        }
        .cat-dropdown-menu {
            opacity: 0;
            visibility: hidden;
            transform: translateY(6px);
            transition: all 0.2s ease;
            z-index: 60;
        }

        /* Tiêu đề Section chuẩn Flatsome (Section Title Container) */
        .section-title-container {
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-bottom: 2px solid #e2e8f0;
            margin-bottom: 1rem;
            padding-bottom: 0.5rem;
            flex-wrap: wrap;
            gap: 0.5rem;
        }
        .section-title-main {
            position: relative;
            font-weight: 800;
            text-transform: uppercase;
            color: #12355b;
            letter-spacing: 0.02em;
        }
        .section-title-main::after {
            content: '';
            position: absolute;
            bottom: -0.6rem;
            left: 0;
            width: 100%;
            height: 3px;
            background-color: #c58b2b;
        }

        /* Badge % giảm giá góc trên bên trái chuẩn Flatsome */
        .badge-circle-sale {
            position: absolute;
            top: 8px;
            left: 8px;
            z-index: 10;
            background-color: #d26e4b;
            color: #ffffff;
            font-weight: 700;
            font-size: 11px;
            line-height: 1;
            padding: 6px 8px;
            border-radius: 9999px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.18);
        }

        /* Đảm bảo tên sản phẩm hiển thị đầy đủ, không bị tràn hoặc cắt mất chữ */
        .product-title-text {
            word-break: break-word;
            overflow-wrap: break-word;
            white-space: normal;
            line-height: 1.38;
        }

        /* Thanh cuộn ngang mượt cho danh mục trên điện thoại */
        .no-scrollbar::-webkit-scrollbar {
            display: none;
        }
        .no-scrollbar {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }

        /* Hiệu ứng rung nhẹ cho nút liên hệ nổi */
        @keyframes pulse-ring {
            0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(18, 53, 91, 0.5); }
            70% { transform: scale(1); box-shadow: 0 0 0 8px rgba(18, 53, 91, 0); }
            100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(18, 53, 91, 0); }
        }
        .contact-pulse {
            animation: pulse-ring 2.2s infinite;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 antialiased selection:bg-ltm-primary selection:text-white">

    <!-- ==================== 1. TOP BAR (UX BUILDER FLATSOME TOP BAR) ==================== -->
    <div class="bg-ltm-primary text-white text-xs border-b border-white/10">
        <div class="flatsome-container py-2 flex flex-col sm:flex-row items-center justify-between gap-1.5 text-center sm:text-left">
            <div class="flex flex-wrap items-center justify-center sm:justify-start gap-x-4 gap-y-1">
                <span class="font-semibold tracking-wide text-amber-300">
                    <i class="fa-solid fa-building mr-1"></i>CÔNG TY TNHH THƯƠNG MẠI VÀ DỊCH VỤ L.T.M (ltm.com)
                </span>
                <span class="hidden md:inline text-white/40">|</span>
                <span class="text-slate-100">
                    <i class="fa-solid fa-location-dot text-amber-400 mr-1"></i>28 Lương Trúc Đàm, Thanh Khê, Đà Nẵng
                </span>
            </div>
            <div class="flex items-center justify-center gap-4 text-[11px] sm:text-xs">
                <a href="https://share.google/9qG3KQ5P8u1OBtSPS" target="_blank" rel="noopener noreferrer" class="hover:text-amber-300 transition flex items-center gap-1">
                    <i class="fa-solid fa-map-location-dot text-amber-400"></i> Chỉ đường Google Maps
                </a>
                <span class="text-white/30">|</span>
                <a href="https://www.facebook.com/profile.php?id=100046135087441" target="_blank" rel="noopener noreferrer" class="hover:text-amber-300 transition flex items-center gap-1">
                    <i class="fa-brands fa-facebook text-amber-400"></i> Fanpage L.T.M
                </a>
            </div>
        </div>
    </div>

    <!-- ==================== 2. HEADER (KHÔNG ĐỂ NÚT GỌI NGAY ĐỂ TRÁNH TRÀN VIỀN) ==================== -->
    <header id="header" class="bg-white sticky top-0 z-50 shadow-sm border-b border-slate-200">
        <!-- Header Main -->
        <div class="flatsome-container py-2.5 md:py-3 flex items-center justify-between gap-3">
            <!-- Nút mở menu danh mục trên điện thoại -->
            <button id="mobileMenuBtn" type="button" aria-label="Mở danh mục" class="lg:hidden p-2 rounded-lg border border-slate-200 text-ltm-primary hover:bg-slate-100 transition shrink-0">
                <i class="fa-solid fa-bars text-lg"></i>
            </button>

            <!-- Logo gọn nhỏ + Tên thương hiệu -->
            <a href="#top" class="flex items-center gap-2.5 min-w-0 shrink">
                <div class="w-10 h-10 sm:w-11 sm:h-11 rounded-lg bg-white border border-slate-200 p-1 flex items-center justify-center shrink-0 overflow-hidden shadow-xs">
                    <img 
                        src="https://lh3.googleusercontent.com/d/1657a_RNzOWwdZGeDnC2P_1sW2SUH5Jia" 
                        onerror="if(!this.dataset.t1){this.dataset.t1='1';this.src='https://drive.google.com/thumbnail?id=1657a_RNzOWwdZGeDnC2P_1sW2SUH5Jia&sz=w400';}else{this.onerror=null;this.src='https://placehold.co/120x120/12355b/ffffff?text=LTM';}"
                        alt="Logo Công Ty TNHH TM & DV L.T.M" 
                        class="w-full h-full object-contain"
                    >
                </div>
                <div class="min-w-0">
                    <div class="text-xs sm:text-sm md:text-base font-extrabold text-ltm-primary leading-tight truncate">
                        CÔNG TY TNHH TM & DV L.T.M
                    </div>
                    <div class="text-[11px] sm:text-xs text-slate-500 font-medium truncate">
                        ltm.com • Gạch Ốp Lát & Thiết Bị Nhà Tắm Đà Nẵng
                    </div>
                </div>
            </a>

            <!-- Ô tìm kiếm sản phẩm trên máy tính (Chuẩn Flatsome) -->
            <div class="hidden md:flex flex-1 max-w-md mx-2">
                <div class="relative w-full">
                    <input 
                        id="desktopSearchInput" 
                        type="text" 
                        placeholder="Tìm gạch 60x120, gạch 80x80, gạch gỗ, gạch hoa, thiết bị nhà tắm..." 
                        class="w-full pl-3.5 pr-10 py-2 text-xs lg:text-sm bg-slate-100 border border-slate-300 rounded-full focus:outline-none focus:border-ltm-primary focus:bg-white transition"
                    >
                    <button id="desktopSearchBtn" type="button" aria-label="Tìm kiếm" class="absolute right-1.5 top-1/2 -translate-y-1/2 w-7 h-7 rounded-full bg-ltm-primary text-white flex items-center justify-center hover:bg-ltm-secondary transition">
                        <i class="fa-solid fa-magnifying-glass text-xs"></i>
                    </button>
                </div>
            </div>

            <!-- Liên kết nhanh bên phải (Không để nút gọi ngay tránh tràn viền) -->
            <div class="flex items-center gap-2 shrink-0">
                <a href="#bao-gia" class="text-xs font-semibold px-3 py-2 rounded-lg bg-amber-500/15 text-ltm-primary border border-amber-500/30 hover:bg-amber-500 hover:text-white transition whitespace-nowrap">
                    <i class="fa-solid fa-file-invoice mr-1"></i>Báo giá
                </a>
                <a href="#ban-do" class="hidden sm:inline-flex text-xs font-semibold px-3 py-2 rounded-lg bg-slate-100 text-slate-700 hover:bg-ltm-primary hover:text-white transition whitespace-nowrap">
                    <i class="fa-solid fa-location-dot mr-1 text-ltm-gold"></i>Showroom
                </a>
            </div>
        </div>

        <!-- Thanh tìm kiếm gọn trên điện thoại -->
        <div class="md:hidden flatsome-container pb-2">
            <div class="relative w-full">
                <input 
                    id="mobileSearchInput" 
                    type="text" 
                    placeholder="Tìm kiếm gạch men, gạch hoa, gạch gỗ, thiết bị tắm..." 
                    class="w-full pl-3.5 pr-9 py-1.5 text-xs bg-slate-100 border border-slate-300 rounded-full focus:outline-none focus:border-ltm-primary focus:bg-white"
                >
                <button id="mobileSearchBtn" type="button" aria-label="Tìm kiếm" class="absolute right-1.5 top-1/2 -translate-y-1/2 w-6 h-6 rounded-full bg-ltm-primary text-white flex items-center justify-center">
                    <i class="fa-solid fa-magnifying-glass text-[10px]"></i>
                </button>
            </div>
        </div>

        <!-- Thanh Menu Danh Mục Sản Phẩm trên Máy Tính (Viết liền trên 1 hàng chữ nhỏ gọn, không tự xuống dòng từng mục) -->
        <nav class="hidden lg:block bg-ltm-primary text-white border-t border-white/10">
            <div class="flatsome-container">
                <ul class="desktop-cat-nav py-0.5">
                    <li>
                        <a href="#top" data-filter="all" class="filter-trigger desktop-cat-item inline-flex items-center gap-1 rounded text-amber-300 hover:bg-white/10">
                            <i class="fa-solid fa-house text-[11px]"></i> TRANG CHỦ
                        </a>
                    </li>
                    <li class="relative cat-dropdown-parent">
                        <a href="#san-pham-all" data-filter="gach-lat-nen" class="filter-trigger desktop-cat-item inline-flex items-center gap-1 rounded hover:bg-white/10 hover:text-amber-300">
                            GẠCH LÁT NỀN <i class="fa-solid fa-chevron-down text-[9px] opacity-75"></i>
                        </a>
                        <div class="cat-dropdown-menu absolute left-0 top-full w-48 bg-white text-slate-800 rounded-b-lg shadow-xl border border-slate-200 py-1.5 text-xs">
                            <a href="#san-pham-all" data-filter="gach-lat-nen" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Lát Nền 60x60</a>
                            <a href="#san-pham-all" data-filter="gach-lat-nen" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Lát Nền 80x80</a>
                            <a href="#san-pham-all" data-filter="gach-lat-nen" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Lát Nền 100x100</a>
                            <a href="#san-pham-all" data-filter="gach-lat-nen" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Lát Nền 120x120</a>
                        </div>
                    </li>
                    <li class="relative cat-dropdown-parent">
                        <a href="#san-pham-all" data-filter="gach-op-tuong" class="filter-trigger desktop-cat-item inline-flex items-center gap-1 rounded hover:bg-white/10 hover:text-amber-300">
                            GẠCH ỐP TƯỜNG <i class="fa-solid fa-chevron-down text-[9px] opacity-75"></i>
                        </a>
                        <div class="cat-dropdown-menu absolute left-0 top-full w-48 bg-white text-slate-800 rounded-b-lg shadow-xl border border-slate-200 py-1.5 text-xs">
                            <a href="#san-pham-all" data-filter="gach-op-tuong" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Ốp Tường 30x60</a>
                            <a href="#san-pham-all" data-filter="gach-op-tuong" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Ốp Tường 60x120</a>
                            <a href="#san-pham-all" data-filter="gach-op-tuong" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Ốp Tường 80x160</a>
                            <a href="#san-pham-all" data-filter="gach-op-tuong" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Ốp Tường 75x150</a>
                            <a href="#san-pham-all" data-filter="gach-op-tuong" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Ốp Tường 90x180</a>
                        </div>
                    </li>
                    <li class="relative cat-dropdown-parent">
                        <a href="#san-pham-all" data-filter="gach-kho-lon" class="filter-trigger desktop-cat-item inline-flex items-center gap-1 rounded hover:bg-white/10 hover:text-amber-300">
                            GẠCH KHỔ LỚN <i class="fa-solid fa-chevron-down text-[9px] opacity-75"></i>
                        </a>
                        <div class="cat-dropdown-menu absolute left-0 top-full w-52 bg-white text-slate-800 rounded-b-lg shadow-xl border border-slate-200 py-1.5 text-xs">
                            <a href="#san-pham-all" data-filter="gach-kho-lon" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Khổ Lớn 1600x3200</a>
                            <a href="#san-pham-all" data-filter="gach-kho-lon" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Khổ Lớn 1200x2400</a>
                            <a href="#san-pham-all" data-filter="gach-kho-lon" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Khổ Lớn 1200x2800</a>
                            <a href="#san-pham-all" data-filter="gach-kho-lon" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Khổ Lớn 1200x1800</a>
                        </div>
                    </li>
                    <li class="relative cat-dropdown-parent">
                        <a href="#san-pham-all" data-filter="gach-trang-tri" class="filter-trigger desktop-cat-item inline-flex items-center gap-1 rounded hover:bg-white/10 hover:text-amber-300">
                            GẠCH TRANG TRÍ <i class="fa-solid fa-chevron-down text-[9px] opacity-75"></i>
                        </a>
                        <div class="cat-dropdown-menu absolute left-0 top-full w-48 bg-white text-slate-800 rounded-b-lg shadow-xl border border-slate-200 py-1.5 text-xs">
                            <a href="#san-pham-all" data-filter="gach-trang-tri" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Hoa / Gạch Bông</a>
                            <a href="#san-pham-all" data-filter="gach-trang-tri" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Terrazzo Cao Cấp</a>
                            <a href="#san-pham-all" data-filter="gach-trang-tri" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Gạch Mosaic Nghệ Thuật</a>
                        </div>
                    </li>
                    <li>
                        <a href="#san-pham-all" data-filter="gach-go" class="filter-trigger desktop-cat-item inline-flex items-center gap-1 rounded hover:bg-white/10 hover:text-amber-300">
                            GẠCH VÂN GỖ
                        </a>
                    </li>
                    <li class="relative cat-dropdown-parent">
                        <a href="#san-pham-all" data-filter="thiet-bi-nha-tam" class="filter-trigger desktop-cat-item inline-flex items-center gap-1 rounded hover:bg-white/10 hover:text-amber-300">
                            THIẾT BỊ VỆ SINH <i class="fa-solid fa-chevron-down text-[9px] opacity-75"></i>
                        </a>
                        <div class="cat-dropdown-menu absolute right-0 top-full w-52 bg-white text-slate-800 rounded-b-lg shadow-xl border border-slate-200 py-1.5 text-xs">
                            <a href="#san-pham-all" data-filter="thiet-bi-nha-tam" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Tủ Lavabo Nhập Khẩu</a>
                            <a href="#san-pham-all" data-filter="thiet-bi-nha-tam" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Bồn Cầu Thông Minh & 1 Khối</a>
                            <a href="#san-pham-all" data-filter="thiet-bi-nha-tam" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Sen Cây Tắm & Vòi Lavabo</a>
                            <a href="#san-pham-all" data-filter="thiet-bi-nha-tam" class="filter-trigger block px-3.5 py-2 hover:bg-slate-100 hover:text-ltm-primary font-medium whitespace-nowrap">Bồn Tắm & Phụ Kiện Nhà Tắm</a>
                        </div>
                    </li>
                    <li>
                        <a href="#doi-tac" class="desktop-cat-item inline-flex items-center rounded hover:bg-white/10 hover:text-amber-300">
                            ĐỐI TÁC
                        </a>
                    </li>
                    <li>
                        <a href="#bai-viet" class="desktop-cat-item inline-flex items-center rounded hover:bg-white/10 hover:text-amber-300">
                            TIN TỨC
                        </a>
                    </li>
                    <li>
                        <a href="#bao-gia" class="desktop-cat-item inline-flex items-center rounded hover:bg-white/10 hover:text-amber-300">
                            BÁO GIÁ
                        </a>
                    </li>
                    <li>
                        <a href="#lien-he" class="desktop-cat-item inline-flex items-center rounded hover:bg-white/10 hover:text-amber-300">
                            LIÊN HỆ
                        </a>
                    </li>
                </ul>
            </div>
        </nav>

        <!-- Thanh Danh Mục Ngang Gọn Đẹp Trên Điện Thoại & Máy Tính Bảng -->
        <div class="lg:hidden bg-ltm-primary text-white border-t border-white/10">
            <div class="flatsome-container py-1.5 flex items-center gap-1.5 overflow-x-auto no-scrollbar">
                <button type="button" data-filter="all" class="filter-trigger whitespace-nowrap text-[11px] font-semibold px-2.5 py-1 rounded bg-amber-500 text-white shrink-0">
                    Tất cả
                </button>
                <button type="button" data-filter="gach-lat-nen" class="filter-trigger whitespace-nowrap text-[11px] font-semibold px-2.5 py-1 rounded bg-white/10 hover:bg-white/20 shrink-0">
                    Gạch Lát Nền
                </button>
                <button type="button" data-filter="gach-op-tuong" class="filter-trigger whitespace-nowrap text-[11px] font-semibold px-2.5 py-1 rounded bg-white/10 hover:bg-white/20 shrink-0">
                    Gạch Ốp Tường
                </button>
                <button type="button" data-filter="gach-kho-lon" class="filter-trigger whitespace-nowrap text-[11px] font-semibold px-2.5 py-1 rounded bg-white/10 hover:bg-white/20 shrink-0">
                    Gạch Khổ Lớn
                </button>
                <button type="button" data-filter="gach-trang-tri" class="filter-trigger whitespace-nowrap text-[11px] font-semibold px-2.5 py-1 rounded bg-white/10 hover:bg-white/20 shrink-0">
                    Gạch Hoa & Trang Trí
                </button>
                <button type="button" data-filter="gach-go" class="filter-trigger whitespace-nowrap text-[11px] font-semibold px-2.5 py-1 rounded bg-white/10 hover:bg-white/20 shrink-0">
                    Gạch Vân Gỗ
                </button>
                <button type="button" data-filter="thiet-bi-nha-tam" class="filter-trigger whitespace-nowrap text-[11px] font-semibold px-2.5 py-1 rounded bg-white/10 hover:bg-white/20 shrink-0">
                    Thiết Bị Nhà Tắm
                </button>
            </div>
        </div>
    </header>

    <!-- Menu Drawer Danh Mục Trên Điện Thoại -->
    <div id="mobileDrawer" class="fixed inset-0 z-50 hidden">
        <div id="mobileDrawerOverlay" class="absolute inset-0 bg-slate-900/60 backdrop-blur-xs"></div>
        <div class="relative w-72 max-w-[85vw] h-full bg-white shadow-2xl flex flex-col justify-between overflow-y-auto">
            <div>
                <div class="p-4 bg-ltm-primary text-white flex items-center justify-between">
                    <div class="flex items-center gap-2">
                        <img 
                            src="https://lh3.googleusercontent.com/d/1657a_RNzOWwdZGeDnC2P_1sW2SUH5Jia" 
                            onerror="this.src='https://placehold.co/80x80/12355b/ffffff?text=LTM'"
                            alt="Logo L.T.M" 
                            class="w-8 h-8 rounded bg-white p-0.5 object-contain"
                        >
                        <span class="font-bold text-sm">DANH MỤC LTM.COM</span>
                    </div>
                    <button id="closeMobileDrawer" type="button" class="w-8 h-8 rounded-full bg-white/10 flex items-center justify-center text-white">
                        <i class="fa-solid fa-xmark"></i>
                    </button>
                </div>
                <div class="p-3 divide-y divide-slate-100 text-xs font-semibold text-slate-700">
                    <a href="#san-pham-all" data-filter="all" class="mobile-nav-link filter-trigger flex items-center justify-between py-2.5 px-2 rounded hover:bg-slate-100">
                        <span><i class="fa-solid fa-border-all w-5 text-ltm-primary"></i> Tất Cả Sản Phẩm</span>
                        <i class="fa-solid fa-angle-right text-slate-400"></i>
                    </a>
                    <a href="#san-pham-all" data-filter="gach-lat-nen" class="mobile-nav-link filter-trigger flex items-center justify-between py-2.5 px-2 rounded hover:bg-slate-100">
                        <span><i class="fa-solid fa-layer-group w-5 text-ltm-primary"></i> Gạch Lát Nền (60x60, 80x80, 100x100)</span>
                        <i class="fa-solid fa-angle-right text-slate-400"></i>
                    </a>
                    <a href="#san-pham-all" data-filter="gach-op-tuong" class="mobile-nav-link filter-trigger flex items-center justify-between py-2.5 px-2 rounded hover:bg-slate-100">
                        <span><i class="fa-solid fa-table-cells-large w-5 text-ltm-primary"></i> Gạch Ốp Tường (30x60, 60x120, 80x160)</span>
                        <i class="fa-solid fa-angle-right text-slate-400"></i>
                    </a>
                    <a href="#san-pham-all" data-filter="gach-kho-lon" class="mobile-nav-link filter-trigger flex items-center justify-between py-2.5 px-2 rounded hover:bg-slate-100">
                        <span><i class="fa-solid fa-expand w-5 text-ltm-primary"></i> Gạch Khổ Lớn (1200x2400, 1600x3200)</span>
                        <i class="fa-solid fa-angle-right text-slate-400"></i>
                    </a>
                    <a href="#san-pham-all" data-filter="gach-trang-tri" class="mobile-nav-link filter-trigger flex items-center justify-between py-2.5 px-2 rounded hover:bg-slate-100">
                        <span><i class="fa-solid fa-wand-magic-sparkles w-5 text-ltm-primary"></i> Gạch Trang Trí, Gạch Hoa, Mosaic</span>
                        <i class="fa-solid fa-angle-right text-slate-400"></i>
                    </a>
                    <a href="#san-pham-all" data-filter="gach-go" class="mobile-nav-link filter-trigger flex items-center justify-between py-2.5 px-2 rounded hover:bg-slate-100">
                        <span><i class="fa-solid fa-tree w-5 text-ltm-primary"></i> Gạch Gỗ / Gạch Giả Gỗ Cao Cấp</span>
                        <i class="fa-solid fa-angle-right text-slate-400"></i>
                    </a>
                    <a href="#san-pham-all" data-filter="thiet-bi-nha-tam" class="mobile-nav-link filter-trigger flex items-center justify-between py-2.5 px-2 rounded hover:bg-slate-100">
                        <span><i class="fa-solid fa-bath w-5 text-ltm-primary"></i> Thiết Bị Nhà Tắm Nhập Khẩu</span>
                        <i class="fa-solid fa-angle-right text-slate-400"></i>
                    </a>
                    <a href="#doi-tac" class="mobile-nav-link flex items-center justify-between py-2.5 px-2 rounded hover:bg-slate-100">
                        <span><i class="fa-solid fa-handshake w-5 text-ltm-gold"></i> Đối Tác Thương Hiệu</span>
                        <i class="fa-solid fa-angle-right text-slate-400"></i>
                    </a>
                    <a href="#bai-viet" class="mobile-nav-link flex items-center justify-between py-2.5 px-2 rounded hover:bg-slate-100">
                        <span><i class="fa-solid fa-newspaper w-5 text-ltm-gold"></i> Bài Viết & Kinh Nghiệm</span>
                        <i class="fa-solid fa-angle-right text-slate-400"></i>
                    </a>
                    <a href="#bao-gia" class="mobile-nav-link flex items-center justify-between py-2.5 px-2 rounded hover:bg-slate-100">
                        <span><i class="fa-solid fa-file-signature w-5 text-ltm-gold"></i> Yêu Cầu Báo Giá</span>
                        <i class="fa-solid fa-angle-right text-slate-400"></i>
                    </a>
                    <a href="#ban-do" class="mobile-nav-link flex items-center justify-between py-2.5 px-2 rounded hover:bg-slate-100">
                        <span><i class="fa-solid fa-map-location-dot w-5 text-ltm-gold"></i> Bản Đồ & Fanpage</span>
                        <i class="fa-solid fa-angle-right text-slate-400"></i>
                    </a>
                </div>
            </div>
            <div class="p-4 bg-slate-50 border-t border-slate-200 text-xs space-y-1.5">
                <div class="font-bold text-ltm-primary">CÔNG TY TNHH TM & DV L.T.M</div>
                <div class="text-slate-600"><i class="fa-solid fa-location-dot mr-1 text-ltm-gold"></i>28 Lương Trúc Đàm, Thanh Khê, Đà Nẵng</div>
                <div class="text-slate-600"><i class="fa-solid fa-phone mr-1 text-ltm-gold"></i>Hotline/Zalo: 0914.191.825</div>
            </div>
        </div>
    </div>

    <!-- ==================== 3. BANNER SLIDER TỰ TRƯỢT (2 SLIDE KÍCH THƯỚC BẰNG NHAU, CHỮ CÁCH XA VIỀN, KHÔNG MẤT CHỮ) ==================== -->
    <section id="top" class="py-3 md:py-4">
        <div class="flatsome-container">
            <div class="relative w-full overflow-hidden rounded-xl shadow-md bg-ltm-primary">
                <!-- Khung chứa 2 banner có cùng chiều cao chuẩn trên cả điện thoại và máy tính -->
                <div id="bannerTrack" class="relative w-full h-[250px] sm:h-[310px] md:h-[380px] lg:h-[420px]">
                    
                    <!-- SLIDE 1: Gạch Ốp Lát Cao Cấp Đà Nẵng -->
                    <div class="banner-slide absolute inset-0 w-full h-full transition-opacity duration-700 opacity-100 z-10 bg-gradient-to-r from-[#0d2744] via-[#12355b] to-[#1d4e89] flex items-center">
                        <!-- Khoảng đệm lớn (px-8 sm:px-14 md:px-20) đảm bảo chữ và ảnh cách xa viền banner tuyệt đối -->
                        <div class="w-full h-full px-8 sm:px-14 md:px-20 py-5 sm:py-8 grid grid-cols-12 items-center gap-3 md:gap-6">
                            <!-- Nội dung chữ nằm gọn bên trong banner -->
                            <div class="col-span-7 sm:col-span-7 text-white space-y-1.5 sm:space-y-3">
                                <div class="inline-block text-[10px] sm:text-xs font-bold uppercase tracking-wider px-2.5 py-0.5 rounded bg-amber-500/20 text-amber-300 border border-amber-400/30">
                                    LTM.COM • SHOWROOM GẠCH ĐÀ NẴNG
                                </div>
                                <h1 class="text-sm sm:text-xl md:text-3xl lg:text-4xl font-extrabold leading-snug text-white">
                                    GẠCH ỐP LÁT CAO CẤP ĐÀ NẴNG
                                </h1>
                                <p class="text-[11px] sm:text-xs md:text-sm text-slate-200 leading-relaxed">
                                    Chuyên Gạch Men, Gạch Hoa, Gạch Gỗ, Gạch Khổ Lớn &amp; Gạch Trang Trí Cao Cấp. Mẫu mã sang trọng, bền đẹp cho mọi công trình.
                                </p>
                                <div class="pt-1 flex flex-wrap items-center gap-2 text-[10px] sm:text-xs text-amber-300 font-semibold">
                                    <span><i class="fa-solid fa-location-dot mr-1"></i>28 Lương Trúc Đàm, Thanh Khê</span>
                                    <span class="hidden sm:inline">•</span>
                                    <span><i class="fa-solid fa-phone mr-1"></i>0914.191.825</span>
                                </div>
                            </div>
                            <!-- Cụm ảnh sản phẩm thực tế nằm gọn trong khung phải của banner -->
                            <div class="col-span-5 sm:col-span-5 h-full flex items-center justify-center">
                                <div class="grid grid-cols-2 gap-1.5 sm:gap-2.5 w-full max-w-[160px] sm:max-w-[240px] md:max-w-[300px] p-1.5 sm:p-2.5 bg-white/10 rounded-xl border border-white/20 backdrop-blur-xs">
                                    <img 
                                        src="https://lh3.googleusercontent.com/d/1P2fePSvPXm6YIcNDixVa0YwFWshcHFDY" 
                                        onerror="this.src='https://drive.google.com/thumbnail?id=1P2fePSvPXm6YIcNDixVa0YwFWshcHFDY&sz=w500'"
                                        alt="Gạch ốp lát cao cấp L.T.M" 
                                        class="w-full h-16 sm:h-24 md:h-28 object-cover rounded-lg border border-white/30"
                                    >
                                    <img 
                                        src="https://lh3.googleusercontent.com/d/11z7ir7cmqEcdrYuAThZvpOhgUVFsLUnP" 
                                        onerror="this.src='https://drive.google.com/thumbnail?id=11z7ir7cmqEcdrYuAThZvpOhgUVFsLUnP&sz=w500'"
                                        alt="Gạch men vân đá L.T.M" 
                                        class="w-full h-16 sm:h-24 md:h-28 object-cover rounded-lg border border-white/30"
                                    >
                                    <img 
                                        src="https://lh3.googleusercontent.com/d/19jauCH_X7lcc0KNlu2OJ75CRiw3ArT7r" 
                                        onerror="this.src='https://drive.google.com/thumbnail?id=19jauCH_X7lcc0KNlu2OJ75CRiw3ArT7r&sz=w500'"
                                        alt="Gạch trang trí L.T.M" 
                                        class="w-full h-16 sm:h-24 md:h-28 object-cover rounded-lg border border-white/30"
                                    >
                                    <img 
                                        src="https://lh3.googleusercontent.com/d/1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN" 
                                        onerror="this.src='https://drive.google.com/thumbnail?id=1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN&sz=w500'"
                                        alt="Gạch vân gỗ L.T.M" 
                                        class="w-full h-16 sm:h-24 md:h-28 object-cover rounded-lg border border-white/30"
                                    >
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- SLIDE 2: Thiết Bị Nhà Tắm Nhập Khẩu & Gạch Trang Trí (Kích thước bằng hệt Slide 1) -->
                    <div class="banner-slide absolute inset-0 w-full h-full transition-opacity duration-700 opacity-0 z-0 bg-gradient-to-r from-[#1a2e40] via-[#163a5f] to-[#0f2b48] flex items-center">
                        <!-- Khoảng đệm lớn (px-8 sm:px-14 md:px-20) đảm bảo chữ và ảnh cách xa viền banner tuyệt đối -->
                        <div class="w-full h-full px-8 sm:px-14 md:px-20 py-5 sm:py-8 grid grid-cols-12 items-center gap-3 md:gap-6">
                            <div class="col-span-7 sm:col-span-7 text-white space-y-1.5 sm:space-y-3">
                                <div class="inline-block text-[10px] sm:text-xs font-bold uppercase tracking-wider px-2.5 py-0.5 rounded bg-amber-500/20 text-amber-300 border border-amber-400/30">
                                    CÔNG TY TNHH TM &amp; DV L.T.M
                                </div>
                                <h2 class="text-sm sm:text-xl md:text-3xl lg:text-4xl font-extrabold leading-snug text-white">
                                    THIẾT BỊ NHÀ TẮM NHẬP KHẨU
                                </h2>
                                <p class="text-[11px] sm:text-xs md:text-sm text-slate-200 leading-relaxed">
                                    Phân phối Bồn Cầu, Tủ Lavabo, Sen Tắm, Bồn Tắm &amp; Phụ Kiện Phòng Tắm chính hãng. Chiết khấu hấp dẫn cho nhà thầu và công trình.
                                </p>
                                <div class="pt-1 flex flex-wrap items-center gap-2 text-[10px] sm:text-xs text-amber-300 font-semibold">
                                    <span><i class="fa-solid fa-truck-fast mr-1"></i>Giao hàng tận công trình Đà Nẵng</span>
                                    <span class="hidden sm:inline">•</span>
                                    <span><i class="fa-solid fa-phone mr-1"></i>0914.191.825</span>
                                </div>
                            </div>
                            <div class="col-span-5 sm:col-span-5 h-full flex items-center justify-center">
                                <div class="grid grid-cols-2 gap-1.5 sm:gap-2.5 w-full max-w-[160px] sm:max-w-[240px] md:max-w-[300px] p-1.5 sm:p-2.5 bg-white/10 rounded-xl border border-white/20 backdrop-blur-xs">
                                    <img 
                                        src="https://lh3.googleusercontent.com/d/19k5uWHn_xeas2_BMP_JgBDwwu-IysSRP" 
                                        onerror="this.src='https://drive.google.com/thumbnail?id=19k5uWHn_xeas2_BMP_JgBDwwu-IysSRP&sz=w500'"
                                        alt="Thiết bị vệ sinh L.T.M" 
                                        class="w-full h-16 sm:h-24 md:h-28 object-cover rounded-lg border border-white/30"
                                    >
                                    <img 
                                        src="https://lh3.googleusercontent.com/d/1oah4j6YAPIsJacMYQFJ0JGVemrMwqCgf" 
                                        onerror="this.src='https://drive.google.com/thumbnail?id=1oah4j6YAPIsJacMYQFJ0JGVemrMwqCgf&sz=w500'"
                                        alt="Phòng tắm nhập khẩu L.T.M" 
                                        class="w-full h-16 sm:h-24 md:h-28 object-cover rounded-lg border border-white/30"
                                    >
                                    <img 
                                        src="https://lh3.googleusercontent.com/d/15IWAPhzVLsyUO5TDRoWXxvncrHoFcH1_" 
                                        onerror="this.src='https://drive.google.com/thumbnail?id=15IWAPhzVLsyUO5TDRoWXxvncrHoFcH1_&sz=w500'"
                                        alt="Tủ lavabo cao cấp L.T.M" 
                                        class="w-full h-16 sm:h-24 md:h-28 object-cover rounded-lg border border-white/30"
                                    >
                                    <img 
                                        src="https://lh3.googleusercontent.com/d/1WLKyUBxRc63xFN9GBUhFcqE0xPo0sQKh" 
                                        onerror="this.src='https://drive.google.com/thumbnail?id=1WLKyUBxRc63xFN9GBUhFcqE0xPo0sQKh&sz=w500'"
                                        alt="Sen tắm nhập khẩu L.T.M" 
                                        class="w-full h-16 sm:h-24 md:h-28 object-cover rounded-lg border border-white/30"
                                    >
                                </div>
                            </div>
                        </div>
                    </div>

                </div>

                <!-- Nút điều hướng Trái / Phải của Banner -->
                <button id="prevBannerBtn" type="button" aria-label="Slide trước" class="absolute left-2 top-1/2 -translate-y-1/2 z-20 w-7 h-7 sm:w-9 sm:h-9 rounded-full bg-black/30 hover:bg-black/55 text-white flex items-center justify-center transition">
                    <i class="fa-solid fa-chevron-left text-xs sm:text-sm"></i>
                </button>
                <button id="nextBannerBtn" type="button" aria-label="Slide tiếp" class="absolute right-2 top-1/2 -translate-y-1/2 z-20 w-7 h-7 sm:w-9 sm:h-9 rounded-full bg-black/30 hover:bg-black/55 text-white flex items-center justify-center transition">
                    <i class="fa-solid fa-chevron-right text-xs sm:text-sm"></i>
                </button>

                <!-- Chấm tròn chỉ báo Slide -->
                <div class="absolute bottom-2.5 left-1/2 -translate-x-1/2 z-20 flex items-center gap-2">
                    <button type="button" data-slide="0" class="banner-dot w-6 h-2 rounded-full bg-amber-400 transition-all"></button>
                    <button type="button" data-slide="1" class="banner-dot w-2 h-2 rounded-full bg-white/50 hover:bg-white transition-all"></button>
                </div>
            </div>
        </div>
    </section>

    <!-- ==================== 4. DANH MỤC SẢN PHẨM TRANG CHỦ (CHỮ NHỎ GỌN, LẤY TỪ WEB MẪU, ĐẸP TRÊN PC & MOBILE) ==================== -->
    <section id="danh-muc-trang-chu" class="py-4 md:py-6">
        <div class="flatsome-container">
            <div class="section-title-container">
                <h2 class="section-title-main text-sm sm:text-base md:text-lg">
                    DANH MỤC SẢN PHẨM
                </h2>
                <span class="text-xs text-slate-500">Chọn danh mục để lọc nhanh sản phẩm</span>
            </div>

            <!-- Lưới danh mục sản phẩm chuẩn mẫu gachmendanang.vn (Chữ danh mục nhỏ gọn, không xuống dòng lộn xộn) -->
            <div class="grid grid-cols-3 sm:grid-cols-4 md:grid-cols-6 lg:grid-cols-6 gap-2.5 sm:gap-3.5">
                <!-- Danh mục 1: Gạch Lát Nền -->
                <button type="button" data-filter="gach-lat-nen" class="filter-trigger group bg-white rounded-xl border border-slate-200 hover:border-ltm-primary p-2 sm:p-2.5 shadow-xs hover:shadow-md transition text-center flex flex-col items-center">
                    <div class="w-full aspect-[4/3] rounded-lg overflow-hidden bg-slate-100 mb-2">
                        <img 
                            src="https://lh3.googleusercontent.com/d/1P2fePSvPXm6YIcNDixVa0YwFWshcHFDY" 
                            onerror="this.src='https://drive.google.com/thumbnail?id=1P2fePSvPXm6YIcNDixVa0YwFWshcHFDY&sz=w400'"
                            alt="Gạch Lát Nền" 
                            class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
                        >
                    </div>
                    <div class="text-[11px] sm:text-xs font-bold text-ltm-primary whitespace-nowrap">GẠCH LÁT NỀN</div>
                    <div class="text-[10px] text-slate-500 whitespace-nowrap">60x60 • 80x80 • 100x100</div>
                </button>

                <!-- Danh mục 2: Gạch Ốp Tường -->
                <button type="button" data-filter="gach-op-tuong" class="filter-trigger group bg-white rounded-xl border border-slate-200 hover:border-ltm-primary p-2 sm:p-2.5 shadow-xs hover:shadow-md transition text-center flex flex-col items-center">
                    <div class="w-full aspect-[4/3] rounded-lg overflow-hidden bg-slate-100 mb-2">
                        <img 
                            src="https://lh3.googleusercontent.com/d/1KTDzdSGqiXWuLZDkPoDD7oZZVL-5F3Rr" 
                            onerror="this.src='https://drive.google.com/thumbnail?id=1KTDzdSGqiXWuLZDkPoDD7oZZVL-5F3Rr&sz=w400'"
                            alt="Gạch Ốp Tường" 
                            class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
                        >
                    </div>
                    <div class="text-[11px] sm:text-xs font-bold text-ltm-primary whitespace-nowrap">GẠCH ỐP TƯỜNG</div>
                    <div class="text-[10px] text-slate-500 whitespace-nowrap">30x60 • 60x120 • 80x160</div>
                </button>

                <!-- Danh mục 3: Gạch Khổ Lớn -->
                <button type="button" data-filter="gach-kho-lon" class="filter-trigger group bg-white rounded-xl border border-slate-200 hover:border-ltm-primary p-2 sm:p-2.5 shadow-xs hover:shadow-md transition text-center flex flex-col items-center">
                    <div class="w-full aspect-[4/3] rounded-lg overflow-hidden bg-slate-100 mb-2">
                        <img 
                            src="https://lh3.googleusercontent.com/d/1uqL6ACCB5ne0G1BYkXCurdnrsf1m2lr4" 
                            onerror="this.src='https://drive.google.com/thumbnail?id=1uqL6ACCB5ne0G1BYkXCurdnrsf1m2lr4&sz=w400'"
                            alt="Gạch Khổ Lớn" 
                            class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
                        >
                    </div>
                    <div class="text-[11px] sm:text-xs font-bold text-ltm-primary whitespace-nowrap">GẠCH KHỔ LỚN</div>
                    <div class="text-[10px] text-slate-500 whitespace-nowrap">1200x2400 • 1600x3200</div>
                </button>

                <!-- Danh mục 4: Gạch Trang Trí & Gạch Hoa -->
                <button type="button" data-filter="gach-trang-tri" class="filter-trigger group bg-white rounded-xl border border-slate-200 hover:border-ltm-primary p-2 sm:p-2.5 shadow-xs hover:shadow-md transition text-center flex flex-col items-center">
                    <div class="w-full aspect-[4/3] rounded-lg overflow-hidden bg-slate-100 mb-2">
                        <img 
                            src="https://lh3.googleusercontent.com/d/19jauCH_X7lcc0KNlu2OJ75CRiw3ArT7r" 
                            onerror="this.src='https://drive.google.com/thumbnail?id=19jauCH_X7lcc0KNlu2OJ75CRiw3ArT7r&sz=w400'"
                            alt="Gạch Trang Trí" 
                            class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
                        >
                    </div>
                    <div class="text-[11px] sm:text-xs font-bold text-ltm-primary whitespace-nowrap">GẠCH TRANG TRÍ</div>
                    <div class="text-[10px] text-slate-500 whitespace-nowrap">Gạch Hoa • Terrazzo • Mosaic</div>
                </button>

                <!-- Danh mục 5: Gạch Vân Gỗ -->
                <button type="button" data-filter="gach-go" class="filter-trigger group bg-white rounded-xl border border-slate-200 hover:border-ltm-primary p-2 sm:p-2.5 shadow-xs hover:shadow-md transition text-center flex flex-col items-center">
                    <div class="w-full aspect-[4/3] rounded-lg overflow-hidden bg-slate-100 mb-2">
                        <img 
                            src="https://lh3.googleusercontent.com/d/1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN" 
                            onerror="this.src='https://drive.google.com/thumbnail?id=1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN&sz=w400'"
                            alt="Gạch Vân Gỗ" 
                            class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
                        >
                    </div>
                    <div class="text-[11px] sm:text-xs font-bold text-ltm-primary whitespace-nowrap">GẠCH VÂN GỖ</div>
                    <div class="text-[10px] text-slate-500 whitespace-nowrap">15x80 • 15x90 • 20x100</div>
                </button>

                <!-- Danh mục 6: Thiết Bị Vệ Sinh Nhập Khẩu -->
                <button type="button" data-filter="thiet-bi-nha-tam" class="filter-trigger group bg-white rounded-xl border border-slate-200 hover:border-ltm-primary p-2 sm:p-2.5 shadow-xs hover:shadow-md transition text-center flex flex-col items-center">
                    <div class="w-full aspect-[4/3] rounded-lg overflow-hidden bg-slate-100 mb-2">
                        <img 
                            src="https://lh3.googleusercontent.com/d/19k5uWHn_xeas2_BMP_JgBDwwu-IysSRP" 
                            onerror="this.src='https://drive.google.com/thumbnail?id=19k5uWHn_xeas2_BMP_JgBDwwu-IysSRP&sz=w400'"
                            alt="Thiết Bị Vệ Sinh" 
                            class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
                        >
                    </div>
                    <div class="text-[11px] sm:text-xs font-bold text-ltm-primary whitespace-nowrap">THIẾT BỊ VỆ SINH</div>
                    <div class="text-[10px] text-slate-500 whitespace-nowrap">Lavabo • Bồn Cầu • Sen Tắm</div>
                </button>
            </div>

            <!-- Các nút kích thước chi tiết giống hệt gachmendanang.vn (chữ nhỏ gọn, viết liền không gãy dòng) -->
            <div class="mt-3 flex flex-wrap items-center gap-1.5">
                <button type="button" data-filter="all" class="filter-trigger text-[11px] font-semibold px-2.5 py-1 rounded border border-ltm-primary bg-ltm-primary text-white whitespace-nowrap">Tất cả (19 mẫu thực tế)</button>
                <button type="button" data-filter="gach-lat-nen" class="filter-trigger text-[11px] font-medium px-2.5 py-1 rounded border border-slate-200 bg-white hover:border-ltm-primary text-slate-700 whitespace-nowrap">Gạch 60x60</button>
                <button type="button" data-filter="gach-lat-nen" class="filter-trigger text-[11px] font-medium px-2.5 py-1 rounded border border-slate-200 bg-white hover:border-ltm-primary text-slate-700 whitespace-nowrap">Gạch 80x80</button>
                <button type="button" data-filter="gach-lat-nen" class="filter-trigger text-[11px] font-medium px-2.5 py-1 rounded border border-slate-200 bg-white hover:border-ltm-primary text-slate-700 whitespace-nowrap">Gạch 100x100</button>
                <button type="button" data-filter="gach-op-tuong" class="filter-trigger text-[11px] font-medium px-2.5 py-1 rounded border border-slate-200 bg-white hover:border-ltm-primary text-slate-700 whitespace-nowrap">Gạch 30x60</button>
                <button type="button" data-filter="gach-op-tuong" class="filter-trigger text-[11px] font-medium px-2.5 py-1 rounded border border-slate-200 bg-white hover:border-ltm-primary text-slate-700 whitespace-nowrap">Gạch 60x120</button>
                <button type="button" data-filter="gach-op-tuong" class="filter-trigger text-[11px] font-medium px-2.5 py-1 rounded border border-slate-200 bg-white hover:border-ltm-primary text-slate-700 whitespace-nowrap">Gạch 80x160</button>
                <button type="button" data-filter="gach-kho-lon" class="filter-trigger text-[11px] font-medium px-2.5 py-1 rounded border border-slate-200 bg-white hover:border-ltm-primary text-slate-700 whitespace-nowrap">Gạch 1200x2400</button>
                <button type="button" data-filter="gach-kho-lon" class="filter-trigger text-[11px] font-medium px-2.5 py-1 rounded border border-slate-200 bg-white hover:border-ltm-primary text-slate-700 whitespace-nowrap">Gạch 1600x3200</button>
                <button type="button" data-filter="gach-trang-tri" class="filter-trigger text-[11px] font-medium px-2.5 py-1 rounded border border-slate-200 bg-white hover:border-ltm-primary text-slate-700 whitespace-nowrap">Gạch Hoa &amp; Bông</button>
                <button type="button" data-filter="gach-go" class="filter-trigger text-[11px] font-medium px-2.5 py-1 rounded border border-slate-200 bg-white hover:border-ltm-primary text-slate-700 whitespace-nowrap">Gạch Giả Gỗ</button>
                <button type="button" data-filter="thiet-bi-nha-tam" class="filter-trigger text-[11px] font-medium px-2.5 py-1 rounded border border-slate-200 bg-white hover:border-ltm-primary text-slate-700 whitespace-nowrap">Thiết Bị Nhà Tắm</button>
            </div>
        </div>
    </section>

    <!-- ==================== 5. DANH SÁCH SẢN PHẨM THỰC TẾ (19 ẢNH GOOGLE DRIVE, CHIA 2 CỘT TRÊN ĐIỆN THOẠI, % GIẢM GIÁ GÓC TRÊN TRÁI) ==================== -->
    <div id="san-pham-all" class="space-y-8 py-2">
        <!-- Khu vực hiển thị kết quả khi lọc / tìm kiếm -->
        <div id="filterStatusBanner" class="flatsome-container hidden">
            <div class="bg-amber-50 border border-amber-200 rounded-lg px-4 py-2.5 flex items-center justify-between text-xs sm:text-sm">
                <span id="filterStatusText" class="font-semibold text-ltm-primary">Đang hiển thị sản phẩm theo danh mục</span>
                <button id="resetFilterBtn" type="button" class="text-xs font-bold text-red-600 hover:underline">
                    <i class="fa-solid fa-rotate-left mr-1"></i>Xem tất cả 19 sản phẩm
                </button>
            </div>
        </div>

        <!-- PHẦN 5.1: GẠCH LÁT NỀN & GẠCH ỐP TƯỜNG CAO CẤP (60x120, 80x80, 80x160) -->
        <section class="product-section" data-section-cat="gach-lat-nen gach-op-tuong">
            <div class="flatsome-container">
                <div class="section-title-container">
                    <h2 class="section-title-main text-sm sm:text-base md:text-lg">
                        GẠCH LÁT NỀN &amp; GẠCH ỐP TƯỜNG CAO CẤP
                    </h2>
                    <a href="#bao-gia" class="text-xs font-semibold text-ltm-secondary hover:text-ltm-gold">
                        Nhận bảng giá sỉ công trình <i class="fa-solid fa-angle-right ml-0.5"></i>
                    </a>
                </div>
                <!-- Grid 2 cột trên điện thoại (grid-cols-2), 3 cột tablet, 4 cột desktop -->
                <div id="grid-lat-op" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3 sm:gap-4 md:gap-5"></div>
            </div>
        </section>

        <!-- PHẦN 5.2: GẠCH KHỔ LỚN CAO CẤP (1200x2400, 100x100, 1600x3200) -->
        <section class="product-section" data-section-cat="gach-kho-lon">
            <div class="flatsome-container">
                <div class="section-title-container">
                    <h2 class="section-title-main text-sm sm:text-base md:text-lg">
                        GẠCH KHỔ LỚN VÂN ĐÁ NHẬP KHẨU (1200x2400 • 1600x3200)
                    </h2>
                    <a href="#bao-gia" class="text-xs font-semibold text-ltm-secondary hover:text-ltm-gold">
                        Tư vấn map gạch thực tế <i class="fa-solid fa-angle-right ml-0.5"></i>
                    </a>
                </div>
                <div id="grid-kho-lon" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3 sm:gap-4 md:gap-5"></div>
            </div>
        </section>

        <!-- PHẦN 5.3: GẠCH HOA, GẠCH GỖ & GẠCH TRANG TRÍ CAO CẤP -->
        <section class="product-section" data-section-cat="gach-trang-tri gach-go">
            <div class="flatsome-container">
                <div class="section-title-container">
                    <h2 class="section-title-main text-sm sm:text-base md:text-lg">
                        GẠCH HOA, GẠCH VÂN GỖ &amp; GẠCH TRANG TRÍ CAO CẤP
                    </h2>
                    <a href="#bao-gia" class="text-xs font-semibold text-ltm-secondary hover:text-ltm-gold">
                        Xem mẫu tại Showroom <i class="fa-solid fa-angle-right ml-0.5"></i>
                    </a>
                </div>
                <div id="grid-trang-tri-go" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3 sm:gap-4 md:gap-5"></div>
            </div>
        </section>

        <!-- PHẦN 5.4: THIẾT BỊ NHÀ TẮM NHẬP KHẨU CAO CẤP -->
        <section class="product-section" data-section-cat="thiet-bi-nha-tam">
            <div class="flatsome-container">
                <div class="section-title-container">
                    <h2 class="section-title-main text-sm sm:text-base md:text-lg">
                        THIẾT BỊ NHÀ TẮM &amp; VỆ SINH NHẬP KHẨU
                    </h2>
                    <a href="#bao-gia" class="text-xs font-semibold text-ltm-secondary hover:text-ltm-gold">
                        Ưu đãi combo phòng tắm <i class="fa-solid fa-angle-right ml-0.5"></i>
                    </a>
                </div>
                <div id="grid-nha-tam" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3 sm:gap-4 md:gap-5"></div>
            </div>
        </section>
    </div>

    <!-- ==================== 6. GIỚI THIỆU VỀ CÔNG TY TNHH THƯƠNG MẠI VÀ DỊCH VỤ L.T.M ==================== -->
    <section class="py-6 md:py-8">
        <div class="flatsome-container">
            <div class="bg-white rounded-xl border border-slate-200 p-4 sm:p-6 md:p-8 shadow-xs">
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-center">
                    <div class="lg:col-span-7 space-y-3">
                        <h2 class="text-base sm:text-lg md:text-xl font-extrabold text-ltm-primary uppercase">
                            CÔNG TY TNHH THƯƠNG MẠI VÀ DỊCH VỤ L.T.M – TỔNG KHO GẠCH ỐP LÁT &amp; THIẾT BỊ NHÀ TẮM ĐÀ NẴNG
                        </h2>
                        <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
                            <strong>CÔNG TY TNHH THƯƠNG MẠI VÀ DỊCH VỤ L.T.M</strong> (Website: <strong>ltm.com</strong>) là đơn vị uy tín lâu năm tại Đà Nẵng chuyên cung cấp <strong>gạch men, gạch hoa, gạch gỗ, gạch khổ lớn, gạch trang trí cao cấp và thiết bị nhà tắm nhập khẩu</strong> cho nhà phố, biệt thự, khách sạn, resort và các dự án công trình tại Đà Nẵng – Miền Trung.
                        </p>
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-3 pt-1 text-xs text-slate-700">
                            <div class="p-3 rounded-lg bg-slate-50 border border-slate-200">
                                <div class="font-bold text-ltm-primary mb-1"><i class="fa-solid fa-gem text-ltm-gold mr-1.5"></i>Sản Phẩm Chính Hãng Tuyển Chọn</div>
                                <p class="text-slate-600">Đa dạng mẫu gạch xương đá Porcelain, Granite, gạch nhập khẩu Tây Ban Nha, Italy, Ấn Độ và các thương hiệu hàng đầu trong nước.</p>
                            </div>
                            <div class="p-3 rounded-lg bg-slate-50 border border-slate-200">
                                <div class="font-bold text-ltm-primary mb-1"><i class="fa-solid fa-truck-ramp-box text-ltm-gold mr-1.5"></i>Giá Tốt Tận Kho – Giao Tận Chân Công Trình</div>
                                <p class="text-slate-600">Chính sách chiết khấu cao cho kiến trúc sư, nhà thầu và chủ nhà. Hỗ trợ vận chuyển nhanh chóng tại Đà Nẵng.</p>
                            </div>
                        </div>
                    </div>
                    <div class="lg:col-span-5">
                        <div class="bg-ltm-primary text-white rounded-xl p-5 space-y-3">
                            <div class="flex items-center gap-3 border-b border-white/15 pb-3">
                                <img 
                                    src="https://lh3.googleusercontent.com/d/1657a_RNzOWwdZGeDnC2P_1sW2SUH5Jia" 
                                    onerror="this.src='https://placehold.co/80x80/ffffff/12355b?text=LTM'"
                                    alt="Logo L.T.M" 
                                    class="w-11 h-11 rounded-lg bg-white p-1 object-contain shrink-0"
                                >
                                <div>
                                    <div class="font-bold text-sm text-amber-300">THÔNG TIN DOANH NGHIỆP</div>
                                    <div class="text-xs text-slate-200">CÔNG TY TNHH TM &amp; DV L.T.M</div>
                                </div>
                            </div>
                            <ul class="space-y-2 text-xs text-slate-100">
                                <li class="flex items-start gap-2">
                                    <i class="fa-solid fa-location-dot text-amber-400 mt-0.5 w-4"></i>
                                    <span><strong>Showroom:</strong> 28 Lương Trúc Đàm, Quận Thanh Khê, TP. Đà Nẵng</span>
                                </li>
                                <li class="flex items-start gap-2">
                                    <i class="fa-solid fa-phone-volume text-amber-400 mt-0.5 w-4"></i>
                                    <span><strong>Hotline / Zalo:</strong> <a href="tel:0914191825" class="text-amber-300 font-bold hover:underline">0914.191.825</a></span>
                                </li>
                                <li class="flex items-start gap-2">
                                    <i class="fa-solid fa-globe text-amber-400 mt-0.5 w-4"></i>
                                    <span><strong>Website:</strong> ltm.com</span>
                                </li>
                                <li class="flex items-start gap-2">
                                    <i class="fa-brands fa-facebook text-amber-400 mt-0.5 w-4"></i>
                                    <span><strong>Fanpage:</strong> <a href="https://www.facebook.com/profile.php?id=100046135087441" target="_blank" rel="noopener noreferrer" class="underline hover:text-amber-300">Gạch Ốp Lát Cao Cấp L.T.M Đà Nẵng</a></span>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ==================== 7. DANH MỤC CÁC ĐỐI TÁC THƯƠNG HIỆU ==================== -->
    <section id="doi-tac" class="py-4 md:py-6">
        <div class="flatsome-container">
            <div class="section-title-container">
                <h2 class="section-title-main text-sm sm:text-base md:text-lg">
                    ĐỐI TÁC &amp; THƯƠNG HIỆU PHÂN PHỐI
                </h2>
                <span class="text-xs text-slate-500">Hợp tác cùng các nhà sản xuất gạch &amp; thiết bị vệ sinh hàng đầu</span>
            </div>

            <div class="grid grid-cols-2 sm:grid-cols-4 lg:grid-cols-8 gap-2.5 sm:gap-3">
                <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center hover:border-ltm-primary transition">
                    <div class="text-xs sm:text-sm font-extrabold text-ltm-primary tracking-wider">ROCERSA</div>
                    <div class="text-[10px] text-slate-500">Gạch Nhập Khẩu TBN</div>
                </div>
                <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center hover:border-ltm-primary transition">
                    <div class="text-xs sm:text-sm font-extrabold text-ltm-primary tracking-wider">VIET HUONG</div>
                    <div class="text-[10px] text-slate-500">Ceramics Cao Cấp</div>
                </div>
                <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center hover:border-ltm-primary transition">
                    <div class="text-xs sm:text-sm font-extrabold text-ltm-primary tracking-wider">EUROTILE</div>
                    <div class="text-[10px] text-slate-500">Gạch Nghệ Thuật</div>
                </div>
                <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center hover:border-ltm-primary transition">
                    <div class="text-xs sm:text-sm font-extrabold text-ltm-primary tracking-wider">VIGLACERA</div>
                    <div class="text-[10px] text-slate-500">Gạch &amp; Thiết Bị Tắm</div>
                </div>
                <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center hover:border-ltm-primary transition">
                    <div class="text-xs sm:text-sm font-extrabold text-ltm-primary tracking-wider">ĐỒNG TÂM</div>
                    <div class="text-[10px] text-slate-500">Gạch Men &amp; Gạch Bông</div>
                </div>
                <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center hover:border-ltm-primary transition">
                    <div class="text-xs sm:text-sm font-extrabold text-ltm-primary tracking-wider">PRIME</div>
                    <div class="text-[10px] text-slate-500">Gạch Ốp Lát Cao Cấp</div>
                </div>
                <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center hover:border-ltm-primary transition">
                    <div class="text-xs sm:text-sm font-extrabold text-ltm-primary tracking-wider">TOTO</div>
                    <div class="text-[10px] text-slate-500">Thiết Bị Nhà Tắm</div>
                </div>
                <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center hover:border-ltm-primary transition">
                    <div class="text-xs sm:text-sm font-extrabold text-ltm-primary tracking-wider">INAX</div>
                    <div class="text-[10px] text-slate-500">Thiết Bị Vệ Sinh</div>
                </div>
            </div>
        </div>
    </section>

    <!-- ==================== 8. FORM YÊU CẦU TƯ VẤN VÀ BÁO GIÁ TRANG CHỦ ==================== -->
    <section id="bao-gia" class="py-5 md:py-7">
        <div class="flatsome-container">
            <div class="bg-gradient-to-br from-ltm-primary to-[#1b497d] rounded-xl p-4 sm:p-6 md:p-8 text-white shadow-md">
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-center">
                    <div class="lg:col-span-5 space-y-2.5">
                        <h2 class="text-base sm:text-xl font-extrabold uppercase text-amber-300">
                            ĐĂNG KÝ NHẬN BÁO GIÁ &amp; MẪU GẠCH THỰC TẾ
                        </h2>
                        <p class="text-xs sm:text-sm text-slate-200 leading-relaxed">
                            Quý khách hàng, Kiến trúc sư và Nhà thầu cần báo giá sỉ/lẻ các dòng gạch men, gạch hoa, gạch gỗ, gạch khổ lớn hoặc combo thiết bị phòng tắm nhập khẩu vui lòng để lại thông tin. Bộ phận kinh doanh L.T.M sẽ gửi báo giá qua Zalo chỉ sau 5 phút!
                        </p>
                        <div class="pt-2 space-y-1.5 text-xs text-slate-100">
                            <div><i class="fa-solid fa-check text-amber-400 mr-2"></i>Báo giá chiết khấu trực tiếp theo khối lượng công trình</div>
                            <div><i class="fa-solid fa-check text-amber-400 mr-2"></i>Gửi hình ảnh &amp; video thực tế từng mẫu gạch tại kho</div>
                            <div><i class="fa-solid fa-check text-amber-400 mr-2"></i>Hỗ trợ phối cảnh &amp; giao hàng tận nơi tại Đà Nẵng</div>
                        </div>
                    </div>

                    <div class="lg:col-span-7">
                        <form id="quoteRequestForm" class="bg-white text-slate-800 rounded-xl p-4 sm:p-5 shadow-lg space-y-3">
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                                <div>
                                    <label class="block text-xs font-bold text-slate-700 mb-1">Họ và tên quý khách *</label>
                                    <input type="text" id="qName" required placeholder="Nhập họ và tên..." class="w-full px-3 py-2 text-xs sm:text-sm border border-slate-300 rounded-lg focus:outline-none focus:border-ltm-primary">
                                </div>
                                <div>
                                    <label class="block text-xs font-bold text-slate-700 mb-1">Số điện thoại / Zalo *</label>
                                    <input type="tel" id="qPhone" required placeholder="Ví dụ: 0914191825" class="w-full px-3 py-2 text-xs sm:text-sm border border-slate-300 rounded-lg focus:outline-none focus:border-ltm-primary">
                                </div>
                            </div>
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                                <div>
                                    <label class="block text-xs font-bold text-slate-700 mb-1">Danh mục cần báo giá</label>
                                    <select id="qCategory" class="w-full px-3 py-2 text-xs sm:text-sm border border-slate-300 rounded-lg focus:outline-none focus:border-ltm-primary bg-white">
                                        <option value="Gạch lát nền cao cấp (60x60, 80x80, 100x100)">Gạch lát nền cao cấp (60x60, 80x80, 100x100)</option>
                                        <option value="Gạch ốp tường (30x60, 60x120, 80x160)">Gạch ốp tường (30x60, 60x120, 80x160)</option>
                                        <option value="Gạch khổ lớn (1200x2400, 1600x3200)">Gạch khổ lớn (1200x2400, 1600x3200)</option>
                                        <option value="Gạch hoa, gạch bông & gạch trang trí">Gạch hoa, gạch bông &amp; gạch trang trí</option>
                                        <option value="Gạch vân gỗ cao cấp">Gạch vân gỗ cao cấp</option>
                                        <option value="Thiết bị nhà tắm nhập khẩu">Thiết bị nhà tắm nhập khẩu</option>
                                        <option value="Báo giá trọn gói nhà mới / công trình">Báo giá trọn gói nhà mới / công trình</option>
                                    </select>
                                </div>
                                <div>
                                    <label class="block text-xs font-bold text-slate-700 mb-1">Diện tích / Số lượng dự kiến</label>
                                    <input type="text" id="qArea" placeholder="Ví dụ: 150m2 hoặc 3 phòng tắm..." class="w-full px-3 py-2 text-xs sm:text-sm border border-slate-300 rounded-lg focus:outline-none focus:border-ltm-primary">
                                </div>
                            </div>
                            <div>
                                <label class="block text-xs font-bold text-slate-700 mb-1">Yêu cầu chi tiết (Mã sản phẩm, địa chỉ giao hàng...)</label>
                                <textarea id="qNote" rows="2" placeholder="Nhập thêm ghi chú nếu có..." class="w-full px-3 py-2 text-xs sm:text-sm border border-slate-300 rounded-lg focus:outline-none focus:border-ltm-primary"></textarea>
                            </div>
                            <div class="flex flex-col sm:flex-row items-center justify-between gap-2 pt-1">
                                <button type="submit" class="w-full sm:w-auto px-6 py-2.5 rounded-lg bg-ltm-primary hover:bg-ltm-secondary text-white font-bold text-xs sm:text-sm transition">
                                    <i class="fa-solid fa-paper-plane mr-1.5"></i>GỬI YÊU CẦU BÁO GIÁ NGAY
                                </button>
                                <span class="text-[11px] text-slate-500">Hoặc liên hệ trực tiếp Zalo: <strong class="text-ltm-primary">0914.191.825</strong></span>
                            </div>
                            <div id="quoteSuccessBox" class="hidden p-3 rounded-lg bg-emerald-50 border border-emerald-200 text-emerald-800 text-xs font-medium"></div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ==================== 9. DANH MỤC CÁC BÀI VIẾT TRANG CHỦ ==================== -->
    <section id="bai-viet" class="py-5 md:py-7">
        <div class="flatsome-container">
            <div class="section-title-container">
                <h2 class="section-title-main text-sm sm:text-base md:text-lg">
                    BÀI VIẾT &amp; KINH NGHIỆM CHỌN GẠCH ỐP LÁT
                </h2>
                <span class="text-xs text-slate-500">Cẩm nang kiến trúc &amp; nội thất L.T.M Đà Nẵng</span>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                <!-- Bài viết 1 -->
                <article class="bg-white rounded-xl border border-slate-200 overflow-hidden shadow-xs hover:shadow-md transition flex flex-col">
                    <div class="aspect-[16/9] bg-slate-100 overflow-hidden">
                        <img 
                            src="https://lh3.googleusercontent.com/d/1uqL6ACCB5ne0G1BYkXCurdnrsf1m2lr4" 
                            onerror="this.src='https://drive.google.com/thumbnail?id=1uqL6ACCB5ne0G1BYkXCurdnrsf1m2lr4&sz=w600'"
                            alt="Xu hướng chọn gạch khổ lớn Đà Nẵng" 
                            class="w-full h-full object-cover hover:scale-105 transition duration-300"
                        >
                    </div>
                    <div class="p-4 flex-1 flex flex-col justify-between space-y-2">
                        <div class="space-y-1.5">
                            <span class="text-[11px] font-semibold text-ltm-gold uppercase">Xu hướng 2026</span>
                            <h3 class="text-sm font-bold text-ltm-primary leading-snug">
                                Kinh Nghiệm Chọn Gạch Lát Nền 80x80, 60x120 &amp; Gạch Khổ Lớn Cho Nhà Phố Đà Nẵng
                            </h3>
                            <p class="text-xs text-slate-600 leading-relaxed">
                                Bí quyết phối màu gạch vân đá Marble, chọn bề mặt bóng kiếng hay mờ Matt giúp phòng khách rộng thoáng, sang trọng và chống thấm ố vượt trội.
                            </p>
                        </div>
                        <button type="button" data-post="0" class="open-post-btn text-left text-xs font-bold text-ltm-secondary hover:text-ltm-gold pt-1">
                            Đọc chi tiết <i class="fa-solid fa-arrow-right ml-1"></i>
                        </button>
                    </div>
                </article>

                <!-- Bài viết 2 -->
                <article class="bg-white rounded-xl border border-slate-200 overflow-hidden shadow-xs hover:shadow-md transition flex flex-col">
                    <div class="aspect-[16/9] bg-slate-100 overflow-hidden">
                        <img 
                            src="https://lh3.googleusercontent.com/d/1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN" 
                            onerror="this.src='https://drive.google.com/thumbnail?id=1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN&sz=w600'"
                            alt="Gạch gỗ và gạch hoa trang trí" 
                            class="w-full h-full object-cover hover:scale-105 transition duration-300"
                        >
                    </div>
                    <div class="p-4 flex-1 flex flex-col justify-between space-y-2">
                        <div class="space-y-1.5">
                            <span class="text-[11px] font-semibold text-ltm-gold uppercase">Tư vấn nội thất</span>
                            <h3 class="text-sm font-bold text-ltm-primary leading-snug">
                                Ưu Điểm Của Gạch Vân Gỗ &amp; Gạch Hoa Cao Cấp Trong Khí Hậu Miền Trung
                            </h3>
                            <p class="text-xs text-slate-600 leading-relaxed">
                                Thay thế sàn gỗ tự nhiên dễ cong vênh ẩm mốc bằng gạch giả gỗ Porcelain chống nước 100%, kết hợp gạch bông trang trí tạo điểm nhấn nghệ thuật.
                            </p>
                        </div>
                        <button type="button" data-post="1" class="open-post-btn text-left text-xs font-bold text-ltm-secondary hover:text-ltm-gold pt-1">
                            Đọc chi tiết <i class="fa-solid fa-arrow-right ml-1"></i>
                        </button>
                    </div>
                </article>

                <!-- Bài viết 3 -->
                <article class="bg-white rounded-xl border border-slate-200 overflow-hidden shadow-xs hover:shadow-md transition flex flex-col">
                    <div class="aspect-[16/9] bg-slate-100 overflow-hidden">
                        <img 
                            src="https://lh3.googleusercontent.com/d/19k5uWHn_xeas2_BMP_JgBDwwu-IysSRP" 
                            onerror="this.src='https://drive.google.com/thumbnail?id=19k5uWHn_xeas2_BMP_JgBDwwu-IysSRP&sz=w600'"
                            alt="Thiết bị nhà tắm nhập khẩu Đà Nẵng" 
                            class="w-full h-full object-cover hover:scale-105 transition duration-300"
                        >
                    </div>
                    <div class="p-4 flex-1 flex flex-col justify-between space-y-2">
                        <div class="space-y-1.5">
                            <span class="text-[11px] font-semibold text-ltm-gold uppercase">Phòng tắm cao cấp</span>
                            <h3 class="text-sm font-bold text-ltm-primary leading-snug">
                                Giải Pháp Đồng Bộ Gạch Ốp Phòng Tắm &amp; Thiết Bị Vệ Sinh Nhập Khẩu Tại L.T.M
                            </h3>
                            <p class="text-xs text-slate-600 leading-relaxed">
                                Cách lựa chọn tủ Lavabo chống nước, bồn cầu liền khối men Nano kháng khuẩn và sen tắm nhiệt độ đồng bộ với gạch ốp tường 30x60, 60x120.
                            </p>
                        </div>
                        <button type="button" data-post="2" class="open-post-btn text-left text-xs font-bold text-ltm-secondary hover:text-ltm-gold pt-1">
                            Đọc chi tiết <i class="fa-solid fa-arrow-right ml-1"></i>
                        </button>
                    </div>
                </article>
            </div>
        </div>
    </section>

    <!-- ==================== 10. ĐƯA GOOGLE MAP & FANPAGE FACEBOOK RA NGOÀI TRANG CHỦ ==================== -->
    <section id="ban-do" class="py-5 md:py-7">
        <div class="flatsome-container">
            <div class="section-title-container">
                <h2 class="section-title-main text-sm sm:text-base md:text-lg">
                    BẢN ĐỒ GOOGLE MAPS &amp; FANPAGE CHÍNH THỨC L.T.M
                </h2>
                <span class="text-xs text-slate-500">Showroom: 28 Lương Trúc Đàm, Thanh Khê, Đà Nẵng</span>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-5">
                <!-- Cột Trái: Google Maps Trực Tiếp Ngoài Trang Chủ -->
                <div class="lg:col-span-7 bg-white rounded-xl border border-slate-200 p-3 sm:p-4 shadow-xs flex flex-col justify-between">
                    <div class="flex flex-wrap items-center justify-between gap-2 mb-3">
                        <div>
                            <h3 class="text-xs sm:text-sm font-bold text-ltm-primary">
                                <i class="fa-solid fa-map-location-dot text-ltm-gold mr-1.5"></i>VỊ TRÍ SHOWROOM TRÊN GOOGLE MAPS
                            </h3>
                            <p class="text-[11px] sm:text-xs text-slate-600">Địa chỉ: 28 Lương Trúc Đàm, Quận Thanh Khê, TP. Đà Nẵng</p>
                        </div>
                        <a href="https://share.google/9qG3KQ5P8u1OBtSPS" target="_blank" rel="noopener noreferrer" class="px-3 py-1.5 rounded-lg bg-ltm-primary hover:bg-ltm-secondary text-white text-xs font-semibold transition">
                            <i class="fa-solid fa-diamond-turn-right mr-1"></i>Mở Google Maps lớn
                        </a>
                    </div>
                    <div class="w-full h-[260px] sm:h-[310px] rounded-lg overflow-hidden border border-slate-200 bg-slate-100">
                        <iframe 
                            title="Google Map Công Ty TNHH TM & DV L.T.M - 28 Lương Trúc Đàm, Thanh Khê, Đà Nẵng"
                            src="https://maps.google.com/maps?q=28%20L%C6%B0%C6%A1ng%20Tr%C3%BAc%20%C4%90%C3%A0m,%20Thanh%20Kh%C3%AA,%20%C4%90%C3%A0%20N%E1%BA%B5ng&t=&z=16&ie=UTF8&iwloc=&output=embed"
                            class="w-full h-full border-0"
                            loading="lazy"
                            referrerpolicy="no-referrer-when-downgrade">
                        </iframe>
                    </div>
                </div>

                <!-- Cột Phải: Fanpage Facebook Đưa Ra Ngoài Trang Chủ -->
                <div class="lg:col-span-5 bg-white rounded-xl border border-slate-200 p-3 sm:p-4 shadow-xs flex flex-col justify-between">
                    <div>
                        <div class="flex items-center justify-between gap-2 mb-3">
                            <h3 class="text-xs sm:text-sm font-bold text-ltm-primary">
                                <i class="fa-brands fa-facebook text-[#1877F2] mr-1.5"></i>FANPAGE FACEBOOK CHÍNH THỨC
                            </h3>
                            <a href="https://www.facebook.com/profile.php?id=100046135087441" target="_blank" rel="noopener noreferrer" class="text-xs font-semibold text-[#1877F2] hover:underline">
                                Theo dõi trang <i class="fa-solid fa-arrow-up-right-from-square text-[10px]"></i>
                            </a>
                        </div>

                        <!-- Thẻ Fanpage Trực Quan Ngoài Trang Chủ -->
                        <div class="rounded-xl border border-slate-200 overflow-hidden bg-slate-50">
                            <!-- Ảnh bìa Fanpage -->
                            <div class="relative h-28 bg-gradient-to-r from-ltm-primary via-ltm-secondary to-[#1e3a8a] p-3 flex items-end">
                                <div class="flex items-center gap-3">
                                    <img 
                                        src="https://lh3.googleusercontent.com/d/1657a_RNzOWwdZGeDnC2P_1sW2SUH5Jia" 
                                        onerror="this.src='https://placehold.co/80x80/ffffff/12355b?text=LTM'"
                                        alt="Logo Fanpage L.T.M" 
                                        class="w-14 h-14 rounded-xl bg-white p-1 border-2 border-white shadow-md object-contain shrink-0"
                                    >
                                    <div class="text-white">
                                        <div class="font-bold text-xs sm:text-sm leading-tight">CÔNG TY TNHH TM &amp; DV L.T.M</div>
                                        <div class="text-[11px] text-amber-300">Gạch Ốp Lát &amp; Thiết Bị Nhà Tắm Đà Nẵng</div>
                                    </div>
                                </div>
                            </div>
                            <!-- Thông tin và hình ảnh thực tế trên Fanpage -->
                            <div class="p-3.5 space-y-3 text-xs">
                                <p class="text-slate-600 leading-relaxed">
                                    Cập nhật hàng ngày các mẫu <strong>gạch men, gạch hoa, gạch gỗ, gạch trang trí cao cấp và thiết bị nhà tắm nhập khẩu</strong> mới về tại kho 28 Lương Trúc Đàm, Thanh Khê, Đà Nẵng.
                                </p>
                                <div class="grid grid-cols-4 gap-1.5">
                                    <img src="https://lh3.googleusercontent.com/d/1P2fePSvPXm6YIcNDixVa0YwFWshcHFDY" onerror="this.src='https://drive.google.com/thumbnail?id=1P2fePSvPXm6YIcNDixVa0YwFWshcHFDY&sz=w200'" alt="Ảnh thực tế 1" class="w-full h-14 object-cover rounded">
                                    <img src="https://lh3.googleusercontent.com/d/171kMlCqYFeFpvYcgH1wQbaIMszY0Ns3O" onerror="this.src='https://drive.google.com/thumbnail?id=171kMlCqYFeFpvYcgH1wQbaIMszY0Ns3O&sz=w200'" alt="Ảnh thực tế 2" class="w-full h-14 object-cover rounded">
                                    <img src="https://lh3.googleusercontent.com/d/1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN" onerror="this.src='https://drive.google.com/thumbnail?id=1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN&sz=w200'" alt="Ảnh thực tế 3" class="w-full h-14 object-cover rounded">
                                    <img src="https://lh3.googleusercontent.com/d/19k5uWHn_xeas2_BMP_JgBDwwu-IysSRP" onerror="this.src='https://drive.google.com/thumbnail?id=19k5uWHn_xeas2_BMP_JgBDwwu-IysSRP&sz=w200'" alt="Ảnh thực tế 4" class="w-full h-14 object-cover rounded">
                                </div>
                                <div class="flex flex-wrap items-center gap-2 pt-1">
                                    <a href="https://www.facebook.com/profile.php?id=100046135087441" target="_blank" rel="noopener noreferrer" class="flex-1 text-center py-2 px-3 rounded-lg bg-[#1877F2] hover:bg-blue-700 text-white font-bold text-xs transition">
                                        <i class="fa-brands fa-facebook-f mr-1.5"></i>Truy Cập Fanpage L.T.M
                                    </a>
                                    <a href="https://zalo.me/0914191825" target="_blank" rel="noopener noreferrer" class="py-2 px-3 rounded-lg bg-slate-200 hover:bg-slate-300 text-slate-800 font-bold text-xs transition">
                                        Chat Zalo
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ==================== 11. FOOTER CHÂN TRANG CHUẨN FLATSOME ==================== -->
    <footer id="lien-he" class="bg-ltm-primary text-white mt-6 border-t-4 border-ltm-gold">
        <div class="flatsome-container py-8 md:py-10">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-12 gap-6">
                <!-- Cột 1: Thông tin công ty -->
                <div class="lg:col-span-5 space-y-3">
                    <div class="flex items-center gap-3">
                        <img 
                            src="https://lh3.googleusercontent.com/d/1657a_RNzOWwdZGeDnC2P_1sW2SUH5Jia" 
                            onerror="this.src='https://placehold.co/80x80/ffffff/12355b?text=LTM'"
                            alt="Logo CÔNG TY TNHH TM & DV L.T.M" 
                            class="w-11 h-11 rounded-lg bg-white p-1 object-contain shrink-0"
                        >
                        <div>
                            <div class="font-extrabold text-sm sm:text-base text-amber-300">CÔNG TY TNHH THƯƠNG MẠI VÀ DỊCH VỤ L.T.M</div>
                            <div class="text-xs text-slate-300">Website chính thức: ltm.com</div>
                        </div>
                    </div>
                    <p class="text-xs text-slate-200 leading-relaxed">
                        Chuyên phân phối Gạch ốp lát cao cấp Đà Nẵng: gạch men, gạch hoa, gạch gỗ, gạch khổ lớn, gạch trang trí cao cấp và thiết bị nhà tắm nhập khẩu chính hãng.
                    </p>
                    <ul class="space-y-1.5 text-xs text-slate-200">
                        <li><i class="fa-solid fa-location-dot text-amber-400 w-5"></i><strong>Địa chỉ:</strong> 28 Lương Trúc Đàm, Quận Thanh Khê, TP. Đà Nẵng</li>
                        <li><i class="fa-solid fa-phone text-amber-400 w-5"></i><strong>Điện thoại / Zalo:</strong> <a href="tel:0914191825" class="text-amber-300 font-bold">0914.191.825</a></li>
                        <li><i class="fa-solid fa-globe text-amber-400 w-5"></i><strong>Website:</strong> ltm.com</li>
                        <li><i class="fa-solid fa-map text-amber-400 w-5"></i><strong>Google Map:</strong> <a href="https://share.google/9qG3KQ5P8u1OBtSPS" target="_blank" rel="noopener noreferrer" class="underline hover:text-amber-300">Xem vị trí chỉ đường</a></li>
                    </ul>
                </div>

                <!-- Cột 2: Danh mục sản phẩm -->
                <div class="lg:col-span-4 space-y-2.5">
                    <h4 class="text-xs sm:text-sm font-bold uppercase text-amber-300 border-b border-white/15 pb-2">
                        DANH MỤC SẢN PHẨM CHÍNH
                    </h4>
                    <div class="grid grid-cols-2 gap-1.5 text-xs text-slate-200">
                        <a href="#san-pham-all" data-filter="gach-lat-nen" class="filter-trigger hover:text-amber-300 py-0.5 whitespace-nowrap">• Gạch Lát Nền 60x60</a>
                        <a href="#san-pham-all" data-filter="gach-lat-nen" class="filter-trigger hover:text-amber-300 py-0.5 whitespace-nowrap">• Gạch Lát Nền 80x80</a>
                        <a href="#san-pham-all" data-filter="gach-lat-nen" class="filter-trigger hover:text-amber-300 py-0.5 whitespace-nowrap">• Gạch Lát Nền 100x100</a>
                        <a href="#san-pham-all" data-filter="gach-op-tuong" class="filter-trigger hover:text-amber-300 py-0.5 whitespace-nowrap">• Gạch Ốp Tường 30x60</a>
                        <a href="#san-pham-all" data-filter="gach-op-tuong" class="filter-trigger hover:text-amber-300 py-0.5 whitespace-nowrap">• Gạch Ốp Tường 60x120</a>
                        <a href="#san-pham-all" data-filter="gach-op-tuong" class="filter-trigger hover:text-amber-300 py-0.5 whitespace-nowrap">• Gạch Ốp Tường 80x160</a>
                        <a href="#san-pham-all" data-filter="gach-kho-lon" class="filter-trigger hover:text-amber-300 py-0.5 whitespace-nowrap">• Gạch Khổ Lớn 1200x2400</a>
                        <a href="#san-pham-all" data-filter="gach-trang-tri" class="filter-trigger hover:text-amber-300 py-0.5 whitespace-nowrap">• Gạch Hoa &amp; Trang Trí</a>
                        <a href="#san-pham-all" data-filter="gach-go" class="filter-trigger hover:text-amber-300 py-0.5 whitespace-nowrap">• Gạch Vân Gỗ Cao Cấp</a>
                        <a href="#san-pham-all" data-filter="thiet-bi-nha-tam" class="filter-trigger hover:text-amber-300 py-0.5 whitespace-nowrap">• Thiết Bị Nhà Tắm</a>
                    </div>
                </div>

                <!-- Cột 3: Hỗ trợ khách hàng -->
                <div class="lg:col-span-3 space-y-2.5">
                    <h4 class="text-xs sm:text-sm font-bold uppercase text-amber-300 border-b border-white/15 pb-2">
                        KẾT NỐI VỚI L.T.M
                    </h4>
                    <p class="text-xs text-slate-200">
                        Liên hệ ngay qua Hotline, Zalo hoặc Fanpage để nhận bảng báo giá ưu đãi nhất cho công trình của bạn.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-1">
                        <a href="tel:0914191825" class="px-3 py-2 rounded-lg bg-amber-500 hover:bg-amber-600 text-white font-bold text-xs transition flex items-center gap-1.5">
                            <i class="fa-solid fa-phone"></i> 0914.191.825
                        </a>
                        <a href="https://www.facebook.com/profile.php?id=100046135087441" target="_blank" rel="noopener noreferrer" class="px-3 py-2 rounded-lg bg-[#1877F2] hover:bg-blue-700 text-white font-bold text-xs transition flex items-center gap-1.5">
                            <i class="fa-brands fa-facebook-f"></i> Fanpage
                        </a>
                    </div>
                </div>
            </div>
        </div>
        <div class="bg-[#0b223b] py-3 text-center text-[11px] text-slate-300 border-t border-white/10">
            <div class="flatsome-container">
                © Bản quyền thuộc về <strong>CÔNG TY TNHH THƯƠNG MẠI VÀ DỊCH VỤ L.T.M (ltm.com)</strong> • 28 Lương Trúc Đàm, Thanh Khê, Đà Nẵng.
            </div>
        </div>
    </footer>

    <!-- ==================== 12. CÁC NÚT LIÊN HỆ NỔI BẬT (ZALO, FACEBOOK, HOTLINE) TƯƠNG THÍCH MÁY TÍNH & ĐIỆN THOẠI ==================== -->
    <div class="fixed right-3 bottom-4 z-40 flex flex-col items-end gap-2.5">
        <!-- Nút Zalo nổi bật -->
        <a 
            href="https://zalo.me/0914191825" 
            target="_blank" 
            rel="noopener noreferrer" 
            aria-label="Chat Zalo 0914.191.825"
            class="group flex items-center gap-2 bg-[#0068ff] hover:bg-[#0052cc] text-white rounded-full p-2.5 sm:px-3.5 sm:py-2 shadow-lg transition"
        >
            <span class="w-6 h-6 rounded-full bg-white text-[#0068ff] font-extrabold text-[11px] flex items-center justify-center shrink-0">Zalo</span>
            <span class="hidden sm:inline text-xs font-bold whitespace-nowrap">Chat Zalo</span>
        </a>

        <!-- Nút Facebook Fanpage nổi bật -->
        <a 
            href="https://www.facebook.com/profile.php?id=100046135087441" 
            target="_blank" 
            rel="noopener noreferrer" 
            aria-label="Fanpage Facebook L.T.M"
            class="group flex items-center gap-2 bg-[#1877F2] hover:bg-blue-700 text-white rounded-full p-2.5 sm:px-3.5 sm:py-2 shadow-lg transition"
        >
            <span class="w-6 h-6 rounded-full bg-white text-[#1877F2] flex items-center justify-center shrink-0">
                <i class="fa-brands fa-facebook-f text-xs"></i>
            </span>
            <span class="hidden sm:inline text-xs font-bold whitespace-nowrap">Facebook</span>
        </a>

        <!-- Nút Hotline nổi bật -->
        <a 
            href="tel:0914191825" 
            aria-label="Gọi Hotline 0914.191.825"
            class="contact-pulse flex items-center gap-2 bg-red-600 hover:bg-red-700 text-white rounded-full p-2.5 sm:px-4 sm:py-2.5 shadow-xl transition"
        >
            <span class="w-6 h-6 rounded-full bg-white text-red-600 flex items-center justify-center shrink-0">
                <i class="fa-solid fa-phone-volume text-xs"></i>
            </span>
            <span class="text-xs font-extrabold whitespace-nowrap pr-1">0914.191.825</span>
        </a>
    </div>

    <!-- ==================== 13. MODAL XEM CHI TIẾT SẢN PHẨM & BÀI VIẾT ==================== -->
    <div id="productModal" class="fixed inset-0 z-50 hidden items-center justify-center p-3 sm:p-4 bg-slate-900/70 backdrop-blur-xs">
        <div class="bg-white rounded-2xl max-w-2xl w-full overflow-hidden shadow-2xl border border-slate-200 max-h-[90vh] flex flex-col">
            <div class="px-4 py-3 bg-ltm-primary text-white flex items-center justify-between">
                <h3 id="modalTitle" class="text-xs sm:text-sm font-bold truncate pr-2">Chi tiết sản phẩm</h3>
                <button id="closeProductModal" type="button" class="w-7 h-7 rounded-full bg-white/15 hover:bg-white/25 flex items-center justify-center text-white shrink-0">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
            <div id="modalBody" class="p-4 sm:p-5 overflow-y-auto"></div>
        </div>
    </div>

    <!-- ==================== JAVASCRIPT XỬ LÝ SẢN PHẨM, BANNER TỰ TRƯỢT, LỌC DANH MỤC & BÁO GIÁ ==================== -->
    <script>
        // Danh sách 19 sản phẩm thực tế lấy chính xác từ 19 file Google Drive của Công ty TNHH TM & DV L.T.M
        const LTM_PRODUCTS = [
            // Nhóm 1: Gạch Lát Nền & Gạch Ốp Tường Cao Cấp (6 ảnh đầu)
            {
                id: 'LTM-01',
                driveId: '1P2fePSvPXm6YIcNDixVa0YwFWshcHFDY',
                name: 'Gạch Lát Nền 80x80 Vân Đá Cẩm Thạch LTM-8801 Đà Nẵng',
                catSlug: 'gach-lat-nen',
                catLabel: 'GẠCH LÁT NỀN 80X80',
                oldPrice: '480.000 ₫',
                newPrice: '370.000 ₫',
                discount: '-23%',
                size: '800 x 800 mm',
                surface: 'Bóng kiếng toàn phần (Polished)',
                body: 'Xương đá Porcelain cao cấp',
                section: 'grid-lat-op'
            },
            {
                id: 'LTM-02',
                driveId: '11z7ir7cmqEcdrYuAThZvpOhgUVFsLUnP',
                name: 'Gạch Ốp Lát 60x120 Vân Đá Hoàng Gia LTM-61202 Đà Nẵng',
                catSlug: 'gach-op-tuong',
                catLabel: 'GẠCH 60X120',
                oldPrice: '530.000 ₫',
                newPrice: '415.000 ₫',
                discount: '-22%',
                size: '600 x 1200 mm',
                surface: 'Bóng kiếng Kim Cương',
                body: 'Xương đá Porcelain chống thấm',
                section: 'grid-lat-op'
            },
            {
                id: 'LTM-03',
                driveId: '1KTDzdSGqiXWuLZDkPoDD7oZZVL-5F3Rr',
                name: 'Gạch Ốp Tường 60x120 Vân Khói Xám Ý LTM-61203 Đà Nẵng',
                catSlug: 'gach-op-tuong',
                catLabel: 'GẠCH ỐP TƯỜNG 60X120',
                oldPrice: '460.000 ₫',
                newPrice: '360.000 ₫',
                discount: '-22%',
                size: '600 x 1200 mm',
                surface: 'Mờ Matt mịn sang trọng',
                body: 'Granite đồng chất',
                section: 'grid-lat-op'
            },
            {
                id: 'LTM-04',
                driveId: '1X31hmhpLVVORV-tmMSZYzBO-qtpyusry',
                name: 'Gạch Lát Nền 80x80 Vân Đá Trắng Ý LTM-8804 Đà Nẵng',
                catSlug: 'gach-lat-nen',
                catLabel: 'GẠCH LÁT NỀN 80X80',
                oldPrice: '450.000 ₫',
                newPrice: '355.000 ₫',
                discount: '-21%',
                size: '800 x 800 mm',
                surface: 'Bóng kiếng chống trầy',
                body: 'Porcelain cao cấp',
                section: 'grid-lat-op'
            },
            {
                id: 'LTM-05',
                driveId: '171kMlCqYFeFpvYcgH1wQbaIMszY0Ns3O',
                name: 'Gạch Ốp Lát 80x160 Vân Đá Tự Nhiên LTM-81605 Đà Nẵng',
                catSlug: 'gach-op-tuong',
                catLabel: 'GẠCH 80X160',
                oldPrice: '582.000 ₫',
                newPrice: '455.000 ₫',
                discount: '-22%',
                size: '800 x 1600 mm',
                surface: 'Siêu bóng Vi Tinh',
                body: 'Xương đá Porcelain',
                section: 'grid-lat-op'
            },
            {
                id: 'LTM-06',
                driveId: '1t8U7WQsmDbGWzmSelkxzjVv8M0BvIxAg',
                name: 'Gạch Men Lát Nền 60x60 Vân Đá Kem LTM-6606 Đà Nẵng',
                catSlug: 'gach-lat-nen',
                catLabel: 'GẠCH LÁT NỀN 60X60',
                oldPrice: '320.000 ₫',
                newPrice: '255.000 ₫',
                discount: '-20%',
                size: '600 x 600 mm',
                surface: 'Men bóng kháng khuẩn',
                body: 'Xương Bán Sứ / Porcelain',
                section: 'grid-lat-op'
            },

            // Nhóm 2: Gạch Khổ Lớn Cao Cấp (4 ảnh tiếp theo)
            {
                id: 'LTM-07',
                driveId: '1uqL6ACCB5ne0G1BYkXCurdnrsf1m2lr4',
                name: 'Gạch Khổ Lớn 1200x2400 Vân Đá Cẩm Thạch LTM-122401',
                catSlug: 'gach-kho-lon',
                catLabel: 'GẠCH KHỔ LỚN 1200X2400',
                oldPrice: '830.000 ₫',
                newPrice: '610.000 ₫',
                discount: '-27%',
                size: '1200 x 2400 mm',
                surface: 'Bóng kiếng cao cấp nhập khẩu',
                body: 'Xương đá Porcelain khổ lớn',
                section: 'grid-kho-lon'
            },
            {
                id: 'LTM-08',
                driveId: '1NwR4v0eypEtIwPi6NJVJCKoNCFFQ8G54',
                name: 'Gạch Khổ Lớn 1200x2400 Vân Đá Onyx LTM-122402 Đà Nẵng',
                catSlug: 'gach-kho-lon',
                catLabel: 'GẠCH KHỔ LỚN 1200X2400',
                oldPrice: '850.000 ₫',
                newPrice: '630.000 ₫',
                discount: '-26%',
                size: '1200 x 2400 mm',
                surface: 'Siêu bóng chiều sâu 3D',
                body: 'Xương đá Porcelain nhập khẩu',
                section: 'grid-kho-lon'
            },
            {
                id: 'LTM-09',
                driveId: '1_HXfxWiPLtWiayxMPjgFCsl1WS1wGb7h',
                name: 'Gạch Lát Nền Khổ Lớn 100x100 Vân Đá LTM-101001 Đà Nẵng',
                catSlug: 'gach-kho-lon',
                catLabel: 'GẠCH KHỔ LỚN 100X100',
                oldPrice: '640.000 ₫',
                newPrice: '495.000 ₫',
                discount: '-23%',
                size: '1000 x 1000 mm',
                surface: 'Bóng kiếng toàn phần',
                body: 'Granite cao cấp chịu lực',
                section: 'grid-kho-lon'
            },
            {
                id: 'LTM-10',
                driveId: '17YrxXteZmzhvVRYgfaklNGC2hKjN09N8',
                name: 'Gạch Khổ Lớn 1200x2800 Vân Đá Liên Tiếp LTM-122801',
                catSlug: 'gach-kho-lon',
                catLabel: 'GẠCH KHỔ LỚN 1200X2800',
                oldPrice: '1.850.000 ₫',
                newPrice: '1.450.000 ₫',
                discount: '-22%',
                size: '1200 x 2800 mm',
                surface: 'Men vi tinh kim cương',
                body: 'Xương đá nhập khẩu cao cấp',
                section: 'grid-kho-lon'
            },

            // Nhóm 3: Gạch Hoa, Gạch Vân Gỗ & Gạch Trang Trí Cao Cấp (5 ảnh tiếp theo)
            {
                id: 'LTM-11',
                driveId: '19jauCH_X7lcc0KNlu2OJ75CRiw3ArT7r',
                name: 'Gạch Hoa Trang Trí Nghệ Thuật Cao Cấp LTM-GH01 Đà Nẵng',
                catSlug: 'gach-trang-tri',
                catLabel: 'GẠCH HOA TRANG TRÍ',
                oldPrice: '420.000 ₫',
                newPrice: '330.000 ₫',
                discount: '-21%',
                size: '200 x 200 / 600 x 600 mm',
                surface: 'Men Matt chống trơn trượt',
                body: 'Porcelain họa tiết cổ điển',
                section: 'grid-trang-tri-go'
            },
            {
                id: 'LTM-12',
                driveId: '1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN',
                name: 'Gạch Vân Gỗ Tự Nhiên 15x90 Cao Cấp LTM-GG01 Đà Nẵng',
                catSlug: 'gach-go',
                catLabel: 'GẠCH VÂN GỖ 15X90',
                oldPrice: '390.000 ₫',
                newPrice: '310.000 ₫',
                discount: '-21%',
                size: '150 x 900 mm',
                surface: 'Vân gỗ sần tự nhiên chống trơn',
                body: 'Xương đá Porcelain chống ẩm',
                section: 'grid-trang-tri-go'
            },
            {
                id: 'LTM-13',
                driveId: '1vHG-pgeryaSItJoQ5ciiCGSWA7SJSU8c',
                name: 'Gạch Gỗ Ghép Xương Cá 15x80 LTM-GG02 Đà Nẵng',
                catSlug: 'gach-go',
                catLabel: 'GẠCH VÂN GỖ 15X80',
                oldPrice: '365.000 ₫',
                newPrice: '285.000 ₫',
                discount: '-22%',
                size: '150 x 800 mm',
                surface: 'Vân gỗ Sồi ấm cúng',
                body: 'Xương Granite bền màu',
                section: 'grid-trang-tri-go'
            },
            {
                id: 'LTM-14',
                driveId: '1X-ECML9CKN4ycBfVFu4pC0wnqzTS12CP',
                name: 'Gạch Trang Trí Terrazzo & Mosaic LTM-TT01 Đà Nẵng',
                catSlug: 'gach-trang-tri',
                catLabel: 'GẠCH TRANG TRÍ',
                oldPrice: '450.000 ₫',
                newPrice: '350.000 ₫',
                discount: '-22%',
                size: '600 x 600 mm',
                surface: 'Terrazzo hạt đá tinh tế',
                body: 'Xương đá Porcelain',
                section: 'grid-trang-tri-go'
            },
            {
                id: 'LTM-15',
                driveId: '1CGBZ4cuB7DMWadnoktlMoji6MB3dioC-',
                name: 'Gạch Bông & Gạch Hoa Điểm Nhấn LTM-GH02 Đà Nẵng',
                catSlug: 'gach-trang-tri',
                catLabel: 'GẠCH HOA CAO CẤP',
                oldPrice: '410.000 ₫',
                newPrice: '325.000 ₫',
                discount: '-21%',
                size: '300 x 600 / 600 x 600 mm',
                surface: 'Men Matt nghệ thuật',
                body: 'Porcelain chống bám bẩn',
                section: 'grid-trang-tri-go'
            },

            // Nhóm 4: Thiết Bị Nhà Tắm Nhập Khẩu (4 ảnh cuối)
            {
                id: 'LTM-16',
                driveId: '19k5uWHn_xeas2_BMP_JgBDwwu-IysSRP',
                name: 'Bộ Tủ Lavabo & Gương LED Phòng Tắm Nhập Khẩu LTM-TB01',
                catSlug: 'thiet-bi-nha-tam',
                catLabel: 'THIẾT BỊ NHÀ TẮM',
                oldPrice: '6.800.000 ₫',
                newPrice: '5.250.000 ₫',
                discount: '-23%',
                size: '800 x 500 mm',
                surface: 'Sứ tráng men Nano chống bám bẩn',
                body: 'Tủ PVC/Hợp kim chống nước 100%',
                section: 'grid-nha-tam'
            },
            {
                id: 'LTM-17',
                driveId: '1oah4j6YAPIsJacMYQFJ0JGVemrMwqCgf',
                name: 'Bồn Cầu Liền Khối Men Tuyết Nhập Khẩu LTM-TB02 Đà Nẵng',
                catSlug: 'thiet-bi-nha-tam',
                catLabel: 'BỒN CẦU NHẬP KHẨU',
                oldPrice: '5.500.000 ₫',
                newPrice: '4.200.000 ₫',
                discount: '-24%',
                size: '720 x 390 x 750 mm',
                surface: 'Men Nano kháng khuẩn siêu bóng',
                body: 'Xả xoáy Siphon êm mạnh',
                section: 'grid-nha-tam'
            },
            {
                id: 'LTM-18',
                driveId: '15IWAPhzVLsyUO5TDRoWXxvncrHoFcH1_',
                name: 'Chậu Rửa Lavabo Đặt Bàn Nghệ Thuật LTM-TB03 Đà Nẵng',
                catSlug: 'thiet-bi-nha-tam',
                catLabel: 'LAVABO CAO CẤP',
                oldPrice: '2.150.000 ₫',
                newPrice: '1.650.000 ₫',
                discount: '-23%',
                size: '480 x 370 x 140 mm',
                surface: 'Men sứ cao cấp chống ố vàng',
                body: 'Thiết kế hiện đại sang trọng',
                section: 'grid-nha-tam'
            },
            {
                id: 'LTM-19',
                driveId: '1WLKyUBxRc63xFN9GBUhFcqE0xPo0sQKh',
                name: 'Bộ Sen Cây Tắm Đứng Nóng Lạnh Nhập Khẩu LTM-TB04',
                catSlug: 'thiet-bi-nha-tam',
                catLabel: 'VÒI SEN TẮM',
                oldPrice: '3.900.000 ₫',
                newPrice: '2.950.000 ₫',
                discount: '-24%',
                size: 'Bát sen phím đàn mưa nhiệt đới',
                surface: 'Mạ PVD chống gỉ sét',
                body: 'Đồng thau nguyên chất 59A',
                section: 'grid-nha-tam'
            }
        ];

        // Tạo HTML cho từng thẻ sản phẩm chuẩn Flatsome (chỉ có duy nhất % giảm giá ở góc trên bên trái, tên sản phẩm đầy đủ không cắt chữ)
        function createProductCardHTML(product) {
            const primaryImg = `https://lh3.googleusercontent.com/d/${product.driveId}`;
            const backupImg = `https://drive.google.com/thumbnail?id=${product.driveId}&sz=w800`;
            const fallbackPlaceholder = `https://placehold.co/600x600/12355b/ffffff?text=${encodeURIComponent(product.id)}`;

            return `
                <div class="product-card group bg-white rounded-xl border border-slate-200 hover:border-ltm-primary shadow-xs hover:shadow-md transition flex flex-col justify-between overflow-hidden" data-cat="${product.catSlug}" data-name="${product.name.toLowerCase()}">
                    <div>
                        <!-- Khung ảnh sản phẩm + Badge % giảm giá góc trên bên trái chuẩn Flatsome -->
                        <div class="relative aspect-square w-full bg-slate-100 overflow-hidden cursor-pointer open-product-modal" data-id="${product.id}">
                            <span class="badge-circle-sale">${product.discount}</span>
                            <img 
                                src="${primaryImg}" 
                                onerror="if(!this.dataset.retry){this.dataset.retry='1';this.src='${backupImg}';}else{this.onerror=null;this.src='${fallbackPlaceholder}';}"
                                alt="${product.name}" 
                                loading="lazy"
                                class="w-full h-full object-cover group-hover:scale-105 transition duration-500"
                            >
                        </div>

                        <!-- Nội dung chữ dưới ảnh sản phẩm (Không bị tràn hoặc thiếu chữ) -->
                        <div class="p-2.5 sm:p-3.5 text-center space-y-1.5">
                            <div class="text-[10px] font-semibold uppercase tracking-wide text-slate-400">
                                ${product.catLabel}
                            </div>
                            <h3 class="product-title-text text-xs sm:text-sm font-bold text-slate-800 group-hover:text-ltm-primary transition cursor-pointer open-product-modal" data-id="${product.id}">
                                ${product.name}
                            </h3>
                        </div>
                    </div>

                    <!-- Giá gốc gạch ngang + Giá giảm chuẩn Flatsome -->
                    <div class="px-2.5 pb-3 sm:px-3.5 sm:pb-3.5 text-center space-y-2">
                        <div class="flex flex-wrap items-center justify-center gap-x-2 gap-y-0.5 text-xs sm:text-sm">
                            <del class="text-slate-400 text-[11px] sm:text-xs font-normal">${product.oldPrice}</del>
                            <span class="text-red-600 font-extrabold">${product.newPrice}</span>
                        </div>
                        <button type="button" data-id="${product.id}" class="open-product-modal w-full py-1.5 px-2 rounded-lg bg-slate-100 hover:bg-ltm-primary text-ltm-primary hover:text-white font-semibold text-[11px] sm:text-xs transition">
                            Xem chi tiết &amp; Báo giá
                        </button>
                    </div>
                </div>
            `;
        }

        // Hiển thị toàn bộ 19 sản phẩm vào các khung tương ứng
        function renderAllProducts() {
            const containers = {
                'grid-lat-op': document.getElementById('grid-lat-op'),
                'grid-kho-lon': document.getElementById('grid-kho-lon'),
                'grid-trang-tri-go': document.getElementById('grid-trang-tri-go'),
                'grid-nha-tam': document.getElementById('grid-nha-tam')
            };

            LTM_PRODUCTS.forEach(prod => {
                if (containers[prod.section]) {
                    containers[prod.section].insertAdjacentHTML('beforeend', createProductCardHTML(prod));
                }
            });
        }

        // Xử lý lọc sản phẩm theo danh mục & từ khóa tìm kiếm
        function filterProducts(categorySlug, searchQuery = '') {
            const cards = document.querySelectorAll('.product-card');
            const sections = document.querySelectorAll('.product-section');
            const statusBanner = document.getElementById('filterStatusBanner');
            const statusText = document.getElementById('filterStatusText');
            const cleanQuery = searchQuery.trim().toLowerCase();

            let visibleCount = 0;

            cards.forEach(card => {
                const cardCat = card.getAttribute('data-cat');
                const cardName = card.getAttribute('data-name');
                const matchCat = (categorySlug === 'all') || (cardCat === categorySlug);
                const matchSearch = (!cleanQuery) || cardName.includes(cleanQuery);

                if (matchCat && matchSearch) {
                    card.classList.remove('hidden');
                    visibleCount++;
                } else {
                    card.classList.add('hidden');
                }
            });

            // Ẩn các section trống khi đang lọc
            sections.forEach(sec => {
                const visibleInSec = sec.querySelectorAll('.product-card:not(.hidden)').length;
                if (visibleInSec === 0) {
                    sec.classList.add('hidden');
                } else {
                    sec.classList.remove('hidden');
                }
            });

            if (categorySlug !== 'all' || cleanQuery !== '') {
                statusBanner.classList.remove('hidden');
                statusText.textContent = cleanQuery 
                    ? `Kết quả tìm kiếm cho "${searchQuery}": ${visibleCount} sản phẩm`
                    : `Đang lọc theo danh mục (${visibleCount} sản phẩm thực tế)`;
            } else {
                statusBanner.classList.add('hidden');
            }
        }

        // Dữ liệu chi tiết bài viết
        const BLOG_POSTS = [
            {
                title: 'Kinh Nghiệm Chọn Gạch Lát Nền 80x80, 60x120 & Gạch Khổ Lớn Cho Nhà Phố Đà Nẵng',
                content: `
                    <p class="mb-3 text-xs sm:text-sm text-slate-700 leading-relaxed">
                        Khi hoàn thiện nhà phố hoặc biệt thự tại Đà Nẵng, việc lựa chọn kích thước và chất liệu gạch lát nền đóng vai trò quyết định đến độ sang trọng và tuổi thọ công trình:
                    </p>
                    <ul class="list-disc pl-5 space-y-2 text-xs sm:text-sm text-slate-700">
                        <li><strong>Phòng khách diện tích trên 25m2:</strong> Nên ưu tiên gạch khổ lớn 80x80cm, 60x120cm hoặc 1200x2400mm vân đá Cẩm Thạch giúp giảm thiểu đường ron và mở rộng không gian.</li>
                        <li><strong>Chất liệu xương gạch:</strong> Chọn gạch xương đá Porcelain hoặc Granite đồng chất tại L.T.M có độ hút nước dưới 0.5%, chống ố vàng và chịu lực cực tốt.</li>
                        <li><strong>Màu sắc:</strong> Tông trắng vân mây, kem sáng hoặc xám khói Ý đang là xu hướng chủ đạo năm 2026.</li>
                    </ul>
                `
            },
            {
                title: 'Ưu Điểm Của Gạch Vân Gỗ & Gạch Hoa Cao Cấp Trong Khí Hậu Miền Trung',
                content: `
                    <p class="mb-3 text-xs sm:text-sm text-slate-700 leading-relaxed">
                        Khí hậu miền Trung có mùa mưa ẩm kéo dài, do đó gạch giả gỗ (15x80, 15x90) và gạch bông/gạch hoa trang trí tại <strong>CÔNG TY TNHH TM & DV L.T.M</strong> được rất nhiều gia chủ lựa chọn:
                    </p>
                    <ul class="list-disc pl-5 space-y-2 text-xs sm:text-sm text-slate-700">
                        <li><strong>Chống nước và mối mọt 100%:</strong> Giữ nguyên vẻ đẹp ấm cúng của gỗ tự nhiên nhưng không lo cong vênh hay trầy xước.</li>
                        <li><strong>Gạch hoa & Terrazzo tạo điểm nhấn:</strong> Rất phù hợp ốp mảng tường bếp, giếng trời, ban công, quán cafe hoặc phòng tắm.</li>
                    </ul>
                `
            },
            {
                title: 'Giải Pháp Đồng Bộ Gạch Ốp Phòng Tắm & Thiết Bị Vệ Sinh Nhập Khẩu Tại L.T.M',
                content: `
                    <p class="mb-3 text-xs sm:text-sm text-slate-700 leading-relaxed">
                        Tại Showroom <strong>28 Lương Trúc Đàm, Thanh Khê, Đà Nẵng</strong>, khách hàng có thể chọn trọn bộ gạch ốp tường phòng tắm (30x60, 60x120) phối sẵn cùng thiết bị vệ sinh nhập khẩu:
                    </p>
                    <ul class="list-disc pl-5 space-y-2 text-xs sm:text-sm text-slate-700">
                        <li><strong>Tủ Lavabo & Gương LED chống ẩm:</strong> Chất liệu PVC/Hợp kim cao cấp bền bỉ trong môi trường ẩm ướt.</li>
                        <li><strong>Bồn cầu 1 khối & Sen cây nóng lạnh:</strong> Lớp men Nano kháng khuẩn chống bám bẩn, tiết kiệm nước và dễ vệ sinh.</li>
                    </ul>
                `
            }
        ];

        window.addEventListener('DOMContentLoaded', () => {
            renderAllProducts();

            // 1. Điều khiển Banner Slider tự trượt 2 ảnh bằng nhau
            const slides = document.querySelectorAll('.banner-slide');
            const dots = document.querySelectorAll('.banner-dot');
            let currentSlide = 0;

            function showSlide(index) {
                currentSlide = (index + slides.length) % slides.length;
                slides.forEach((slide, idx) => {
                    if (idx === currentSlide) {
                        slide.classList.remove('opacity-0', 'z-0');
                        slide.classList.add('opacity-100', 'z-10');
                    } else {
                        slide.classList.remove('opacity-100', 'z-10');
                        slide.classList.add('opacity-0', 'z-0');
                    }
                });
                dots.forEach((dot, idx) => {
                    if (idx === currentSlide) {
                        dot.classList.add('w-6', 'bg-amber-400');
                        dot.classList.remove('w-2', 'bg-white/50');
                    } else {
                        dot.classList.remove('w-6', 'bg-amber-400');
                        dot.classList.add('w-2', 'bg-white/50');
                    }
                });
            }

            let bannerTimer = setInterval(() => showSlide(currentSlide + 1), 4500);

            function resetBannerTimer() {
                clearInterval(bannerTimer);
                bannerTimer = setInterval(() => showSlide(currentSlide + 1), 4500);
            }

            document.getElementById('prevBannerBtn').addEventListener('click', () => {
                showSlide(currentSlide - 1);
                resetBannerTimer();
            });
            document.getElementById('nextBannerBtn').addEventListener('click', () => {
                showSlide(currentSlide + 1);
                resetBannerTimer();
            });
            dots.forEach(dot => {
                dot.addEventListener('click', () => {
                    showSlide(parseInt(dot.getAttribute('data-slide'), 10));
                    resetBannerTimer();
                });
            });

            // 2. Xử lý Mobile Menu Drawer
            const mobileDrawer = document.getElementById('mobileDrawer');
            const openMobileMenu = () => mobileDrawer.classList.remove('hidden');
            const closeMobileMenu = () => mobileDrawer.classList.add('hidden');

            document.getElementById('mobileMenuBtn').addEventListener('click', openMobileMenu);
            document.getElementById('closeMobileDrawer').addEventListener('click', closeMobileMenu);
            document.getElementById('mobileDrawerOverlay').addEventListener('click', closeMobileMenu);
            document.querySelectorAll('.mobile-nav-link').forEach(link => {
                link.addEventListener('click', closeMobileMenu);
            });

            // 3. Xử lý Lọc Danh Mục và Tìm Kiếm
            document.querySelectorAll('.filter-trigger').forEach(btn => {
                btn.addEventListener('click', (e) => {
                    const cat = btn.getAttribute('data-filter') || 'all';
                    filterProducts(cat, '');
                    const prodSection = document.getElementById('san-pham-all');
                    if (prodSection && cat !== 'all') {
                        prodSection.scrollIntoView({ behavior: 'smooth', block: 'start' });
                    }
                });
            });

            document.getElementById('resetFilterBtn').addEventListener('click', () => {
                document.getElementById('desktopSearchInput').value = '';
                document.getElementById('mobileSearchInput').value = '';
                filterProducts('all', '');
            });

            const handleSearch = (inputEl) => {
                const q = inputEl.value;
                filterProducts('all', q);
                document.getElementById('san-pham-all').scrollIntoView({ behavior: 'smooth', block: 'start' });
            };

            document.getElementById('desktopSearchBtn').addEventListener('click', () => handleSearch(document.getElementById('desktopSearchInput')));
            document.getElementById('desktopSearchInput').addEventListener('keydown', (e) => {
                if (e.key === 'Enter') handleSearch(e.target);
            });
            document.getElementById('mobileSearchBtn').addEventListener('click', () => handleSearch(document.getElementById('mobileSearchInput')));
            document.getElementById('mobileSearchInput').addEventListener('keydown', (e) => {
                if (e.key === 'Enter') handleSearch(e.target);
            });

            // 4. Xử lý Modal Chi Tiết Sản Phẩm & Bài Viết
            const modal = document.getElementById('productModal');
            const modalTitle = document.getElementById('modalTitle');
            const modalBody = document.getElementById('modalBody');

            const closeModal = () => {
                modal.classList.add('hidden');
                modal.classList.remove('flex');
            };

            document.getElementById('closeProductModal').addEventListener('click', closeModal);
            modal.addEventListener('click', (e) => {
                if (e.target === modal) closeModal();
            });

            document.body.addEventListener('click', (e) => {
                const prodTrigger = e.target.closest('.open-product-modal');
                if (prodTrigger) {
                    const prodId = prodTrigger.getAttribute('data-id');
                    const prod = LTM_PRODUCTS.find(p => p.id === prodId);
                    if (prod) {
                        const primaryImg = `https://lh3.googleusercontent.com/d/${prod.driveId}`;
                        const backupImg = `https://drive.google.com/thumbnail?id=${prod.driveId}&sz=w800`;
                        modalTitle.textContent = prod.name;
                        modalBody.innerHTML = `
                            <div class="grid grid-cols-1 sm:grid-cols-12 gap-4 items-center">
                                <div class="sm:col-span-6 relative aspect-square rounded-xl overflow-hidden bg-slate-100 border border-slate-200">
                                    <span class="badge-circle-sale">${prod.discount}</span>
                                    <img src="${primaryImg}" onerror="this.src='${backupImg}'" alt="${prod.name}" class="w-full h-full object-cover">
                                </div>
                                <div class="sm:col-span-6 space-y-2.5 text-xs sm:text-sm">
                                    <div class="text-xs font-bold text-ltm-gold uppercase">${prod.catLabel} • Mã: ${prod.id}</div>
                                    <h4 class="text-sm sm:text-base font-extrabold text-ltm-primary">${prod.name}</h4>
                                    <div class="flex items-center gap-2 py-1">
                                        <del class="text-slate-400 text-xs">${prod.oldPrice}</del>
                                        <span class="text-red-600 font-extrabold text-base sm:text-lg">${prod.newPrice}</span>
                                    </div>
                                    <div class="bg-slate-50 p-3 rounded-lg border border-slate-200 space-y-1 text-xs text-slate-700">
                                        <div><strong>Kích thước:</strong> ${prod.size}</div>
                                        <div><strong>Bề mặt:</strong> ${prod.surface}</div>
                                        <div><strong>Chất liệu:</strong> ${prod.body}</div>
                                        <div><strong>Kho hàng:</strong> 28 Lương Trúc Đàm, Thanh Khê, Đà Nẵng</div>
                                    </div>
                                    <div class="pt-2 flex flex-wrap gap-2">
                                        <a href="tel:0914191825" class="flex-1 text-center py-2 px-3 rounded-lg bg-red-600 hover:bg-red-700 text-white font-bold text-xs">
                                            <i class="fa-solid fa-phone mr-1"></i>0914.191.825
                                        </a>
                                        <a href="https://zalo.me/0914191825" target="_blank" rel="noopener noreferrer" class="flex-1 text-center py-2 px-3 rounded-lg bg-[#0068ff] hover:bg-blue-700 text-white font-bold text-xs">
                                            Nhắn Zalo Báo Giá
                                        </a>
                                    </div>
                                </div>
                            </div>
                        `;
                        modal.classList.remove('hidden');
                        modal.classList.add('flex');
                    }
                }

                const postTrigger = e.target.closest('.open-post-btn');
                if (postTrigger) {
                    const postIdx = parseInt(postTrigger.getAttribute('data-post'), 10);
                    const post = BLOG_POSTS[postIdx];
                    if (post) {
                        modalTitle.textContent = post.title;
                        modalBody.innerHTML = `
                            <div class="space-y-3">
                                <h4 class="text-sm sm:text-base font-bold text-ltm-primary">${post.title}</h4>
                                ${post.content}
                                <div class="pt-3 border-t border-slate-200 flex items-center justify-between text-xs text-slate-600">
                                    <span>Tư vấn trực tiếp tại 28 Lương Trúc Đàm, Thanh Khê, Đà Nẵng</span>
                                    <a href="tel:0914191825" class="font-bold text-ltm-primary">Hotline: 0914.191.825</a>
                                </div>
                            </div>
                        `;
                        modal.classList.remove('hidden');
                        modal.classList.add('flex');
                    }
                }
            });

            // 5. Xử lý Form Yêu Cầu Báo Giá Trang Chủ
            document.getElementById('quoteRequestForm').addEventListener('submit', (e) => {
                e.preventDefault();
                const name = document.getElementById('qName').value.trim();
                const phone = document.getElementById('qPhone').value.trim();
                const cat = document.getElementById('qCategory').value;
                const area = document.getElementById('qArea').value.trim();
                const successBox = document.getElementById('quoteSuccessBox');

                successBox.innerHTML = `
                    <i class="fa-solid fa-circle-check mr-1"></i>
                    Cảm ơn <strong>${name}</strong> (${phone})! Yêu cầu báo giá <strong>${cat}</strong> ${area ? `(${area})` : ''} đã được ghi nhận. Bộ phận kinh doanh <strong>CÔNG TY TNHH TM & DV L.T.M (0914.191.825)</strong> sẽ liên hệ tư vấn ngay!
                `;
                successBox.classList.remove('hidden');
                e.target.reset();
            });
        });
    </script>
</body>
</html>
