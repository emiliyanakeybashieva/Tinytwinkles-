<!DOCTYPE html>
<html lang="bg">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Tiny Twinkles "Дизайн на онлайн магазин🛒"</title>
  <script src="https://cdn.tailwindcss.com"></script>

  <!-- ✅ AOS анимации -->
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
  <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
  <script>
    document.addEventListener('DOMContentLoaded', function () {
      AOS.init({
        duration: 800,
        easing: 'ease-in-out',
        once: true,
      });
    });
  </script>
</head>

<body class="bg-gray-50 text-gray-800">

  <!-- ✅ NAVBAR -->
  <nav class="bg-pink-100 p-4 shadow-md fixed w-full top-0 z-50" data-aos="fade-down">
    <div class="max-w-7xl mx-auto px-4 sm:px-4 lg:px-4">
      <div class="flex justify-between h-16 items-center">
        <div class="flex-shrink-0 text-xl font-bold text-pink-500">Tiny Twinkles🛒</div>
        <div class="hidden md:flex space-x-6 items-center">
          <a href="#" class="hover:text-pink-500 transition transform hover:scale-105">Начало</a>
          <a href="#" class="hover:text-pink-500 transition transform hover:scale-105">Продукти</a>
          <a href="#" class="hover:text-pink-500 transition transform hover:scale-105">Контакт</a>
         <div class="flex justify-between h-16 items-center">
        <div class="flex justify-between h-16 items-center">
        <div class="flex justify-between h-16 items-center">
         <div class="flex justify-between h-16 items-center">

        </div>
        <button onclick="toggleCart()" class="relative">
          <svg class="w-6 h-6 text-pink-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 7M7 13l-1.5 7h11L17 13M6 21a1 1 0 100-2 1 1 0 000 2zm12 0a1 1 0 100-2 1 1 0 000 2z" />
          </svg>
          <span id="cart-count"
            class="absolute -top-2 -right-2 bg-red-500 text-white text-xs w-5 h-5 flex items-center justify-center rounded-full"></span>
        </button>
        <button id="menu-btn" class="md:hidden focus:outline-none">
          <svg class="w-6 h-6 text-gray-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </button>
      </div>
    </div>
    <div id="mobile-menu" class="md:hidden hidden px-4 pb-4">
      <a href="#" class="block py-2 hover:text-pink-500">Начало</a>
      <a href="#" class="block py-2 hover:text-pink-500">Продукти</a>
      <a href="#" class="block py-2 hover:text-pink-500">Контакт</a>
    </div>
  </nav>

  <!-- ✅ HERO SECTION -->
  <section class="pt-20 bg-pink-100" data-aos="fade-up">
    <div class="max-w-6xl mx-auto text-center px-2 py-16">
      <h1 class="text-3xl font-bold text-black-600 mb-4">
        👶 Tiny Twinkles – любов в дрешки за най-малките. ✨🧸🍼 <br>
        С любов и грижа създаваме меки, качествени и сладки дрешки за най-малките съкровища.
      </h1>
      <p class="text-lg mb-6">Качество и стил за бебета – доставяме в България и UK 🛒</p>
      <a href="#" class="bg-pink-500 text-black-600 px-6 py-3 rounded-full hover:bg-pink-600 transition transform hover:scale-105">Разгледай продуктите</a>
    </div>
  </section>

  <!-- ✅ PRODUCTS SECTION -->
  <section class="max-w-8xl mx-auto px-4 py-12">
    <h2 class="text-2xl font-semibold mb-6 text-center" data-aos="fade-up">Нашите продукти</h2>
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">

      <!-- ✅ Продукт 1 -->
      <div class="bg-white rounded-lg shadow-md p-4" data-aos="zoom-in">
        <img src="https://cdncloudcart.com/10383/products/images/63718/rainy-bebeska-pelena-zajce-85h85-sm--copy-642d602c1031c_600x600.png?1680695454" alt="Одеяло" class="w-full rounded-md mb-3">
        <h3 class="font-semibold text-lg">Одеяло "Облаче"</h3>
        <p class="text-sm text-gray-500">Пухкаво и топло одеяло за сладки сънища.</p>
        <p class="text-pink-500 font-bold mt-2">19.99 лв</p>
        <button class="mt-4 bg-pink-500 text-white w-full py-2 rounded hover:bg-pink-600">Добави в количката</button>
      </div>

      <!-- ✅ Продукт 2 -->
      <div class="bg-white rounded-lg shadow-md p-4" data-aos="zoom-in">
        <img src="https://crazy-kids.bg/image/cache/data/products/bebe-girls/2025-s/1742-251/25-01742-048-L-4-800x800.jpg" alt="Бански" class="w-full rounded-md mb-3">
        <h3 class="font-semibold text-lg">Бебешки бански костюм</h3>
        <p class="text-sm text-gray-500">Mayoral с принт за момиче.</p>
        <p class="text-pink-500 font-bold mt-2">25.00 лв</p>
        <button class="mt-4 bg-pink-500 text-white w-full py-2 rounded hover:bg-pink-600">Добави в количката</button>
      </div>

      <!-- ✅ Продукт 3 -->
      <div class="bg-white rounded-lg shadow-md p-4" data-aos="zoom-in">
        <img src="https://tochici.bg/wp-content/uploads/2019/05/02605b_green-face.jpg" alt="Цял бански" class="w-full rounded-md mb-3">
        <h3 class="font-semibold text-lg">Бебешки цял бански</h3>
        <p class="text-sm text-gray-500">С къси ръкави и крачоли с рибка – зелен.</p>
        <p class="text-pink-500 font-bold mt-2">30.00 лв</p>
        <button class="mt-4 bg-pink-500 text-white w-full py-2 rounded hover:bg-pink-600">Добави в количката</button>
      </div>

      <!-- ✅ Продукт 4 -->
      <div class="bg-white rounded-lg shadow-md p-4" data-aos="zoom-in">
        <img src="https://www.store.bg/dcrimg/695788313/banski-za-momichence-little-dutch.jpg" alt="Бански" class="w-full rounded-md mb-3">
        <h3 class="font-semibold text-lg">Бебешки бански</h3>
        <p class="text-sm text-gray-500">Little Dutch</p>
        <p class="text-pink-500 font-bold mt-2">35.00 лв</p>
        <button class="mt-4 bg-pink-500 text-white w-full py-2 rounded hover:bg-pink-600">Добави в количката</button>
      </div>

      <!-- ✅ Продукт 5 -->
      <div class="bg-white rounded-lg shadow-md p-4" data-aos="zoom-in">
        <img src="https://cdncloudcart.com/21964/products/images/18565/detski-kasi-pantalonki-v-lilavo-s-kartinka-66642a52c61f4_1280x1280.jpeg?1717840494" alt="Панталонки" class="w-full rounded-md mb-3">
        <h3 class="font-semibold text-lg">Къси панталонки</h3>
        <p class="text-sm text-gray-500">В лилаво с картинка за момиче.</p>
        <p class="text-pink-500 font-bold mt-2">15.00 лв</p>
        <button class="mt-4 bg-pink-500 text-white w-full py-2 rounded hover:bg-pink-600">Добави в количката</button>
      </div>

      <!-- ✅ Продукт 6 -->
      <div class="bg-white rounded-lg shadow-md p-4" data-aos="zoom-in">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRcGdV1VcuJTrmJwJlp-0r4pgGBEFM4FgJFjw&s" alt="Панталонки" class="w-full rounded-md mb-3">
        <h3 class="font-semibold text-lg">Розови панталонки</h3>
        <p class="text-sm text-gray-500">За момиче</p>
        <p class="text-pink-500 font-bold mt-2">16.00 лв</p>
        <button class="mt-4 bg-pink-500 text-white w-full py-2 rounded hover:bg-pink-600">Добави в количката</button>
      </div>

    </div>
  </section>

  <!-- ✅ FOOTER -->
  <footer class="bg-pink-100 text-center py-6 text-sm text-pink-700" data-aos="fade-up">
    <div class="flex flex-col md:flex-row justify-center items-center gap-4">
      <a href="https://www.facebook.com/share/16dLukZNSi/" target="_blank"
        class="bg-blue-600 text-white px-4 py-2 rounded-lg shadow hover:bg-blue-700 transition">🔗 Facebook страница</a>
      <a href="mailto:emiemiliyana@gmail.com"
        class="bg-pink-500 text-sm text-white px-4 py-2 rounded-lg shadow hover:bg-pink-700 transition">📧 Пиши ми на имейл</a>
    </div>
    <p class="mt-4">© 2025 Tiny Twinkles. Всички права запазени.</p>
  </footer>

</body>
</html>

