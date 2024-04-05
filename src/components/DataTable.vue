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
}
.btn-tablet-edit{
	background-color: #08B1BA;
	color: var(--white);
	font-size: 20px;
	border-radius: 4px;

}
.btn-tablet-delete{
	background-color: #EE3333;
	color: var(--white);
	font-size: 20px;
	border-radius: 4px;
}
.form-check{
	display: flex;
	gap: 5px
}
</style>
