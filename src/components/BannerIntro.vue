<script setup></script>

<template>
	<div class="content-bg">
		<div class="img-banner">
			<h2 class="p-3 ">Admin. Dashboard</h2>
			<p class="text">
				Tenemos la misión de ayudar a desarrolladores como usted a crear
				hermosos proyectos de forma gratuita.
			</p>
		</div>
	</div>
</template>

<style scoped>
.content-bg{
    width: 100%;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    width: 100%;
    position: relative;
    top: 0;
}

.img-banner{
    width: 100%;
    z-index: -10;
    background-image: url(../assets/title-bg.png);
    background-position: center center;
    background-repeat: no-repeat;
    background-size: cover;
    height: 300px;
    padding: 50px;
    max-height: 100%;
    min-height: 200px;
    color: var(--white);
}

.img-banner h2{
    font-size: 3rem;
    font-weight: bold;
}

.img-banner p{
    font-size: 22px;
    padding: 0 15px;
    font-weight: bold;
}
</style>
