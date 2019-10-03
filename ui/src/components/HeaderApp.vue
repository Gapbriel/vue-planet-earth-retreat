<template>
	<div class="headerApp">

		<div class="title-container">
			<div class="title">Planet Earth Retreat</div>
		</div>

		<div id="nav">
			<ul class="nav justify-content-center">
				<li class="nav-item">
				<!-- <a class="nav-link active" href="#">Home</a> -->
				    <router-link class="nav-link active" to="/" style="width: 100%; height: 100%;">
          				Home
        			</router-link>
				</li>
				<li class="nav-item">
					<router-link class="nav-link" to="/retreats" style="width: 100%; height: 100%;">
          				Retreats
        			</router-link>
				</li>
				<li class="nav-item">
					<!-- <a class="nav-link" href="#">Gallery</a> -->
					<router-link class="nav-link" to="/gallery" style="width: 100%; height: 100%;">
          				Gallery
        			</router-link>
				</li>
				<li class="nav-item">
					<!-- <a class="nav-link" href="#">About</a> -->
					<router-link class="nav-link" to="/about" style="width: 100%; height: 100%;">
          				About
        			</router-link>
				</li>
				<li class="nav-item">
					<!-- <a class="nav-link" href="#">Contact</a> -->
					<router-link class="nav-link" to="/contact" style="width: 100%; height: 100%;">
          				Contact
        			</router-link>
				</li>
			</ul>
	    </div>
	</div>	
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue';

export default {
  name: 'headerApp'
};
</script>

<style lang="less" scoped>
	.headerApp{
		background: black;
		display: flex;
		justify-content: center;
		align-items: center;
		align-content: center;
		flex-wrap: wrap;
		.title-container{
			.title{
				font-size: 30px;
				font-weight: bold;
				color: #f9eb69;
				padding: 3% 10%;
				line-height: 1;
				text-transform: uppercase;
			}	
		}

		#nav{
			width: 100%;
			color: white;
			z-index: 1;
			background: black;
			* > {
				color: white;
			}
			.nav-item{
				.nav-link{
					padding: .5rem .7rem;
					text-transform: uppercase;
					font-size: .7em;
				}
			}
		}
	}
</style>
