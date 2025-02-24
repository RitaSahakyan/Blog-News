<template>
    <header class="header">
      <img :src="headerImg" alt="" class="header_img" />
      <div class="header_content">
        <p class="header_heading">Статьи & Новости</p>
        <p class="header_text">Домой / Блог</p>
      </div>
    </header>
</template>

<script>
export default {
  name:"HeaderComponent",
  data(){
    return{
        headerImg: require('@/assets/BlogBackground.svg')
    }
  }
};
</script>

<style>
.header{
    height: 452px;
    margin-top: 45px;
    position: relative;
}
    .header_img{
        width: 100%;
        height: 356px;
        overflow: hidden;
    }
    .header_content{
      position: absolute;
        width: 503px;
        height: 274px;
        border-radius: 50px 50px 0 0;
        background-color: #ffffff;
        top: 39.5%;
        left: 41.5%;
    }
    .header_heading{
        font-size: 50px;
        margin-top: 41px;
        margin-left: 78px;
        color: #292F36 ;
        width: 347px;
        height: 126px;
    }
    .header_text{
        font-size: 22px;
        color: #4D5053;
        width: 105px;
        height: 66px;
        margin-left: 189px;
        margin-bottom: 41px;
    }

</style>