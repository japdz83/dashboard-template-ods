<script setup>
import { RouterLink, RouterView } from 'vue-router'
import SideBar from './components/SideBar.vue'
import Navbar from './components/Navbar.vue'
</script>

<template>
	<div class="wrapper">
		<SideBar />
		<div class="container-fluid ">
			<Navbar />
			<RouterView />
		</div>
	</div>
</template>

<style></style>
