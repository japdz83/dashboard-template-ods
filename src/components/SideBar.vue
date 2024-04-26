<script setup>
import { ref } from 'vue'
import { RouterLink } from 'vue-router'

import LogoURL from '../assets/img/Logo-Dashboard.png'

const is_expanded = ref(localStorage.getItem("is_expanded") === "true")

const ToggleSidebar = () => {
	is_expanded.value = !is_expanded.value
	localStorage.setItem("is_expanded", is_expanded.value)
}
</script>

<template>
	<aside :class="`${is_expanded ? 'is-expanded' : ''}`">
		<div class="header">
			<div class="logo">
				<img :src="LogoURL" alt="Logo Empresa" />
				<span class="text mx-2 h2">Logo UI</span>
			</div>

			<i class="bx bx-left-arrow-alt toggle" @click="ToggleSidebar"></i>
		</div>

		<h3>Home</h3>
		<div class="menu">
			<router-link :to="{ name: 'Dashboard' }" class="ancla-link">
				<i class="bx bxs-dashboard bx-drop"></i>
				<span class="text mx-2">Dashboard</span>
			</router-link>
			<router-link :to="{ name: 'About' }" class="ancla-link">
				<i class="bx bxs-component bx-drop"></i>
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
					<i class="bx bxs-data bx-drop"></i>
					<span class="text mx-2">DataTablet</span>
					<i class="bx bx-chevron-down text"></i>
				</button>
			</div>
			<div class="collapse" id="collapse-reporte">
				<router-link
					:to="{ name: 'Tablet'}"
					class="ancla-link link-collapse"
				>
					<i class="bx bx-table bx-drop"></i>
					<span class="text mx-2">Tablet</span>
				</router-link>
				<router-link
					:to="{ name: 'Reportes'}"
					class="ancla-link link-collapse"
				>
					<i class="bx bxs-report bx-drop"></i>
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
					<i class="bx bx-user-plus bx-drop"></i>
					<span class="text mx-2">Autenticación</span>
					<i class="bx bx-chevron-down text"></i>
				</button>
			</div>
			<div class="collapse" id="collapseAuth">
				<router-link
					:to="{ name: 'Login' }"
					class="ancla-link link-collapse"
				>
					<i class="bx bxs-user bx-drop"></i>
					<span class="text mx-2 ">Login</span>
				</router-link>
				<router-link
					:to="{ name: 'Registro'}"
					class="ancla-link link-collapse"
				>
					<i class="bx bx-user-plus bx-drop"></i>
					<span class="text mx-2">Register</span>
				</router-link>
				<router-link
					:to="{ name: 'Recuperar_password'}"
					class="ancla-link link-collapse"
				>
					<i class="bx bx-lock-open-alt bx-drop"></i>
					<span class="text mx-2">Recuperar Contraseña</span>
				</router-link>
			</div>
		</div>
	</aside>
</template>

<style scoped></style>
