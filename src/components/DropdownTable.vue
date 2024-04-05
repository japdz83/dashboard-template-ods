<script setup></script>

<template>
	<div class="dropdown">
		<a
			class="btn dropdown-toggle"
			href="#"
			role="button"
			data-bs-toggle="dropdown"
			aria-expanded="false"
		>
			Acción por lote
		</a>

		<ul class="dropdown-menu">
			<li><a class="dropdown-item" href="#">Action</a></li>
			<li><a class="dropdown-item" href="#">Another action</a></li>
			<li><a class="dropdown-item" href="#">Something else here</a></li>
		</ul>
	</div>
</template>

<style scoped>
.dropdown .dropdown-toggle {
    background: var(--white);
    border: 1px solid #C3C3C3;
    border-radius: 1px;
}
.dropdown-item {
    border: none !important;
}
</style>
