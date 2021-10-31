  <template>
    <div id="app">
      <div class="container">
      <img src="src/assets/logo.svg">
      <input type="text" placeholder="Ürün, kategori veya marka ara" name="searchBar" id="aramaKutusu">
      <a type="button" class="araBtn"><FontAwesomeIcon icon="search"></FontAwesomeIcon></a>
      <ul class="navBar">
        <li><a href="http://router.vuejs.org/" target="_blank"><FontAwesomeIcon icon="user-plus"></FontAwesomeIcon>Üye Ol</a></li>
        <li><a href="http://vuex.vuejs.org/" target="_blank"><FontAwesomeIcon icon="user"></FontAwesomeIcon>Üye Girişi</a></li>
        <li><a href="http://vue-loader.vuejs.org/" target="_blank"><FontAwesomeIcon icon="shopping-cart"></FontAwesomeIcon>Sepetim</a></li>
        <li><a href="https://github.com/vuejs/awesome-vue" target="_blank"><FontAwesomeIcon icon="paper-plane"></FontAwesomeIcon>Sipariş Takibi</a></li>
      </ul>
      <ul class="Menu">
        <li><a href="https://vuejs.org" target="_blank"><FontAwesomeIcon icon="ellipsis-v"></FontAwesomeIcon><FontAwesomeIcon icon="ellipsis-v"></FontAwesomeIcon><FontAwesomeIcon icon="ellipsis-v">
          </FontAwesomeIcon>Tüm Lensler</a></li>
        <li><a href="https://forum.vuejs.org" target="_blank">Saydam Lens</a></li>
        <li><a href="https://chat.vuejs.org" target="_blank">Günlük Lens</a></li>
        <li><a href="https://twitter.com/vuejs" target="_blank">Renkli Lens</a></li>
        <li><a href="https://vuejs.org" target="_blank">Toric Lens</a></li>
        <li><a href="https://forum.vuejs.org" target="_blank">İndirimli Lens</a></li>
        <li><a href="https://chat.vuejs.org" target="_blank">Solüsyonlar</a></li>
        <li><a href="https://twitter.com/vuejs" target="_blank">Göz Bakım</a></li>
        <li><a href="https://twitter.com/vuejs" target="_blank">Kampanyalar</a></li>
      </ul>
      </div>
    
    </div>
</template>

<script>
    import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
    import { library } from '@fortawesome/fontawesome-svg-core'
    import { fas } from '@fortawesome/free-solid-svg-icons'
    library.add(fas);
    export  default {
    name: 'app',
    data () {
      return {
        msg: 'Merhabalar Bu benim ilk başarılı uygulamam olabilir.'
      }
    },
    components:{
      FontAwesomeIcon
    }
  }
  </script>

  <style scoped>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;

    color: #2c3e50;
    margin-top: 60px;
  }

  h1, h2 {
    font-weight: normal;
    border:3px solid #2c3e50 ;
    background: red;
  }

  .navBar {
    display: inline-block;
    list-style-type: none;
    padding: 0;
    margin-left: 15px;
  }


  .navBar li {
    display: inline-block;
    margin: 0 5px;
  }

  .navBar li a {
    text-decoration: none;
    color: black;
  }
  .navBar li a:hover{
    color: orangered;
  }
  .container{ 
    width:90%;
    margin: 0 auto;
    text-align: center;
  }
  .container img{
    float: left;
    margin-left: 85px;
  }
  #aramaKutusu{
    display: inline-block;
    line-height: 30px;
    width: 30%;
    border: 1px solid orangered;
    border-radius: 3px;
  }
  #aramaKutusu{
    display: inline-block;
    line-height: 30px;
    width: 30%;
    border: 1px solid orangered;
    
    border-radius: 3px;
  }
  .araBtn{
    height: 33px;
   /* border: 1px solid orangered;
    border-radius: 3px;
    border-bottom-left-radius: 0  ;
    border-top-left-radius: 0;
    background: white;*/
    margin-left: -30px;
  }
  .araBtn:hover{
  cursor: pointer;
  }
  .Menu{
    border-top: 1px solid #e3e3e3;
    border-bottom: 1px solid #e3e3e3;
    padding: 15px 0;
    box-shadow: 0px 10px 18px 10px #e3e3e3;
  }
  .Menu li{
    border-left: 1px solid gray;
    padding-left: 15px;
    display: inline-block;
    margin: 0 5px;
  }
  .Menu li a{
    text-decoration: none;
    color: #2c3e50;
    font-weight: bold;
  }
  .Menu li a:hover{
    color:orangered;
  }

  </style>
