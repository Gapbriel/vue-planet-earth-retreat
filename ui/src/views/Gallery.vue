<template>
  <section class="gallery">
    <h1>This is an gallery page</h1>
    <appSlider></appSlider>
  </section>
</template>
<script>
// import backgroundUrlImage from '../assets/20190825_183616.png'
 import appSlider from '@/components/AppSlider.vue';
export default {
  components: {appSlider},
  name: 'home',
  data(){
  	return{
  		
  	}
  },
  computed: {
    img1: function() {
        return require("../assets/home_img_2.png");
    },
    img2: function() {
        return require("../assets/home_img_1.png");
    }
  }
};

</script>