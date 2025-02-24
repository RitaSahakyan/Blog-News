<template>
  <div id="app">
    <p class="blogandnews_heading container">Статьи & Новости</p>
    <div class="blog container">
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


<style>

.blogandnews_heading{
    font-size: 50px;
    color: #292F36;
}
.blog{
    display: flex;
    margin-top: 27px;
    height: 1010px;
}
        .blog_info{
            margin-top: 12px;
            width: 481px;
            font-size: 22px;
            color: #4D5053;
        }
        .blog_articles{
            height: 521px;
            display: flex;
            gap: 20px;
            display: flex;
            flex-wrap: wrap;
        }
            .blog_articles-item{
                background-color: #FFFFFF;
                border: 1px solid #E7E7E7;
                border-radius: 15%;
                width: 382px;
            }
            .blog_articles-item:nth-child(2){
                border: 1px solid #E7E7E7;
                background-color: #F4F0EC;

            }

            .blog_articles-img 
            {
                padding: 21px 21px 21px 21px;
                display: flex;
                position: relative;
            }
                .blog_articles-img-Text{
                position: absolute;
                background-color: #FFFFFF;
                font-size: 16px;
                width: 129px;
                height: 40px;
                color: #4D5053;
                display: flex;
                align-items: center;
                justify-content: center;
                margin-left: 40px;
                margin-top: -90px;
                border-radius: 10px 10px 10px 0;
            }
            .blog_articles-heading{
                font-size: 25px;
                color: #292F36;
                margin: 0 21px;
            }
            .blog_articles-footer{
                margin: 30px 21px 21px 21px;
                display: flex;
                align-items: center;
                justify-content: space-between;
            }
            .blog_articles-text{
                font-size: 16px;
                color: #4D5053;
            }
            .blog_articles-btn{
                width: 52px;
                height: 52px;
                background-color: #F4F0EC;
                border-radius: 50%;
                border: none;
            }
            .blog_articles-btn:nth-child(2){
                background-color: #FFFFFF;
            }
</style>
  