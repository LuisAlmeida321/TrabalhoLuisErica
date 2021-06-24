<template>
<div class="background">
	<img src="../assets/wallpapersdendino.jpg" alt="auto">
</div>

</template>

<style scoped>

/* .background{} */


/* Generic */

body {
	width: 100%;
	height: 100vh;
	display: flex;
	justify-content: center;
	align-items: flex-end;
	overflow: hidden;
	background-image: linear-gradient(135deg, #070437, #000);
}

.main {
	position: relative;
	width: 60vw;
	height: 45vw;
}

.filter {
	position: absolute;
	width: 100%;
	height: 100%;
	background-image: linear-gradient(110deg, #04021f 32%, transparent 50%);
	z-index: 4000;
}

.light {
	position: absolute;
	top: 0;
	left: 50vw;
	width: 50vw;
	height: 100vh;
	z-index: 2000;
	transform: skewX(20deg) translate(-30%);
	background-image: linear-gradient(to bottom, rgba(236, 232, 214, .15), rgba(236, 232, 214, .035), transparent);
	filter: blur(2vw);
	z-index: 5000;
}

@media (max-width: 600px) {
	.light {
		left: 30vw;
		width: 70vw;
	}
}

</style>

<script>

export default {

  name: "erro",

  components: {},

};

</script>