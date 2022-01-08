  <template>
    <div>
      <div class="about-container">
        <img class="img-about" src="https://static.vecteezy.com/system/resources/previews/001/226/460/non_2x/breaking-news-tv-background-vector.jpg" alt="Картинка о нас">
        <h1 class="name-about">Что мы такое? Кто мы такие? Что мы такие?!</h1>
        <div class="text-about">
          Мы рускоязычный новостной википортал, который рассказывает о новостях на различную тематику уже несколько лет! Рассказываем о том, о чем не стоит молчать, несмотря на цензуру.
          Оставайтесь с нами и будьте в курсе последних событий.
        </div>
        <h3>Контакты: +7-930-853-37-02</h3>
        <h3>Адрес: г.Белгород, ул. 5 Августа, д.44, кв.45</h3>
        <div class="text-about">
          Заходите на огонек! &#x1f525&#x1f525&#x1f525
        </div>
        <iframe class="map" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2533.5394777717925!2d36.57836431569275!3d50.57992547949339!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x41266a7ab80bc211%3A0xd7fc9ac427647622!2z0YPQuy4gNSDQkNCy0LPRg9GB0YLQsCwgNDQsINCR0LXQu9Cz0L7RgNC-0LQsINCR0LXQu9Cz0L7RgNC-0LTRgdC60LDRjyDQvtCx0LsuLCAzMDgwMjQ!5e0!3m2!1sru!2sru!4v1632497371947!5m2!1sru!2sru"></iframe>
      </div>
    </div>
  </template>

  <style>
    .about-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      position: relative;
      width: 70%;
      margin-left: 300px; /**/
      height: calc(100vh - 80px);
      overflow-y: scroll;
      padding-bottom: 20px;
      scrollbar-width: none; /* Для мозилы */
      background-color: white;
      border-radius: 10px;
      line-height: 24px;
    }

    /* для всех браузеров кроме мозилы */
    .about-container::-webkit-scrollbar {
      width: 0;
    }

    .text-about {
      margin: 10px 20px 15px 20px;
      font-size: 20px;
      align-items: end;
      font-weight: bolder;
    }
    .name-about {
      margin-top: 20px;
      font-size: 40px;
      margin-bottom: 20px;
    }

    .img-about {
      min-width: 100%;
      max-height: 500px;
      margin: 0;
      padding: 0;
    }

    .map {
      border: 0;
      min-height: 430px;
      min-width: 860px;
    }
  </style>
