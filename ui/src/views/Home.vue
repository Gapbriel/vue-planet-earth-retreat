<template>
	<section class="home">
		<div class="home_img1">
			<img :src="img1" class="rounded">
		</div>
		<div class="home_img2">
			<img :src="img2" class="rounded">
		</div>
	</section> 
</template>

<script>
// import backgroundUrlImage from '../assets/20190825_183616.png'
export default {
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
  },
};

</script>

<style lang="less" scoped> 
	.home{
		height: 100%;
		overflow: auto;
		img{
			width: 65vw;
			margin: 5%;
		}
	}
</style>
