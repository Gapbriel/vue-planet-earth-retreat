<template>
	<carousel :perPageCustom="[[768, 2], [1024, 1]]">
	  <slide>
	    Slide 1 Content
	  </slide>
	  <slide>
	    Slide 2 Content
	  </slide>
</carousel>
</template>

<script>
// import backgroundUrlImage from '../assets/20190825_183616.png'
import { Carousel, Slide } from 'vue-carousel';
export default {
	// require styles

  name: 'app-slider',
  components: {
    Carousel,
    Slide
  },
  data(){
  	return{
  		   swiperOption: {
          scrollbar: {
            el: '.swiper-scrollbar',
            hide: true
          }
        }	
  	}
  },
  mounted() {

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

<style lang="less" scoped> 

</style>
