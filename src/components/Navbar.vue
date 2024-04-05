<script setup>
import flag from '../assets/flag-Ing.png'
import avatar from '../assets/avatar-1.png'
</script>

<template>
	<header class="p-3 border-bottom-1 z-1 shadow  ">
		<div class="container-fluid ">
			<div
				class="d-flex flex-wrap align-items-center justify-content-start content-nav"
			>
				<form
					class="col-4 col-lg-auto mb-3 mb-lg-0 me-lg-3 "
					role="search"
				>
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

				<div
					class="nav col-12 col-lg-auto me-lg-auto mb-2 justify-content-center mb-md-0"
				></div>

				<div class="d-flex text-end user-access">
					<ul
						class="nav col-12 col-lg-auto me-lg-auto mb-2 mb-md-0 align-middle "
					>
						<li>
							<a
								href="#"
								class="nav-link px-2 link-body-emphasis"
							>
								<img :src="flag" alt="Item-Lenguaje" />
							</a>
						</li>
						<li>
							<a
								href="#"
								class="nav-link px-2 link-body-emphasis"
							>
								<i class="bx bxs-bell"></i>
							</a>
						</li>
						<li>
							<a
								href="#"
								class="nav-link px-2 link-body-emphasis"
							>
								<i class="bx bxs-envelope"></i>
							</a>
						</li>
					</ul>

					<div class="dropdown">
						<a
							href="#"
							class="d-block link-body-emphasis text-decoration-none dropdown-toggle"
							data-bs-toggle="dropdown"
							aria-expanded="false"
						>
							<img
								:src="avatar"
								alt="mdo"
								width="32"
								height="32"
								class="rounded-circle"
							/>
						</a>

						<ul class="dropdown-menu text-small">
							<li>
								<a class="dropdown-item" href="#"
									>New project...</a
								>
							</li>
							<li>
								<a class="dropdown-item" href="#">Settings</a>
							</li>
							<li>
								<a class="dropdown-item" href="#">Profile</a>
							</li>
							<li><hr class="dropdown-divider" /></li>
							<li>
								<a class="dropdown-item" href="#">Sign out</a>
							</li>
						</ul>
					</div>
				</div>
			</div>
		</div>
	</header>
</template>

<style scoped>
.content-nav{
	display: grid;
	gap: 10px;
	grid-template-rows: 1fr;
	grid-template-columns: 2, 1fr ;
}
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

.user-access{
	display: flex;
	align-items: center;
	justify-content: end;
	justify-content: space-between;
}

.user-access ul li a{
	font-size: 1.5rem;
	color: var(--grey) !important;
}
</style>
