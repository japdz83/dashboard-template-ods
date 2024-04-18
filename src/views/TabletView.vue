<script setup>
import Tablet from '../components/DataTable.vue'
import ModalForm from '../components/ModalForm.vue'
import Impresora from '../assets/btn-reportes/impresora-1.png'
import Excel from '../assets/btn-reportes/excel-1.png'
import PDF from '../assets/btn-reportes/pdf-1.png'
</script>

<template>
	<div class="container-fluid p-4">
		<div class="row">
			<div
				class="d-flex justify-content-between align-items-center w-100 "
			>
				<div class="box_reporte d-flex gap-2 ">
					<button class="buton_reporte">
						<img :src="Impresora" alt="" />
					</button>
					<button class="buton_reporte">
						<img :src="Excel" alt="" />
					</button>
					<button class="buton_reporte">
						<img :src="PDF" alt="" />
					</button>
				</div>
				<div class="box_btn-crear">
					<button
						class="px-4 py-2 d-flex align-items-center gap-3"
						data-bs-toggle="modal"
						data-bs-target="#exampleModal"
						data-bs-whatever="@mdo"
					>
						<i class="bx bx-plus"></i>
						<span>Crear</span>
					</button>
				</div>
			</div>
		</div>

		<div class="tablet-content mt-5 row">
			<div class="col-12">
				<Tablet />
			</div>
		</div>
	</div>

	<ModalForm />
</template>

<style scoped>
.buton_reporte{
	width: 60px;
	height: 60px;
	padding: 1px;
	border: 2px solid #3a57e8 !important;
	border-radius: 50%;
	transition: .3s all ease;
}
.buton_reporte:hover{
	background-color: #e6e6e6 !important;
}
.box_reporte button{
    border: none;
    background-color: transparent;
}
.box_btn-crear button i{
    font-size: 20px;
}

.box_btn-crear button{
    border: none;
    border-radius: 5px;
    background-color: var(--primary);
    color: var(--white);
    font-weight: 700;
	transition: .3s ease all;
}
.box_btn-crear button:hover{
    background-color: var(--primaryHover);

}
</style>
