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
			<router-link :to="{ name: 'Dashboard' }" class="ancla-link">
				<i class="bx bxs-dashboard"></i>
				<span class="text mx-2">Dashboard</span>
			</router-link>
			<router-link :to="{ name: 'About' }" class="ancla-link">
				<i class="bx bxs-component"></i>
				<span class="text mx-2">About</span>
			</router-link>

			<div class="ancla-link">
				<button
					type="button"
					data-bs-toggle="collapse"
					href="#collapse-reporte"
					role="button"
					aria-expanded="false"
					aria-controls="collapse-reporte"
				>
					<i class="bx bxs-data"></i>
					<span class="text mx-2">DataTablet</span>
					<i class="bx bx-chevron-down"></i>
				</button>
			</div>
			<div class="collapse" id="collapse-reporte">
				<router-link
					:to="{ name: 'Tablet'}"
					class="ancla-link link-collapse"
				>
					<i class="bx bx-table"></i>
					<span class="text mx-2">Tablet</span>
				</router-link>
				<router-link
					:to="{ name: 'Reportes'}"
					class="ancla-link link-collapse"
				>
					<i class="bx bxs-report"></i>
					<span class="text mx-2">Reportes</span>
				</router-link>
			</div>
			<div class="ancla-link">
				<button
					type="button"
					data-bs-toggle="collapse"
					href="#collapseAuth"
					role="button"
					aria-expanded="false"
					aria-controls="collapseAuth"
				>
					<i class="bx bx-user-plus"></i>
					<span class="text mx-2">Autenticación</span>
					<i class="bx bx-chevron-down"></i>
				</button>
			</div>
			<div class="collapse" id="collapseAuth">
				<router-link
					:to="{ name: 'Login' }"
					class="ancla-link link-collapse"
				>
					<i class="bx bxs-user"></i>
					<span class="text mx-2">Login</span>
				</router-link>
				<router-link
					:to="{ name: 'Registro'}"
					class="ancla-link link-collapse"
				>
					<i class="bx bx-user-plus"></i>
					<span class="text mx-2">Register</span>
				</router-link>
				<router-link
					:to="{ name: 'Recuperar_password'}"
					class="ancla-link link-collapse"
				>
					<i class="bx bx-lock-open-alt"></i>
					<span class="text mx-2">Recuperar Contraseña</span>
				</router-link>
			</div>
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
	width: calc(2rem + 40px);
	overflow: hidden;
	min-height: 100vh;
	padding: 1rem;
	box-shadow: 12px 0px 15px -5px rgba(0,0,0,0.1);
	transition: all 0.2s ease-in-out;
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
	position: relative;
	display: flex;
	justify-content: flex-end;
	margin-bottom: 1rem;
	position: relative;
	top: -3rem;
	transition: all 0.2s ease-in-out;
}
aside .menu-toggle-wrap .menu-toggle {
	position: absolute;
	display: flex;
	right: -16px;
	top: -5rem;
	z-index: 10;
	cursor: pointer;
	transition: all 0.2s ease-in-out;
	border-radius: 50%;
    border: none;
    background-color: var(--primary);
	align-items: center;
	padding: 2px;
}
aside .menu-toggle-wrap .menu-toggle .bx {
	display: flex;
	transform: rotate(0);
	align-items: center;
	margin: 0 auto;
	padding-top: 1.5px;
	font-size: 1.5rem;
	color: var(--white);
	transition: all 0.2s ease-out;
}
aside .menu-toggle-wrap .menu-toggle:hover  {
	background-color: var(--primaryHover);
}
aside h3,
aside .ancla-link .text,
aside .logo .text{
	opacity: 0;
	transition: opacity all 0.3s ease-in-out;
}

aside h3 {
	color: var(--grey);
	font-size: 0.875rem;
	margin-bottom: 0.5rem;
	text-transform: uppercase;
}
aside .menu {
	margin: 0 -1rem;
	padding: 0 1rem;
}
aside .menu .ancla-link {
	font-size: 16px;
	color: var(--grey);
	display: flex;
	align-items: center;
	text-decoration: none;
	transition: all 0.2s ease-in-out;
	padding: 0.5rem 0.7rem;
	border-radius: 5px;
	margin: 5px 0px;
}

aside .menu .link-collapse{
	margin-left: 0%;
}
aside .menu div button{
	color: var(--grey);
	display: flex;
	justify-content: space-between;
	align-items: center;
	border: none;
	background: transparent;
}
aside .menu div button a{
	margin-left: 1% !important;
}
aside .menu .ancla-linkn .bx {
	font-size: 2rem;
	color: var(--grey);
	transition: all 0.2s ease-in-out;
}
aside .menu .ancla-link .text {
	color: var(--grey);
	transition: all 0.2s ease-in-out;
}
aside .menu .ancla-link:hover {
	background-color: rgba(138, 146, 166, 0.3);
}
aside .menu .ancla-link:hover .bx, aside .menu .ancla-link:hover .text {
	color: var(--grey);
}
aside .menu .ancla-link.router-link-exact-active {
	background-color: var(--primary);
}
aside .menu .ancla-link.router-link-exact-active .bx, aside .menu .ancla-link.router-link-exact-active .text {
	color: var(--white);
}
aside .footer {
	opacity: 0;
	transition: opacity all 0.3s ease-in-out;
}
aside .footer p {
	font-size: 0.875rem;
	color: var(--grey);
}
aside.is-expanded {
	width: var(--sidebar-width);
}

aside.is-expanded .menu-toggle-wrap {
	top: 0rem;
}

aside.is-expanded .menu-toggle-wrap .menu-toggle {
	top: -3rem;
	transform: rotate(-180deg);
}
aside.is-expanded h3, aside.is-expanded .ancla-link .text,
aside.is-expanded .logo .text {
	opacity: 1;
}
aside.is-expanded .ancla-link .bx {
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
