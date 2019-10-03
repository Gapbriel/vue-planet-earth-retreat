<template>
  <div id="app" :style="backImg">
    <header-app></header-app>
    <router-view/>
  </div>
</template>

<script>
    import headerApp from '@/components/HeaderApp.vue';
      
    export default {
      components:{headerApp},
      data(){
        return{
            backImg: {
                width: "100%",
                height: "100%",
                backgroundRepeat: "no-repeat",
                backgroundSize: "cover",
                backgroundPosition: "center center",
                backgroundBlendMode: "overlay",
                position: "fixed",
                backgroundImage : "url(" + require("./assets/" + '20190825_183616.png') + ")"
            }
        }
      }
    };

</script>

<style lang="less" scoped>
    #app {
      font-family: 'Avenir', Helvetica, Arial, sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      text-align: center;
      color: #2c3e50;
    }
</style>
