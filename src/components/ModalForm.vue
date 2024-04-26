<script setup></script>

<template>
	<div
		class="modal fade"
		id="exampleModal"
		tabindex="-1"
		aria-labelledby="exampleModalLabel"
		aria-hidden="true"
	>
		<div class="modal-dialog modal-lg">
			<div class="modal-content">
				<div class="modal-header">
					<h1 class="modal-title fs-5" id="exampleModalLabel">
						Crear Producto
					</h1>
					<button
						type="button"
						class="btn-close"
						data-bs-dismiss="modal"
						aria-label="Close"
					></button>
				</div>
				<div class="modal-body">
					<form>
						<div class="row">
							<div class="col col-6 ">
								<div class="mb-3">
									<label
										for="recipient-name"
										class="col-form-label"
										>Nombre Producto</label
									>
									<input
										type="text"
										class="form-control"
										id="recipient-name"
										placeholder="Tamplate"
									/>
								</div>
							</div>

							<div class="col col-6">
								<div class="mb-3">
									<label
										for="recipient-name"
										class="col-form-label"
										>Categoría</label
									>
									<input
										type="text"
										class="form-control"
										id="recipient-name"
										placeholder="Tecnología"
									/>
								</div>
							</div>
						</div>
						<div class="row">
							<div class="col col-6 ">
								<div class="mb-3">
									<label
										for="recipient-name"
										class="col-form-label"
										>Estilo</label
									>
									<input
										type="text"
										class="form-control"
										id="recipient-name"
										placeholder="Buscar"
									/>
								</div>
							</div>

							<div class="col col-6">
								<div class="mb-3">
									<label
										for="recipient-name"
										class="col-form-label"
										>Precio</label
									>
									<input
										type="text"
										class="form-control"
										id="recipient-name"
										placeholder="$ 150"
									/>
								</div>
							</div>
						</div>

						<div class="mb-3">
							<label for="message-text" class="col-form-label"
								>Detalle</label
							>
							<textarea
								class="form-control"
								id="message-text"
								placeholder="Detalle"
							></textarea>
						</div>
					</form>
				</div>
				<div class="modal-footer">
					<button
						type="button"
						class="btn btn-secondary"
						data-bs-dismiss="modal"
					>
						Cerrar
					</button>
					<button type="button" class="btn btn-form">Crear</button>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
.modal-title{
    color: var(--primary);
    padding: 5px 0px;
    font-weight: 700;
}
.modal-footer button{
    padding: 5px 3rem;
    border-radius: 4px;
}
.form-control{
	border: 1px solid var(--grey) !important;
	padding: 6px !important;
}
.btn-form{
    background-color: var(--buttonColor);
    color: var(--white);
    transition: .3s ease all;
}
.btn-form:hover{
    background-color: var(--buttonColorHover);
    color: var(--white);
}
</style>
