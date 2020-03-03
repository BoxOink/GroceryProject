<template>
  <div class="headerStyle">
    <footer>
        <p v-html="copyRtSymbol"></p>
                
    </footer>
    
  </div>
</template>

<script>
export default {
  
  data(){
    return{
        
        copyRtSymbol:'&copy;Boxin_BT3103'
        }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
footer{
    background:rgb(13, 87, 167);
    padding:10px;
    border-style: solid;
    border-color:black;
    border-width: 2px;
}
p{
    align-content: center;
    color:yellow;
}
</style>