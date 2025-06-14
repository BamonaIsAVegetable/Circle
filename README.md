# Circle


<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cycle - 校園二手交易平台</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@300;400;500;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Noto Sans TC', sans-serif;
            background-color: #f8f9fa;
        }
        .product-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }
    </style>
</head>
<body>
    <!-- 導航欄 -->
    <nav class="bg-emerald-600 text-white shadow-lg sticky top-0 z-50">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 4v5h.582m15.356 2A8.001 8.001 0 004.582 9m0 0H9m11 11v-5h-.581m0 0a8.003 8.003 0 01-15.357-2m15.357 2H15" />
                </svg>
                <span class="text-2xl font-bold">Cycle</span>
            </div>
            <div class="hidden md:flex items-center space-x-8">
                <a href="#" class="hover:text-emerald-200 transition">首頁</a>
                <a href="#" class="hover:text-emerald-200 transition">分類</a>
                <a href="#" class="hover:text-emerald-200 transition">關於我們</a>
                <a href="#" class="hover:text-emerald-200 transition">常見問題</a>
            </div>
            <div class="flex items-center space-x-4">
                <div class="relative">
                    <input type="text" placeholder="搜尋商品..." class="px-4 py-2 rounded-full text-gray-800 text-sm w-40 md:w-64 focus:outline-none focus:ring-2 focus:ring-emerald-500">
                    <button class="absolute right-3 top-2 text-gray-500">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" />
                        </svg>
                    </button>
                </div>
                <button class="bg-white text-emerald-600 px-4 py-2 rounded-full font-medium hover:bg-emerald-100 transition">登入/註冊</button>
                <button class="md:hidden">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                    </svg>
                </button>
            </div>
        </div>
    </nav>

    <!-- 英雄區塊 -->
    <div class="bg-gradient-to-r from-emerald-500 to-teal-400 text-white py-12 md:py-20">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-8 md:mb-0">
                    <h1 class="text-4xl md:text-5xl font-bold mb-4">校園二手交易的新選擇</h1>
                    <p class="text-xl mb-6">循環利用，環保省錢，讓閒置物品找到新主人</p>
                    <div class="flex space-x-4">
                        <button class="bg-white text-emerald-600 px-6 py-3 rounded-full font-medium hover:bg-emerald-50 transition">開始瀏覽</button>
                        <button class="border-2 border-white px-6 py-3 rounded-full font-medium hover:bg-white hover:text-emerald-600 transition">刊登物品</button>
                    </div>
                </div>
                <div class="md:w-1/2 flex justify-center">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-64 w-64" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M4 2a1 1 0 011 1v2.101a7.002 7.002 0 0111.601 2.566 1 1 0 11-1.885.666A5.002 5.002 0 005.999 7H9a1 1 0 010 2H4a1 1 0 01-1-1V3a1 1 0 011-1zm.008 9.057a1 1 0 011.276.61A5.002 5.002 0 0014.001 13H11a1 1 0 110-2h5a1 1 0 011 1v5a1 1 0 11-2 0v-2.101a7.002 7.002 0 01-11.601-2.566 1 1 0 01.61-1.276z" clip-rule="evenodd" />
                    </svg>
                </div>
            </div>
        </div>
    </div>

    <!-- 分類區塊 -->
    <div class="container mx-auto px-4 py-12">
        <h2 class="text-3xl font-bold text-center mb-8">熱門分類</h2>
        <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
            <div class="bg-white rounded-xl p-6 text-center shadow-md hover:shadow-lg transition cursor-pointer">
                <div class="bg-emerald-100 text-emerald-600 p-4 rounded-full w-16 h-16 flex items-center justify-center mx-auto mb-4">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253" />
                    </svg>
                </div>
                <h3 class="font-bold text-lg mb-1">教科書</h3>
                <p class="text-gray-600 text-sm">二手教科書、參考書</p>
            </div>
            <div class="bg-white rounded-xl p-6 text-center shadow-md hover:shadow-lg transition cursor-pointer">
                <div class="bg-emerald-100 text-emerald-600 p-4 rounded-full w-16 h-16 flex items-center justify-center mx-auto mb-4">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                    </svg>
                </div>
                <h3 class="font-bold text-lg mb-1">電子產品</h3>
                <p class="text-gray-600 text-sm">手機、電腦、配件</p>
            </div>
            <div class="bg-white rounded-xl p-6 text-center shadow-md hover:shadow-lg transition cursor-pointer">
                <div class="bg-emerald-100 text-emerald-600 p-4 rounded-full w-16 h-16 flex items-center justify-center mx-auto mb-4">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 15.546c-.523 0-1.046.151-1.5.454a2.704 2.704 0 01-3 0 2.704 2.704 0 00-3 0 2.704 2.704 0 01-3 0 2.704 2.704 0 00-3 0 2.704 2.704 0 01-3 0 2.701 2.701 0 00-1.5-.454M9 6v2m3-2v2m3-2v2M9 3h.01M12 3h.01M15 3h.01M21 21v-7a2 2 0 00-2-2H5a2 2 0 00-2 2v7h18zm-3-9v-2a2 2 0 00-2-2H8a2 2 0 00-2 2v2h12z" />
                    </svg>
                </div>
                <h3 class="font-bold text-lg mb-1">生活用品</h3>
                <p class="text-gray-600 text-sm">家具、廚具、日用品</p>
            </div>
            <div class="bg-white rounded-xl p-6 text-center shadow-md hover:shadow-lg transition cursor-pointer">
                <div class="bg-emerald-100 text-emerald-600 p-4 rounded-full w-16 h-16 flex items-center justify-center mx-auto mb-4">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 11V7a4 4 0 00-8 0v4M5 9h14l1 12H4L5 9z" />
                    </svg>
                </div>
                <h3 class="font-bold text-lg mb-1">服飾鞋包</h3>
                <p class="text-gray-600 text-sm">衣服、鞋子、背包</p>
            </div>
        </div>
    </div>

    <!-- 最新商品 -->
    <div class="bg-gray-50 py-12">
        <div class="container mx-auto px-4">
            <div class="flex justify-between items-center mb-8">
                <h2 class="text-3xl font-bold">最新上架</h2>
                <a href="#" class="text-emerald-600 hover:text-emerald-700 font-medium flex items-center">
                    查看全部
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 ml-1" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z" clip-rule="evenodd" />
                    </svg>
                </a>
            </div>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-6">
                <!-- 商品1 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-md product-card transition duration-300">
                    <div class="h-48 bg-emerald-100 relative">
                        <div class="absolute inset-0 flex items-center justify-center text-emerald-500">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-16 w-16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253" />
                            </svg>
                        </div>
                        <div class="absolute top-2 left-2 bg-emerald-500 text-white px-2 py-1 rounded-full text-xs">9成新</div>
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-1 truncate">微積分課本</h3>
                        <p class="text-gray-600 text-sm mb-2">理工學院適用，含習題解答</p>
                        <div class="flex justify-between items-center">
                            <span class="text-emerald-600 font-bold">$350</span>
                            <span class="text-gray-500 text-sm">3天前</span>
                        </div>
                    </div>
                </div>
                <!-- 商品2 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-md product-card transition duration-300">
                    <div class="h-48 bg-blue-100 relative">
                        <div class="absolute inset-0 flex items-center justify-center text-blue-500">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-16 w-16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                            </svg>
                        </div>
                        <div class="absolute top-2 left-2 bg-blue-500 text-white px-2 py-1 rounded-full text-xs">8成新</div>
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-1 truncate">iPad Air 4 64GB</h3>
                        <p class="text-gray-600 text-sm mb-2">附筆和保護套，電池健康度90%</p>
                        <div class="flex justify-between items-center">
                            <span class="text-emerald-600 font-bold">$12,000</span>
                            <span class="text-gray-500 text-sm">昨天</span>
                        </div>
                    </div>
                </div>
                <!-- 商品3 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-md product-card transition duration-300">
                    <div class="h-48 bg-purple-100 relative">
                        <div class="absolute inset-0 flex items-center justify-center text-purple-500">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-16 w-16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 11V7a4 4 0 00-8 0v4M5 9h14l1 12H4L5 9z" />
                            </svg>
                        </div>
                        <div class="absolute top-2 left-2 bg-purple-500 text-white px-2 py-1 rounded-full text-xs">全新</div>
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-1 truncate">北面後背包</h3>
                        <p class="text-gray-600 text-sm mb-2">25L容量，買錯尺寸，未使用過</p>
                        <div class="flex justify-between items-center">
                            <span class="text-emerald-600 font-bold">$1,800</span>
                            <span class="text-gray-500 text-sm">5天前</span>
                        </div>
                    </div>
                </div>
                <!-- 商品4 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-md product-card transition duration-300">
                    <div class="h-48 bg-amber-100 relative">
                        <div class="absolute inset-0 flex items-center justify-center text-amber-500">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-16 w-16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 15.546c-.523 0-1.046.151-1.5.454a2.704 2.704 0 01-3 0 2.704 2.704 0 00-3 0 2.704 2.704 0 01-3 0 2.704 2.704 0 00-3 0 2.704 2.704 0 01-3 0 2.701 2.701 0 00-1.5-.454M9 6v2m3-2v2m3-2v2M9 3h.01M12 3h.01M15 3h.01M21 21v-7a2 2 0 00-2-2H5a2 2 0 00-2 2v7h18zm-3-9v-2a2 2 0 00-2-2H8a2 2 0 00-2 2v2h12z" />
                            </svg>
                        </div>
                        <div class="absolute top-2 left-2 bg-amber-500 text-white px-2 py-1 rounded-full text-xs">7成新</div>
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-1 truncate">小型電鍋</h3>
                        <p class="text-gray-600 text-sm mb-2">適合宿舍使用，功能正常</p>
                        <div class="flex justify-between items-center">
                            <span class="text-emerald-600 font-bold">$500</span>
                            <span class="text-gray-500 text-sm">1週前</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- 平台特色 -->
    <div class="container mx-auto px-4 py-12">
        <h2 class="text-3xl font-bold text-center mb-12">為什麼選擇 Cycle？</h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <div class="bg-white p-6 rounded-xl shadow-md text-center">
                <div class="bg-emerald-100 text-emerald-600 p-4 rounded-full w-20 h-20 flex items-center justify-center mx-auto mb-4">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 9V7a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2m2 4h10a2 2 0 002-2v-6a2 2 0 00-2-2H9a2 2 0 00-2 2v6a2 2 0 002 2zm7-5a2 2 0 11-4 0 2 2 0 014 0z" />
                    </svg>
                </div>
                <h3 class="text-xl font-bold mb-3">校園專屬</h3>
                <p class="text-gray-600">專為校園師生設計，交易更安全可靠，買賣雙方身分有保障</p>
            </div>
            <div class="bg-white p-6 rounded-xl shadow-md text-center">
                <div class="bg-emerald-100 text-emerald-600 p-4 rounded-full w-20 h-20 flex items-center justify-center mx-auto mb-4">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
                    </svg>
                </div>
                <h3 class="text-xl font-bold mb-3">便捷交易</h3>
                <p class="text-gray-600">校內面交，省去運費與等待時間，當面交易更有保障</p>
            </div>
            <div class="bg-white p-6 rounded-xl shadow-md text-center">
                <div class="bg-emerald-100 text-emerald-600 p-4 rounded-full w-20 h-20 flex items-center justify-center mx-auto mb-4">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 15a4 4 0 004 4h9a5 5 0 10-.1-9.999 5.002 5.002 0 10-9.78 2.096A4.001 4.001 0 003 15z" />
                    </svg>
                </div>
                <h3 class="text-xl font-bold mb-3">環保永續</h3>
                <p class="text-gray-600">促進資源循環利用，減少浪費，為環保盡一份心力</p>
            </div>
        </div>
    </div>

    <!-- 刊登商品 CTA -->
    <div class="bg-emerald-600 text-white py-16">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-3xl font-bold mb-4">有閒置物品想賣掉嗎？</h2>
            <p class="text-xl mb-8 max-w-2xl mx-auto">只需簡單幾步驟，立即將您的二手物品刊登到 Cycle 平台上，讓它們找到新主人！</p>
            <button class="bg-white text-emerald-600 px-8 py-3 rounded-full font-medium text-lg hover:bg-emerald-50 transition">立即刊登商品</button>
        </div>
    </div>

    <!-- 頁腳 -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <div class="flex items-center space-x-2 mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 4v5h.582m15.356 2A8.001 8.001 0 004.582 9m0 0H9m11 11v-5h-.581m0 0a8.003 8.003 0 01-15.357-2m15.357 2H15" />
                        </svg>
                        <span class="text-2xl font-bold">Cycle</span>
                    </div>
                    <p class="text-gray-400">校園二手交易平台，讓閒置物品循環利用，創造更多價值。</p>
                </div>
                <div>
                    <h3 class="font-bold text-lg mb-4">快速連結</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition">首頁</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">瀏覽商品</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">刊登商品</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">我的帳戶</a></li>
                    </ul>
                </div>
                <div>
                    <h3 class="font-bold text-lg mb-4">幫助中心</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition">常見問題</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">使用條款</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">隱私政策</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">聯絡我們</a></li>
                    </ul>
                </div>
                <div>
                    <h3 class="font-bold text-lg mb-4">訂閱最新消息</h3>
                    <p class="text-gray-400 mb-4">獲取最新優惠和平台更新資訊</p>
                    <div class="flex">
                        <input type="email" placeholder="您的電子郵件" class="px-4 py-2 rounded-l-lg text-gray-800 w-full focus:outline-none">
                        <button class="bg-emerald-600 px-4 py-2 rounded-r-lg hover:bg-emerald-700 transition">訂閱</button>
                    </div>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 pt-8 text-center text-gray-400">
                <p>&copy; 2023 Cycle 校園二手交易平台. 保留所有權利。</p>
            </div>
        </div>
    </footer>

    <!-- 移動端選單 (預設隱藏) -->
    <div id="mobileMenu" class="fixed inset-0 bg-gray-900 bg-opacity-95 z-50 hidden">
        <div class="flex justify-end p-4">
            <button id="closeMenu" class="text-white">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                </svg>
            </button>
        </div>
        <div class="flex flex-col items-center text-white text-xl space-y-6 mt-12">
            <a href="#" class="hover:text-emerald-400 transition py-2">首頁</a>
            <a href="#" class="hover:text-emerald-400 transition py-2">分類</a>
            <a href="#" class="hover:text-emerald-400 transition py-2">關於我們</a>
            <a href="#" class="hover:text-emerald-400 transition py-2">常見問題</a>
            <a href="#" class="bg-emerald-600 px-8 py-3 rounded-full mt-4 hover:bg-emerald-700 transition">登入/註冊</a>
        </div>
    </div>

    <script>
        // 移動端選單功能
        const menuButton = document.querySelector('button.md\\:hidden');
        const mobileMenu = document.getElementById('mobileMenu');
        const closeMenu = document.getElementById('closeMenu');

        menuButton.addEventListener('click', () => {
            mobileMenu.classList.remove('hidden');
        });

        closeMenu.addEventListener('click', () => {
            mobileMenu.classList.add('hidden');
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'94f1a2f4625ff238',t:'MTc0OTgxODIxOC4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
