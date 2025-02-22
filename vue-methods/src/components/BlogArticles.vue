<template>
  <div id="app">
    <div class="blog_articles">
      <article v-for="(article, index) in articles" :key="index" class="blog_articles-item">
        <img :src="`/Img/News${index + 1}.svg`" alt="" class="blog_articles-img" />
        <div class="blog_articles-img-Text">{{ article.category }}</div>
        <div class="blog_articles-heading">{{ article.title }}</div>
        <div class="blog_articles-footer">
          <div class="blog_articles-text">{{ article.date }}</div>
          <button class="blog_articles-btn">
            <img src="/Img/arrow.png" alt="" class="blog_articles-arrow" />
          </button>
        </div>
      </article>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      articles: [
        { category: "Дизайн кухни", title: "Создадим лучший макет перепланировки", date: "26 Декабрь,2022" },
        { category: "Дизайн для жизни", title: "Лучшие интерьерные идеи по низкой цене", date: "22 Декабрь, 2022" },
        { category: "Дизайн Интерьера", title: "Лучшие интерьерные решения для офисов", date: "25 Декабрь,2022" },
        { category: "Дизайн кухни", title: "Создадим лучший макет перепланировки", date: "26 Декабрь,2022" },
        { category: "Дизайн для жизни", title: "Лучшие интерьерные идеи по низкой цене", date: "22 Декабрь, 2022" },
        { category: "Дизайн Интерьера", title: "Лучшие интерьерные решения для офисов", date: "25 Декабрь,2022" }
      ]
    };
  }
};
</script>
  