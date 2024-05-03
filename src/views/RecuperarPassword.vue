<script setup>
import LogoURL from '../assets/img/Logo-Dashboard.png'
import BgRecuperar from '../assets/img/bg-olvido-pass.jpg'
import Avatar from '../assets/img/avatar-olvido.png'
</script>

<template>
	<div class="row">
		<div class="col col-4 col-md-4 col-sm-12">
			<div class="form-login mx-auto d-flex flex-column mx-lg-0">
				<div class="card card-plain border-0 p-4 bg-white w-100">
					<div class="card-header  pb-0 border-0 mb-3">
						<div
							class="login-logo text-start d-flex mb-5 align-items-center"
						>
							<img :src="LogoURL" alt="Icon-Logo" />
							<span class="h3 p-3">Logo UI</span>
						</div>
						<div class="img-avatar w-100 text-center">
							<img :src="Avatar" alt="" />
						</div>
						<div class="title text-center">
							<h3 class="text-center fw-bold p-3 fs-2 mb-3">
								¿Olvidaste tu contraseña?
							</h3>
							<p class="text-center px-5">
								¡No te preocupes! Simplemente escribe tu correo
								electrónico y te enviaremos un código para
								restablecer tu contraseña.
							</p>
						</div>
					</div>

					<div class="card-body border-0 mb-3">
						<div class="form-group">
							<div class="mb-3">
								<label
									for="exampleFormControlInput1"
									class="form-label"
								>
									Tú Email</label
								>
								<input
									type="email"
									class="form-control input-login"
									id="exampleFormControlInput1"
									placeholder="name@example.com"
								/>
							</div>
						</div>

						<div class="w-100 text-center ">
							<button
								type="submit"
								class="btn btn-form-submit mt-3"
							>
								Recobrar Contraseña
							</button>
						</div>
					</div>
				</div>
			</div>
		</div>

		<div class="col col-8">
			<div
				class="top-0 my-auto text-center  d-lg-flex d-none h-100 position-relative end-0 justify-content-center flex-column"
			>
				<div
					class="img-login  bg-gradient-primary h-100 d-flex flex-column justify-content-center overflow-hidden"
				></div>
			</div>
		</div>
	</div>
</template>

<style scoped>
.card{
	box-shadow: 3px 5px 5px 1px rgba(0, 0, 0, 0.1);
}
.card-header, .card-footer{
	background-color: #fff;
}
.form-login{
	position: relative;
	width: 600px;
	padding: 2rem;
	margin: 50px auto;
}
.input-login {
	border: 1px solid var(--primary) !important;
	padding: 8px 16px !important;
	border-radius: 5px !important;
}

.img-login{
	width: 100%;
	height: 100vh !important;
	padding: 0px;
    background-image: url(../assets/img/bg-olvido-pass.jpg);
    background-size: cover;
}
.btn-form-submit{
	width: 50% !important;
	background-color: var(--primary);
	padding: 10px 25px;
	border-radius: 5px;
	color: var(--white);
	width: 100%;
	margin: auto;
	transition: .3s all ease;
}
.btn-form-submit:hover{
	background-color: var(--primaryHover);
}
</style>
