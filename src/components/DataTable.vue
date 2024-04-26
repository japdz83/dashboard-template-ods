<script setup>
import Dropdown from './DropdownTable.vue'
import InputSearch from './InputSearch.vue'
</script>

<template>
	<div class="card">
		<div
			class="card-header d-flex align-items-center justify-content-between"
		>
			<div
				class="d-flex align-items-center justify-content-between gap-4"
			>
				<Dropdown />
				<div
					class="text-uppercase text-secondary text-xxs font-weight-bolder opacity-7 ps-2"
				>
					<span>Desde: </span>
					<input
						class="date-tablet"
						type="date"
						id="datepicker"
						width="276"
					/>
				</div>

				<div
					class="text-uppercase text-secondary text-xxs font-weight-bolder opacity-7 ps-2"
				>
					<span>Hasta: </span>
					<input
						class="date-tablet"
						type="date"
						id="datepicker"
						width="276"
					/>
				</div>
				<InputSearch />
			</div>
			<div class="status-content">
				<div
					class="status-items d-flex justify-content-around align-items-center gap-2 "
				>
					<span class="cirle-status-green"></span>
					<span>Activo</span>
				</div>
				<div
					class="status-items d-flex d-flex justify-content-around align-items-center gap-2 "
				>
					<span class="cirle-status-red"></span>
					<span>Eliminado</span>
				</div>
			</div>
		</div>
		<div class="card-body px-0 pt-0 pb-2">
			<div class="table-responsive p-0">
				<table
					class="table align-items-center mb-0 table-striped-columns table-hover"
				>
					<thead>
						<tr>
							<th
								class="text-uppercase text-secondary text-xxs font-weight-bolder opacity-7  "
							>
								<div class="form-check">
									<input
										class="form-check-input"
										type="checkbox"
										value=""
										id="flexCheckDefault"
									/>
									<label
										class="form-check-label"
										for="flexCheckDefault"
									>
										ID
									</label>
								</div>
							</th>
							<th
								class="text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"
							>
								Nombre
							</th>
							<th
								class="text-uppercase text-secondary text-xxs font-weight-bolder opacity-7 ps-2"
							>
								Tecnología
							</th>
							<th
								class="text-uppercase text-secondary text-xxs font-weight-bolder opacity-7 ps-2"
							>
								Desde
							</th>
							<th
								class="text-uppercase text-secondary text-xxs font-weight-bolder opacity-7 ps-2"
							>
								Hasta
							</th>
							<th
								class="text-center text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"
							>
								Status
							</th>
							<th
								class="text-center text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"
							>
								Acciones
							</th>
						</tr>
					</thead>

					<tbody>
						<tr>
							<td class="align-middle">
								<div class="d-flex px-2 py-1">
									<div class="form-check">
										<input
											class="form-check-input"
											type="checkbox"
											value=""
											id="flexCheckDefault"
										/>
										<label
											class="form-check-label"
											for="flexCheckDefault"
										>
											001
										</label>
									</div>
								</div>
							</td>
							<td>
								<div
									class="d-flex flex-column justify-content-center"
								>
									<h6 class="mb-0 text-sm">John Michael</h6>
									<p class="text-xs text-secondary mb-0">
										john@creative-tim.com
									</p>
								</div>
							</td>
							<td>
								<p class="text-xs font-weight-bold mb-0">
									FrontEnd
								</p>
								<p class="text-xs text-secondary mb-0">
									HTML/CSS/Javascritp
								</p>
							</td>

							<td class="align-middle ">
								<span
									class="text-secondary text-xs font-weight-bold"
									>23/04/18</span
								>
							</td>
							<td class="align-middle ">
								<span
									class="text-secondary text-xs font-weight-bold"
									>23/04/18</span
								>
							</td>
							<td class="align-middle text-center">
								<span
									class="text-secondary text-xs font-weight-bold"
									>23/04/18</span
								>
							</td>

							<td
								class=" d-flex justify-content-center align-middle text-center gap-3"
							>
								<button
									type="button"
									class=" btn btn-tablet-ver"
								>
									<i class="bx bx-show"></i>
								</button>
								<button
									type="button"
									class=" btn btn-tablet-edit "
									data-bs-toggle="modal"
									data-bs-target="#exampleModal"
									data-bs-whatever="@mdo"
								>
									<i class="bx bx-edit-alt"></i>
								</button>
								<button
									type="button"
									class=" btn btn-tablet-delete"
								>
									<i class="bx bx-trash-alt"></i>
								</button>
							</td>
						</tr>

						<tr>
							<td class="align-middle">
								<div class="d-flex px-2 py-1">
									<div class="form-check">
										<input
											class="form-check-input"
											type="checkbox"
											value=""
											id="flexCheckDefault"
										/>
										<label
											class="form-check-label"
											for="flexCheckDefault"
										>
											003
										</label>
									</div>
								</div>
							</td>
							<td>
								<div
									class="d-flex flex-column justify-content-center"
								>
									<h6 class="mb-0 text-sm">John Michael</h6>
									<p class="text-xs text-secondary mb-0">
										john@creative-tim.com
									</p>
								</div>
							</td>
							<td>
								<p class="text-xs font-weight-bold mb-0">
									FrontEnd
								</p>
								<p class="text-xs text-secondary mb-0">
									HTML/CSS/Javascritp
								</p>
							</td>

							<td class="align-middle ">
								<span
									class="text-secondary text-xs font-weight-bold"
									>23/04/18</span
								>
							</td>
							<td class="align-middle ">
								<span
									class="text-secondary text-xs font-weight-bold"
									>23/04/18</span
								>
							</td>
							<td class="align-middle text-center">
								<span class="cirle-status-green"></span>
							</td>

							<td
								class=" d-flex justify-content-center align-middle text-center gap-3"
							>
								<button
									type="button"
									class=" btn btn-tablet-ver"
								>
									<i class="bx bx-show"></i>
								</button>
								<button
									type="button"
									class=" btn btn-tablet-edit "
									data-bs-toggle="modal"
									data-bs-target="#exampleModal"
									data-bs-whatever="@mdo"
								>
									<i class="bx bx-edit-alt"></i>
								</button>
								<button
									type="button"
									class=" btn btn-tablet-delete"
								>
									<i class="bx bx-trash-alt"></i>
								</button>
							</td>
						</tr>

						<tr>
							<td class="align-middle">
								<div class="d-flex px-2 py-1">
									<div class="form-check">
										<input
											class="form-check-input"
											type="checkbox"
											value=""
											id="flexCheckDefault"
										/>
										<label
											class="form-check-label"
											for="flexCheckDefault"
										>
											004
										</label>
									</div>
								</div>
							</td>
							<td>
								<div
									class="d-flex flex-column justify-content-center"
								>
									<h6 class="mb-0 text-sm">John Michael</h6>
									<p class="text-xs text-secondary mb-0">
										john@creative-tim.com
									</p>
								</div>
							</td>
							<td>
								<p class="text-xs font-weight-bold mb-0">
									FrontEnd
								</p>
								<p class="text-xs text-secondary mb-0">
									HTML/CSS/Javascritp
								</p>
							</td>

							<td class="align-middle ">
								<span
									class="text-secondary text-xs font-weight-bold"
									>23/04/18</span
								>
							</td>
							<td class="align-middle ">
								<span
									class="text-secondary text-xs font-weight-bold"
									>24/04/18</span
								>
							</td>
							<td class="align-middle text-center">
								<span class="cirle-status-red"></span>
							</td>

							<td
								class=" d-flex justify-content-center align-middle text-center gap-3"
							>
								<button
									type="button"
									class=" btn btn-tablet-ver"
								>
									<i class="bx bx-show"></i>
								</button>
								<button
									type="button"
									class=" btn btn-tablet-edit "
									data-bs-toggle="modal"
									data-bs-target="#exampleModal"
									data-bs-whatever="@mdo"
								>
									<i class="bx bx-edit-alt"></i>
								</button>
								<button
									type="button"
									class=" btn btn-tablet-delete"
								>
									<i class="bx bx-trash-alt"></i>
								</button>
							</td>
						</tr>

						<tr>
							<td class="align-middle">
								<div class="d-flex px-2 py-1">
									<div class="form-check">
										<input
											class="form-check-input"
											type="checkbox"
											value=""
											id="flexCheckDefault"
										/>
										<label
											class="form-check-label"
											for="flexCheckDefault"
										>
											001
										</label>
									</div>
								</div>
							</td>
							<td>
								<div
									class="d-flex flex-column justify-content-center"
								>
									<h6 class="mb-0 text-sm">John Michael</h6>
									<p class="text-xs text-secondary mb-0">
										john@creative-tim.com
									</p>
								</div>
							</td>
							<td>
								<p class="text-xs font-weight-bold mb-0">
									FrontEnd
								</p>
								<p class="text-xs text-secondary mb-0">
									HTML/CSS/Javascritp
								</p>
							</td>

							<td class="align-middle ">
								<span
									class="text-secondary text-xs font-weight-bold"
									>23/04/18</span
								>
							</td>
							<td class="align-middle ">
								<span
									class="text-secondary text-xs font-weight-bold"
									>23/04/18</span
								>
							</td>
							<td class="align-middle text-center">
								<span class="cirle-status-green"></span>
							</td>

							<td
								class=" d-flex justify-content-center align-middle text-center gap-3"
							>
								<button
									type="button"
									class=" btn btn-tablet-ver"
								>
									<i class="bx bx-show"></i>
								</button>
								<button
									type="button"
									class=" btn btn-tablet-edit "
									data-bs-toggle="modal"
									data-bs-target="#exampleModal"
									data-bs-whatever="@mdo"
								>
									<i class="bx bx-edit-alt"></i>
								</button>
								<button
									type="button"
									class=" btn btn-tablet-delete"
								>
									<i class="bx bx-trash-alt"></i>
								</button>
							</td>
						</tr>

						<tr>
							<td class="align-middle">
								<div class="d-flex px-2 py-1">
									<div class="form-check">
										<input
											class="form-check-input"
											type="checkbox"
											value=""
											id="flexCheckDefault"
										/>
										<label
											class="form-check-label"
											for="flexCheckDefault"
										>
											005
										</label>
									</div>
								</div>
							</td>
							<td>
								<div
									class="d-flex flex-column justify-content-center"
								>
									<h6 class="mb-0 text-sm">John Michael</h6>
									<p class="text-xs text-secondary mb-0">
										john@creative-tim.com
									</p>
								</div>
							</td>
							<td>
								<p class="text-xs font-weight-bold mb-0">
									FrontEnd
								</p>
								<p class="text-xs text-secondary mb-0">
									HTML/CSS/Javascritp
								</p>
							</td>

							<td class="align-middle ">
								<span
									class="text-secondary text-xs font-weight-bold"
									>23/04/18</span
								>
							</td>
							<td class="align-middle ">
								<span
									class="text-secondary text-xs font-weight-bold"
									>23/04/18</span
								>
							</td>
							<td class="align-middle text-center">
								<span class="cirle-status-red"></span>
							</td>

							<td
								class=" d-flex justify-content-center align-middle text-center gap-3"
							>
								<button
									type="button"
									class=" btn btn-tablet-ver"
								>
									<i class="bx bx-show"></i>
								</button>
								<button
									type="button"
									class=" btn btn-tablet-edit "
									data-bs-toggle="modal"
									data-bs-target="#exampleModal"
									data-bs-whatever="@mdo"
								>
									<i class="bx bx-edit-alt"></i>
								</button>
								<button
									type="button"
									class=" btn btn-tablet-delete"
								>
									<i class="bx bx-trash-alt"></i>
								</button>
							</td>
						</tr>
					</tbody>
				</table>
			</div>
		</div>
		<div class="card-footer text-body-secondary py-3">
			<div
				class="item-mostrar d-flex align-items-center justify-content-between"
			>
				<div class="d-flex align-items-center justify-content-around">
					<div
						class="mostrando d-flex align-items-center justify-content-around mx-2"
					>
						<span class="text mx-2">Mostrar</span>
						<div class="dropdown drop-pagina">
							<a
								class="btn btn-secondary dropdown-toggle"
								href="#"
								role="button"
								data-bs-toggle="dropdown"
								aria-expanded="false"
							>
								10
							</a>

							<ul class="dropdown-menu">
								<li>
									<a class="dropdown-item" href="#">1</a>
								</li>
								<li>
									<a class="dropdown-item" href="#">2</a>
								</li>
								<li>
									<a class="dropdown-item" href="#"> 3 </a>
								</li>
							</ul>
						</div>
					</div>
					<div
						class="num-registros d-flex align-items-center justify-content-around"
					>
						<span class="mx-2">Mostrando</span>
						<span class="mx-2 num-registro-item">5</span>
						<span class="mx-2">Registros</span>
					</div>
				</div>
				<div
					class="paginacion-table d-flex align-items-center justify-content-around"
				>
					<span> 1 - 10 de 500 </span>
					<span>
						<a href="#" class="prev-paginacion">
							<i class="bx bx-chevron-left "></i>
						</a>
						<a href="#" class="next-paginacion">
							<i class="bx bx-chevron-right "></i>
						</a>
					</span>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
.date-tablet{
    padding: .2rem;
    border: 1px solid #C3C3C3;
    color: var(--grey);
    margin-left: 5px;
}
.status-content{
	display: flex;
	justify-content: space-between;
	align-items: center;
	gap: 10px;
}
.status-items{
	display: flex;
	justify-content: space-between;
	align-items: center;
}
.cirle-status-green{
	background-color: rgb(79, 207, 79);
	width: 10px;
	height: 10px;
	border-radius: 50%;
}

.cirle-status-red{
	background-color: #EE3333;
	width: 10px;
	height: 10px;
	border-radius: 50%;
}
.btn-tablet-ver{
	background-color: var(--primary);
	color: var(--white);
	font-size: 20px;
	border-radius: 4px;
	transition: .3s all ease;
}

.btn-tablet-ver:hover{
	background-color: var(--primaryHover);
}
.btn-tablet-edit{
	background-color: #08B1BA;
	color: var(--white);
	font-size: 20px;
	border-radius: 4px;
	transition: .3s all ease;
}
.btn-tablet-edit:hover{
	background-color: var(--buttonColorHover);
}
.btn-tablet-delete{
	background-color: var(--btnDanger);
	color: var(--white);
	font-size: 20px;
	border-radius: 4px;
	transition: .3s all ease;
}
.btn-tablet-delete:hover{
	background-color: var(--btnDangerHover);
}

.form-check{
	display: flex;
	gap: 5px
}
.mostrando .text{
	font-weight: 600;
}
.drop-pagina .dropdown-toggle{
	width: 70px;
	height: 40px;
	border: 1px solid #7A8789;
	border-radius: 35px !important;
	background-color: #fff;
	color: #7A8789;
}
.num-registro-item{
	display: flex;
	align-items: center;
	justify-content: center;
	width: 50px;
	height: 40px;
	border: 1px solid #7A8789;
	border-radius: 5px;
}
.prev-paginacion,
.next-paginacion{
	color: var(--grey);
	font-size: 25px;
}
</style>
