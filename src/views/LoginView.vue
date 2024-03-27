<script setup>
import LogoURL from '../assets/Logo-Dashboard.png'
</script>

<template>
	<div class="col-12 mt-0 content ">
		<div class="row">
			<div
				class="form-login mx-auto col-xl-4 col-lg-5 col-md-7 d-flex flex-column mx-lg-0"
			>
				<div class="card card-plain border-0">
					<div class="card-header text-start pb-0 border-0">
						<div class="login-logo">
							<img :src="LogoURL" alt="Icon-Logo" />
							<span class="h3">Logo UI</span>
						</div>
					</div>

					<div class="card-body border-0"></div>

					<div
						class="d-flex justify-content-between align-items-center card-footer border-0"
					>
						<div class="check form-control border-0">
							<input
								type="checkbox"
								name="recuerdame"
								id="recuerdame"
							/>
							<span class="text p-2">¿Recuerdame?</span>
						</div>
						<div class="ml-5 w-100 text-rigth">
							<a href="#">¿Olvidaste tú contraseña?</a>
						</div>
					</div>
				</div>
			</div>

			<div
				class="top-0 my-auto text-center col-6 d-lg-flex d-none h-100 pe-0 position-absolute end-0 justify-content-center flex-column"
			>
				<div
					class="img-login position-relative bg-gradient-primary h-100 m-3 p-0  d-flex flex-column justify-content-center overflow-hidden"
				></div>
			</div>
		</div>
	</div>
</template>

<style scoped>
.img-login{
    background-image: url(../assets/login-img.png);
    background-size: cover;
    margin: 0 !important;
}
</style>
