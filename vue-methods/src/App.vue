<template>
  <div id="app">
    <AppHeader />
    <HeaderComponent />
    <LatestComponent />
    <BlogArticles />
    <PaginationComponent />
    <AppFooter />
  </div>
</template>

<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import BlogArticles from './components/BlogArticles.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import LatestComponent from './components/LatestComponent.vue';
import PaginationComponent from './components/PaginationComponent.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    HeaderComponent,
    LatestComponent,
    BlogArticles,
    PaginationComponent,
    AppFooter
  }
}
</script>

<style>
* {
    margin: 0;
    padding: 0;
    text-decoration: none;
}
body{
    background-color: #ffffff;
    font-family: "DM Serif Display", serif;
}
ul, li{
    list-style-type: none;
}

.box-content{
    overflow: hidden;
}
  .container {
    padding-left: calc(50% - 1200px / 2);
    padding-right: calc(50% - 1200px / 2);
}
</style>
