<script setup>
import flag from '../assets/img/Flag/flag-Ing.png'
import avatar from '../assets/img/avatar-1.png'
</script>

<template>
	<header class="px-2 border-bottom-1 shadow">
		<nav class="navbar navbar-expand-lg navbar-light bg-light">
			<div class="container-fluid">
				<div class="d-flex align-items-center">
					<form class="d-flex ms-auto form-nav">
						<i class="bx bx-search"></i>
						<input
							class="form-control me-2 search-nav"
							type="search"
							placeholder="Buscar"
							aria-label="Search"
						/>
					</form>
				</div>

				<button
					class="navbar-toggler"
					type="button"
					data-bs-toggle="collapse"
					data-bs-target="#navbarNavDropdown"
					aria-controls="navbarNavDropdown"
					aria-expanded="false"
					aria-label="Toggle navigation"
				>
					<span class="navbar-toggler-icon"></span>
				</button>

				<div class="collapse navbar-collapse" id="navbarNavDropdown">
					<ul class="navbar-nav ms-auto">
						<li class="nav-item">
							<router-link to="/" class="nav-link">
								<img :src="flag" alt="Item-Lenguaje" />
							</router-link>
						</li>
						<li class="nav-item">
							<router-link to="/usuarios" class="nav-link">
								<i class="bx bxs-bell bx-nav"></i>
							</router-link>
						</li>
						<li class="nav-item">
							<router-link to="/productos" class="nav-link">
								<i class="bx bxs-envelope bx-nav"></i>
							</router-link>
						</li>
					</ul>

					<div class="dropdown">
						<button
							class="dropdown-toggle d-flex text-lg-start align-items-center justify-content-around "
							type="button"
							id="dropdownMenuButton1"
							data-bs-toggle="dropdown"
							aria-expanded="false"
						>
							<img
								:src="avatar"
								alt="mdo"
								width="40"
								height="40"
								class="rounded-circle"
							/>
							<span class="px-3">
								<h6>Austin Robertso</h6>
								<p>Marketing Administrator</p>
							</span>
						</button>
						<ul
							class="dropdown-menu"
							aria-labelledby="dropdownMenuButton1"
						>
							<li>
								<a class="dropdown-item" href="#">Perfil</a>
							</li>
							<li>
								<a class="dropdown-item" href="#"
									>Configuración</a
								>
							</li>
							<li>
								<a class="dropdown-item" href="#"
									>Cerrar sesión</a
								>
							</li>
						</ul>
					</div>
				</div>
			</div>
		</nav>
	</header>
</template>
