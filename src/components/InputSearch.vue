<script setup></script>

<template>
	<form class="col-4 col-lg-auto mb-3 mb-lg-0 me-lg-3 " role="search">
		<div
			class="form-control form-nav d-flex align-items-center justify-content-between "
		>
			<i class="bx bx-search"></i>
			<input
				type="search"
				class="search-nav"
				placeholder="Buscar..."
				aria-label="Search"
			/>
		</div>
	</form>
</template>

<style scoped>
.form-nav {
	display: flex;
	position: relative;
	align-items: center;
}

.form-nav .bx{
	font-size: 1.5rem;
	color: var(--grey);
	margin-right: 0.5rem;
}
.search-nav{
	border: none;
	padding: 4px;
}
.search-nav:focus{
	border: 1px solid var(--primary);
}
</style>
