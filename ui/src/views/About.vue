<template>
  <section class="about h-100 w-100">
    <div class="about-video_container h-100 w-100">
    	<iframe src="https://www.youtube.com/embed/roTqa0EaZM4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
  </section>
</template>

<script>
// import backgroundUrlImage from '../assets/20190825_183616.png'
export default {
  name: 'about',
  data(){
  	return{
  		
  	}
  },
  computed: {
  }
};

</script>

<style lang="less" scoped> 
	.about{
		.about-video_container{
			iframe,
			object,
			embed {
				position: relative;
				top:25px;
				width: 85%;
				height: 75%;
			}

		}
	}
</style>