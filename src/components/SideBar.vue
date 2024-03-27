<script setup>
import { ref } from 'vue'
import { RouterLink } from 'vue-router'

import LogoURL from '../assets/Logo-Dashboard.png'

const is_expanded = ref(localStorage.getItem("is_expanded") === "true")

const ToggleMenu = () => {
	is_expanded.value = !is_expanded.value
	localStorage.setItem("is_expanded", is_expanded.value)
}
</script>

<template>
	<aside :class="`${is_expanded ? 'is-expanded' : ''}`">
		<div class="logo">
			<img :src="LogoURL" alt="Logo Empresa" />
			<span class="text mx-2 h2">Logo UI</span>
		</div>

		<div class="menu-toggle-wrap">
			<button class="menu-toggle" @click="ToggleMenu">
				<i class="bx bx-right-arrow-alt"></i>
			</button>
		</div>

		<h3>Home</h3>
		<div class="menu">
			<router-link to="/" class="button">
				<i class="bx bxs-dashboard"></i>
				<span class="text mx-2">Dashboard</span>
			</router-link>
			<router-link to="/about" class="button">
				<i class="bx bxs-component"></i>
				<span class="text mx-2">About</span>
			</router-link>
			<router-link to="/team" class="button">
				<i class="bx bx-table"></i>
				<span class="text mx-2">Tablet</span>
			</router-link>
			<router-link to="/login" class="button">
				<i class="bx bxs-user"></i>
				<span class="text mx-2">Login</span>
			</router-link>
			<router-link to="/contact" class="button">
				<i class="bx bx-user-plus"></i>
				<span class="text mx-2">Register</span>
			</router-link>
		</div>
	</aside>
</template>

<style scoped>


aside {
	display: flex;
	position: relative;
	flex-direction: column;
	background-color: var(--white);
	color: var(--grey);
	width: calc(2rem + 45px);
	overflow: hidden;
	min-height: 100vh;
	padding: 1rem;
	box-shadow: 12px 0px 15px -5px rgba(0,0,0,0.1);
	transition: 0.2s ease-in-out;
}
aside .flex {
	flex: 1 1 0%;
}
 aside .logo {
	 margin-bottom: 1rem;
	 align-items: center;
}
 aside .logo img {
	 width: 2rem;
}
 aside .logo span {
	padding: 0rem 2rem;
	padding-bottom: 2rem;
	color: var(--primary-alt);
}
 aside .menu-toggle-wrap {
	 display: flex;
	 justify-content: flex-end;
	 margin-bottom: 1rem;
	 position: relative;
	 top: 0;
	 transition: 0.2s ease-in-out;
}
 aside .menu-toggle-wrap .menu-toggle {
	display: flex;
	transition: 0.2s ease-in-out;
	border-radius: 50%;
    border: none;
    background-color: var(--primary);
	align-items: center;
	padding: 3px;
}
aside .menu-toggle-wrap .menu-toggle .bx {
	align-items: center;
	margin: 0 auto;
	padding-top: 1.5px;
	font-size: 2rem;
	color: var(--white);
	transition: 0.2s ease-out;
}
aside .menu-toggle-wrap .menu-toggle:hover .bx {
	transform: translateX(0.5rem);
}
aside h3,
aside .button .text,
aside .logo .text{
	opacity: 0;
	transition: opacity 0.3s ease-in-out;
}

aside h3 {
	color: var(--grey);
	font-size: 0.875rem;
	margin-bottom: 0.5rem;
	text-transform: uppercase;
}
aside .menu {
	margin: 0 -2rem;
	padding: 0 1.5rem;
}
aside .menu .button {
	display: flex;
	align-items: center;
	text-decoration: none;
	transition: 0.2s ease-in-out;
	padding: 0.5rem 1rem;
	border-radius: 5px;
	margin: 3px 0px;
}
aside .menu .button .bx {
	font-size: 2rem;
	color: var(--grey);
	transition: 0.2s ease-in-out;
}
aside .menu .button .text {
	color: var(--grey);
	transition: 0.2s ease-in-out;
}
aside .menu .button:hover {
	background-color: rgba(138, 146, 166, 0.3);
}
aside .menu .button:hover .bx, aside .menu .button:hover .text {
	color: var(--grey);
}
aside .menu .button.router-link-exact-active {
	background-color: var(--primary);
}
aside .menu .button.router-link-exact-active .bx, aside .menu .button.router-link-exact-active .text {
	color: var(--white);
}
aside .footer {
	opacity: 0;
	transition: opacity 0.3s ease-in-out;
}
aside .footer p {
	font-size: 0.875rem;
	color: var(--grey);
}
aside.is-expanded {
	width: var(--sidebar-width);
}
aside.is-expanded .menu-toggle-wrap {
	top: -3rem;
}
aside.is-expanded .menu-toggle-wrap .menu-toggle {
	transform: rotate(-180deg);
}
aside.is-expanded h3, aside.is-expanded .button .text,
aside.is-expanded .logo .text {
	opacity: 1;
}
aside.is-expanded .button .bx {
	margin-right: 1rem;
}
aside.is-expanded .footer {
	opacity: 0;
}
@media (max-width: 1024px) {
	aside {
		position: absolute;
		z-index: 99;
	}
}
</style>
