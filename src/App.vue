<template>
  <div id="app">
    <div>
      <router-view/>
    </div>
    
    <footer>
      <ul>
          <router-link tag="li" :to="{name: 'HomePage'}"><i class="fa fa-home"></i><span>首页</span> </router-link>
          <router-link tag="li" :to="{name: 'Classify'}"><i class="fa fa-table"></i><span>分类</span></router-link>
          <router-link tag="li" :to="{name: 'Shopcart'}"><i class="fa fa-shopping-cart"></i><span>购物车</span></router-link>
          <router-link tag="li" :to="{name: 'Personal'}"><i class="fa fa-user"></i><span>个人</span></router-link>
      </ul>
    </footer>
      
  </div>
 
</template>

<script>
import 'fontIcon'
export default {
  name: 'App'
}
</script>


<style>
  body, h1, h2, h3, h4, h5, h6, p, ul, li, input, button, img { margin: 0; padding: 0;}
  html, body { width: 100%; height: 100%; }

  a   { text-decoration: none; }
  ul  { list-style: none; }
  img { vertical-align: middle; }
  input, button { outline: none; }

  .fl { float: left;}
  .fr { float: right;}
  .clearFix { zoom: 1; }
  .clearFix:after { content: ''; display: block; height: 0; visibility: hidden; clear: both; }

  .flex-center { display: flex; display: -webkit-flex; justify-content: center; align-items: center; flex-wrap: wrap; }
  #app{
    position: relative;
    width: 100%;
    height: 100%
  }
  footer{
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 55px;
    border-top: 1px solid lightgray
  }
  ul{
    display: flex
  }
  li{
    width: 25%;
    height: 55px;
    text-align: center;
    padding-top: 3px
  }
  .fa{
    font-size: 31px;
    color: gray
  }
  span{
    display: block 
  }
</style>
