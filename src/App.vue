<template>
  <div id="app">    
    <app-header></app-header>
    <PageContent></PageContent>
    <app-footer></app-footer>
    
  </div>
</template>

<script>
//Registering components Locally
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import PageContent from './components/PageContent.vue'
export default {
  name: 'App',
  data(){
    return{
        itemsList: [{name:'Singapore Flyer',image:'./assets/SingaporeFlyer.jfif',show:false},
                    {name:'Art Science Museum',image:'/assets/ArtScienceMuseum.jfif',show:false},
                    {name:'Merlion',image:'/assets/Merlion.jfif',show:false},
                    {name:'Singapore River',image:'/assets/SingaporeRiver.jfif',show:false},
                    {name:'Gareden By The Bay',image:'/assets/GaredenByTheBay.jfif',show:false},
                    {name:'Jewel Changi',image:'/assets/JewelChangi.jfif',show:false}]
        }
  },
  components: {
    //Registering with a name
    'app-header':Header,
    'app-footer':Footer,
    //Registering without a name
    PageContent
  }
}
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  
}
</style>
