<template>
  <div>
    <div class="list-content">
      <NewsElement title="Козлов в Minecraft озвучили настоящие козлы"
                   link="Content"
                   imageSrc="https://cdn.igromania.ru/mnt/news/e/8/e/5/9/f/108916/700c43bd51675b31_848x477.jpg"
                   imageAlt="Новостная картинка"/>

      <NewsElement title="Новая распродажа в Steam — Detroit: Become Human, Call of Duty, SOMA, SCUM и не только"
                   link="Content"
                   imageSrc="https://cdn.igromania.ru/mnt/news/9/1/1/d/9/f/108920/9d971f40462a90e1_848x477.jpg"
                   imageAlt="Новостная картинка"/>

      <NewsElement title="Mafia: Definitive Edition запустили на PC с GeForce RTX 3090 в 8K"
                   link="Content"
                   imageSrc="https://cdn.igromania.ru/mnt/news/1/b/f/f/3/9/108923/9cc66d0d42b4dd2c_848x477.jpg"
                   imageAlt="Новостная картинка"/>

      <NewsElement title="Кража Пламени Востока, бонусы и преступления — в свежем обновлении Red Dead Online"
                   link="Content"
                   imageSrc="https://cdn.igromania.ru/mnt/news/b/7/f/b/8/7/108940/e9acd8d1cf677533_848x477.jpg"
                   imageAlt="Новостная картинка"/>

      <NewsElement title="В свежем трейлере Diablo II: Resurrected снялся звезда «Шан-Чи и легенды десяти колец»"
                   link="Content"
                   imageSrc="https://cdn.igromania.ru/mnt/news/0/4/b/1/d/b/108937/be1157e2ec319f94_848x477.jpg"
                   imageAlt="Новостная картинка"/>

      <NewsElement title="После очередного иска из Blizzard ушла главный юрисконсульт"
                   link="Content"
                   imageSrc="https://cdn.igromania.ru/mnt/news/9/7/7/5/3/3/108927/2b087d0a19e7e8c3_848x477.jpg"
                   imageAlt="Новостная картинка"/>

      <NewsElement title="Новая трилогия «Звёздных войн» разгневала Марсию Лукас"
                   link="Content"
                   imageSrc="https://cdn.igromania.ru/mnt/news/a/4/5/f/f/a/108924/221155b5887d85d0_848x477.jpg"
                   imageAlt="Новостная картинка"/>
    </div>
  </div>
</template>

<script>
import NewsElement from "../components/NewsElement";

export default {
  name: 'Home',
  components: {
    NewsElement
  }
}
</script>

<style>
.list-content {
  flex-direction: column;
  align-items: end;
  position: relative;
  width: 30%;
  margin-left: 400px; /**/
  height: calc(100vh - 80px);
  overflow-y: scroll;
  padding-bottom: 20px;
  scrollbar-width: none; /* Для мозилы */
}

/* для всех браузеров кроме мозилы */
.list-content::-webkit-scrollbar {
  width: 0;
}

</style>
