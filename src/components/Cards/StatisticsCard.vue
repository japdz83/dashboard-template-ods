<script setup>
// import porcentaje from '../../assets/porcentaje.png'
import CircleProgress from 'vue3-circle-progress'
import "vue3-circle-progress/dist/circle-progress.css"
</script>

<template>
	<div class="mb-3 card border-0 rounded-2 p-2 mx-0">
		<div class="p-3 card-body">
			<div class="d-flex justify-content-between">
				<div class="text-center icon icon-shape">
					<CircleProgress
						:percent="porcentaje"
						:size="100"
						:border-width="6"
						:border-bg-width="6"
						fill-color="#3a57e8"
						empty-color="#e1e1e1"
					/>
				</div>

				<div class="text-center icon icon-shape">
					<p class="h6 text-dark mb-3 py-2">Ventas Totales</p>
					<p class="h3 valor-venta">$ 560K</p>
				</div>
			</div>
		</div>
	</div>
</template>
