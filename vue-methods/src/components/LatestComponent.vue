<template>
    <div id="app">
        
    <p class="late_heading container">Последний пост</p>
    <div class="latest container">
      <div class="latest_img">
        <img src="Img/latest.svg" alt="" class="latest_img-pic" />
      </div>
      <div class="latest_content">
        <p class="latest_content-heading">
          Low Cost Latest Invented Interior Designing Ideas
        </p>
        <p class="latest_content-text">
          С того времени этот, похожий на латинский, текст стал стандартом в
          печатной промышленности для примеров шрифтов и текстов. Перед
          появлением электронных издательств дизайнеры импровизировали в работе
          над макетами, изображая текст при помощи волнистых линий. С появлением
          самоклеющихся наклеек с напечатанным текстом «Lorem ipsum» появился
          более реалистичный способ обозначения расположения текста на странице.
        </p>
        <div class="latest_content-footer">
          <p class="latest_content-date">26 December,2022</p>
          <button class="latest_content-btn">
            <img src="Img/arrow.png" alt="" class="blog_articles-arrow" />
          </button>
        </div>
      </div>
    </div>
    </div>
</template>

<style>
.late_heading{
    font-size: 50px;
    color: #292F36;
    margin-top: 104px;
}

.latest {
    display: flex;
    margin-top: 27px;
    margin-bottom: 200px;
    height: 674px;
    margin-bottom: 88px;
}
    .latest_img{
        margin-top: 53px;
        margin-left: 22px;
    }

    .latest_content{
        width: 489px;
        height: 540px;
        margin-left: 65px;
        margin-top: 22px;
    }
        .latest_content-heading{
            color:#292F36;
            font-size: 25px;
            margin-bottom: 22px;
            letter-spacing: 2%;
            line-height: 125%;
            width: 440px;
        }
        .latest_content-text{
            color: #4D5053;
            font-size: 22px;
            margin-bottom: 50px;
            line-height: 150%;
            letter-spacing: 1%;
            width: 459px;
        }
        .latest_content-footer{
            display: flex;
            align-items: center;
            justify-content: space-between;
            width: 489px;
            height: 52px;
        }
        .latest_content-date{
            font-size: 16px;
            color: #4D5053;
        }
        .latest_content-btn{
            width: 52px;
            height: 52px;
            background-color: #F4F0EC;
            border-radius: 50%;
            border: none;
        }

</style>