<template>
  <div>
    <div class="content">
      <h1>Козлов в Minecraft озвучили настоящие козлы</h1>
      <img class="content-image" src="https://cdn.igromania.ru/mnt/news/e/8/e/5/9/f/108916/700c43bd51675b31_848x477.jpg" alt="Новостная картинка">
      <div class="content-text">
        В серии роликов <strong>The Secrets of Minecraft </strong>
        на YouTube создатели
        <strong>Minecraft</strong>
        &nbsp;рассказали, что козлов в игре озвучивали реальные козлы. Точнее &nbsp;— использовались голоса людей в сочетании с блеянием коз в соотношении 50 на 50.
      </div>
      <div class="content-text">
        Козий крик вдохновлён смешными звуками, которые издают козы — в конце 2000-х подобные ролики набирали несколько миллионов просмотров. Иногда животные кричат будто люди. Выглядит и звучит это примерно
        <a href="https://www.youtube.com/watch?v=PpccpglnNf0" target="_blank">так</a>.
      </div>
      <div class="content-text">
        Видео The Secrets of Minecraft посвящены обновлению
        <strong>Caves Cliffs</strong>, первая часть которого вышла летом, а вторая появится зимой.
      </div>
      <iframe width="560" height="315" src="https://www.youtube.com/embed/aKQ4bdqJUxc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      <div class="nepncont">
        <div>
          <router-link :to="{name: 'Home'}">Назад</router-link>
        </div>
        <div>
          <router-link :to="{name: 'Home'}">Вперед</router-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style>
  .content {
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
    box-shadow: rgb(255 255 255) 2px 2px 2px;
    line-height: 24px;
  }

  /* для всех браузеров кроме мозилы */
  .content::-webkit-scrollbar {
    width: 0;
  }

  .content-text {
    margin: 10px 20px 15px 20px;
    font-size: 20px;
    align-items: end;
  }

  .content h1 {
    font-size: 30px;
    font-weight: 700;
    line-height: 34px;
    margin-bottom: 15px;
  }

  .content-image {
    max-height: 600px;
    max-width: 900px;
  }

  .content iframe {
    width: 848px;
    min-height: 477px;
    margin: 0 0 23px -23px;
  }

  .nepncont {
    margin: 0;
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-column-gap: 1000px;
  }

  .nepncont div a {
    color: #8f8e94;
    text-decoration: none;
    font-size: 18px;
    font-weight: 700;
    text-transform: uppercase;
    display: inline-block;
  }

  .nepncont div a:hover {
    color:darkred;
  }
</style>
