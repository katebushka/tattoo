<template>
  <div class="head">
    <TheHeader></TheHeader>
    <div class="hero container_all">
      <div>      
        <NuxtLink to="#order" class="btn btn__main">Записаться</NuxtLink>
      </div>
    </div>
  </div>
  <div class="content">
    <div class="container_all content__text" id="about">
      <h1>Привет, меня зовут Эля, я <span>тату-мастер</span> с художественным образованием из Санкт-Петербурга.</h1>
      <p>Если ты ищешь тату мастера, можешь больше не искать, я здесь. Я занимаюсь изобразительным искусством с 10 лет, закончила академию искусств и готова создать для тебя индивидуальный эскиз. Пиши и я создам шедевр на твоём теле</p>
      <SlideComponent></SlideComponent>
    </div>
  </div>
  <div class="content">
    <div class="container_all content__gallery content__text" id="gallery">
      <h2><span>Галлерея</span></h2>
      <h3>Мои работы</h3>
      <div class="content__gallery--box">
        <img src="/gallery/1.jpg" alt="">
        <img src="/gallery/2.jpg" alt="">
        <img src="/gallery/7.jpg" alt="">
        <img src="/gallery/5.jpg" alt="">
        <img src="/gallery/6.jpg" alt="">
        <img src="/gallery/9.jpg" alt="">
        <img src="/gallery/10.jpg" alt="">
      </div>
      <h3>Свободные эскизы</h3>
      <div class="content__gallery--box">
        <img src="/gallery/8.jpg" alt="">
        <img src="/gallery/3.jpg" alt="">
        <img src="/gallery/4.jpg" alt="">
        <img src="/gallery/11.jpg" alt="">
      </div>
    </div>
  </div>
  <div class="content">
    <div class="container_all content__price content__text" id="price">
      <h2><span>Прайс</span></h2>
      <ul>
        <li>
          <div>Разработка эскиза</div>
          <div class="line"></div>
          <div><b>бесплатно</b></div>
        </li>
        <li>
          <div>Черно-белое тату</div>
          <div class="line"></div>
          <div><b>от 2 000 руб.</b></div>
        </li>
        <li>
          <div>Цветное тату</div>
          <div class="line"></div>
          <div><b>от 3 000 руб.</b></div>
        </li>
        <li>
          <div>Аниме тату</div>
          <div class="line"></div>
          <div><b>от 2 000 руб.</b></div>
        </li>
      </ul>
      <p>Все расходные материалы одноразовые, а многоразовое оборудование проходит все этапы обработки, химическую, механическую и термическую.</p>
    </div>
  </div>
  <div class="content">
    <div class="container_all content__text" id="contacts">
      <h2><span>Контакты</span></h2>
      <div class="content__contacts">
        <div style="position:relative;overflow:hidden;margin:0 auto;">
          <NuxtLink to="https://yandex.ru/maps/2/saint-petersburg/?utm_medium=mapframe&utm_source=maps" style="color:#eee;font-size:12px;position:absolute;top:0px;">Санкт‑Петербург</NuxtLink>
          <NuxtLink to="https://yandex.ru/maps/2/saint-petersburg/geo/zhiloy_kompleks_bogatyr_3/4874569406/?ll=30.275969%2C59.994675&utm_medium=mapframe&utm_source=maps&z=17.21" style="color:#eee;font-size:12px;position:absolute;top:14px;">Жилой комплекс Богатырь 3 — Яндекс Карты</NuxtLink>
          <iframe src="https://yandex.ru/map-widget/v1/?ll=30.275969%2C59.994675&mode=search&ol=geo&ouri=ymapsbm1%3A%2F%2Fgeo%3Fdata%3DCgo0ODc0NTY5NDA2Es8B0KDQvtGB0YHQuNGPLCDQodCw0L3QutGCLdCf0LXRgtC10YDQsdGD0YDQsywg0J_RgNC40LzQvtGA0YHQutC40Lkg0YDQsNC50L7QvSwg0LzRg9C90LjRhtC40L_QsNC70YzQvdGL0Lkg0L7QutGA0YPQsyDQmtC-0LzQtdC90LTQsNC90YLRgdC60LjQuSDQkNGN0YDQvtC00YDQvtC8LCDQttC40LvQvtC5INC60L7QvNC_0LvQtdC60YEg0JHQvtCz0LDRgtGL0YDRjCAzIgoN8TTyQRXM-m9C&z=17.21" width="500" height="350" frameborder="1" allowfullscreen="true" style="position:relative;">
          </iframe>
          <div class="content__icons">
            <div class="line"></div>
            <div class="content__icons--item">
              <NuxtLink to="#">
                <svg xmlns="http://www.w3.org/2000/svg" width="40px" height="40px" viewBox="0 0 256 256"><defs><linearGradient id="logosTelegram0" x1="50%" x2="50%" y1="0%" y2="100%"><stop offset="0%" stop-color="#2AABEE"/><stop offset="100%" stop-color="#229ED9"/></linearGradient></defs><path fill="url(#logosTelegram0)" d="M128 0C94.06 0 61.48 13.494 37.5 37.49A128.038 128.038 0 0 0 0 128c0 33.934 13.5 66.514 37.5 90.51C61.48 242.506 94.06 256 128 256s66.52-13.494 90.5-37.49c24-23.996 37.5-56.576 37.5-90.51c0-33.934-13.5-66.514-37.5-90.51C194.52 13.494 161.94 0 128 0Z"/><path fill="#FFF" d="M57.94 126.648c37.32-16.256 62.2-26.974 74.64-32.152c35.56-14.786 42.94-17.354 47.76-17.441c1.06-.017 3.42.245 4.96 1.49c1.28 1.05 1.64 2.47 1.82 3.467c.16.996.38 3.266.2 5.038c-1.92 20.24-10.26 69.356-14.5 92.026c-1.78 9.592-5.32 12.808-8.74 13.122c-7.44.684-13.08-4.912-20.28-9.63c-11.26-7.386-17.62-11.982-28.56-19.188c-12.64-8.328-4.44-12.906 2.76-20.386c1.88-1.958 34.64-31.748 35.26-34.45c.08-.338.16-1.598-.6-2.262c-.74-.666-1.84-.438-2.64-.258c-1.14.256-19.12 12.152-54 35.686c-5.1 3.508-9.72 5.218-13.88 5.128c-4.56-.098-13.36-2.584-19.9-4.708c-8-2.606-14.38-3.984-13.82-8.41c.28-2.304 3.46-4.662 9.52-7.072Z"/></svg>
              </NuxtLink>
            </div>
            <div class="content__icons--item">
              <NuxtLink to="#">
                <svg xmlns="http://www.w3.org/2000/svg" width="40px" height="40px" xml:space="preserve" viewBox="0 0 256 256"><g fill="none" stroke-miterlimit="10" stroke-width="0"><path fill="#5181b8" d="M128 1C83 1 43 25 21 60c8 6 17 9 27 9h91c48 0 90 25 115 62v-3C254 58 198 1 128 1z"/><path fill="#4b76a7" d="M254 128v-10c-25-39-67-58-115-58H48c-9 0-17-1-24-4C11 75 3 97 2 121c25 31 64 51 107 51h2c26 0 37 12 38 37v-1c0 23-10 43-32 46h11c70 0 126-56 126-126z"/><path fill="#466d99" d="M117 254c23-3 40-22 41-45-1-25-21-46-47-46h-2c-43 0-81-19-107-50l-1 15c0 66 51 121 116 126z"/><path fill="#fff" d="M202 88c1-3 0-6-6-6h-16c-5 0-7 2-8 5 0 0-8 21-21 34-4 4-5 6-7 6s-3-2-3-5V88c0-4-1-6-5-6h-26c-3 0-5 2-5 4 0 4 6 5 7 16v25c0 6-1 7-3 7-6 0-20-21-28-45-2-5-3-7-8-7H56c-4 0-5 2-5 5 0 4 5 26 26 56 14 20 34 31 52 31 11 0 12-3 12-7v-15c0-5 1-6 4-6s7 1 17 11c12 12 14 17 20 17h17c5 0 7-3 6-7-2-5-7-12-15-20-3-5-9-10-11-12-3-4-2-5 0-8 0 0 20-29 23-39z"/></g></svg>
              </NuxtLink>
            </div>
            <div class="line"></div>
          </div>
        </div>
        <div class="content__form" id="order">
          <h4>Подать заявку</h4>
          <form>
            <input type="text" placeholder="Введите имя" required>
            <input type="number" name="" id="" placeholder="Введите номер телефона" required>
          </form>
          <button class="btn btn__main">Записаться</button>
        </div>
      </div>
      <div class="row">
        <h5>
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="16" viewBox="0 0 2e7 1.508e7">
            <path style="fill:#204982" d="m6026765 2907127c-299804-1015676-1113594-904356-1.67e6 -431300-1370626 1266075-3155291 3923495-2013094 7.75e6 956578 3241739 4936901 5314839 4936901 5314839h-4.64e6s-2395828-2685264-2.61e6 -5843500c-271260-3993020 1327930-6511332 3183988-8153020 1741824-1544365 3398006-2003480 3398006-2003480l3387831 1.11e7 3387831-1.11e7s1656182 459116 3398006 2003480c1856058 1641687 3455248 4.16e6 3183988 8153020-214173 3158236-2.61e6 5843500-2.61e6 5843500h-4.64e6s3.98e6 -2073100 4936900-5314839c1142197-3826069-642468-6483489-2013094-7.75e6 -556826-473056-1370617-584376-1.67e6 431300-1027971 3241740-3973210 1.253e7 -3973210 1.253e7s-2945239-9291363-3973210-1.253e7z"/>
          </svg>
          Пионерская
        </h5>
        <h5>
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="16" viewBox="0 0 2e7 1.508e7">
            <path style="fill:#520b5f" d="m6026765 2907127c-299804-1015676-1113594-904356-1.67e6 -431300-1370626 1266075-3155291 3923495-2013094 7.75e6 956578 3241739 4936901 5314839 4936901 5314839h-4.64e6s-2395828-2685264-2.61e6 -5843500c-271260-3993020 1327930-6511332 3183988-8153020 1741824-1544365 3398006-2003480 3398006-2003480l3387831 1.11e7 3387831-1.11e7s1656182 459116 3398006 2003480c1856058 1641687 3455248 4.16e6 3183988 8153020-214173 3158236-2.61e6 5843500-2.61e6 5843500h-4.64e6s3.98e6 -2073100 4936900-5314839c1142197-3826069-642468-6483489-2013094-7.75e6 -556826-473056-1370617-584376-1.67e6 431300-1027971 3241740-3973210 1.253e7 -3973210 1.253e7s-2945239-9291363-3973210-1.253e7z"/>
          </svg>
          Комендатский пр-т
        </h5>
        <h5>
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="16" viewBox="0 0 2e7 1.508e7">
            <path style="fill:#520b5f" d="m6026765 2907127c-299804-1015676-1113594-904356-1.67e6 -431300-1370626 1266075-3155291 3923495-2013094 7.75e6 956578 3241739 4936901 5314839 4936901 5314839h-4.64e6s-2395828-2685264-2.61e6 -5843500c-271260-3993020 1327930-6511332 3183988-8153020 1741824-1544365 3398006-2003480 3398006-2003480l3387831 1.11e7 3387831-1.11e7s1656182 459116 3398006 2003480c1856058 1641687 3455248 4.16e6 3183988 8153020-214173 3158236-2.61e6 5843500-2.61e6 5843500h-4.64e6s3.98e6 -2073100 4936900-5314839c1142197-3826069-642468-6483489-2013094-7.75e6 -556826-473056-1370617-584376-1.67e6 431300-1027971 3241740-3973210 1.253e7 -3973210 1.253e7s-2945239-9291363-3973210-1.253e7z"/>
          </svg>
          Старая деревня
        </h5>
      </div>
    </div>
  </div>
</template>