<script setup>
import LogoURL from '../assets/img/Logo-Dashboard.png'
import BgLogin from '../assets/img/login-img.png'
import Gmail from '../assets/img/Gmail.png'
import Facebook from '../assets/img/Facebook.png'
import Instagram from '../assets/img/Instagram.png'
import Linkedin from '../assets/img/Linkedin.png'
</script>

<template>
	<div class="row">
		<div class="col col-6">
			<div class="form-login mx-auto d-flex flex-column mx-lg-0">
				<div class="card card-plain border-0 p-4 bg-white w-100">
					<div class="card-header pb-0 border-0 mb-3">
						<div
							class="login-logo text-start d-flex mb-5 align-items-center"
						>
							<img :src="LogoURL" alt="Icon-Logo" />
							<span class="h3 p-3">Logo UI</span>
						</div>
						<div class="title text-center">
							<h3 class="text-center fw-bold p-3 fs-2">
								Iniciar Sesión
							</h3>
							<p class="text-center">
								Inicia sesión para permanecer conectado.
							</p>
						</div>
					</div>

					<div class="card-body border-0 mb-3">
						<div class="form-group">
							<div class="mb-3">
								<label
									for="exampleFormControlInput1"
									class="form-label"
									>Email</label
								>
								<input
									type="email"
									class="form-control input-login"
									id="exampleFormControlInput1"
									placeholder="name@example.com"
								/>
							</div>
						</div>

						<div class="form-group">
							<div class="mb-3">
								<label
									for="exampleFormControlInput1"
									class="form-label"
									>Contraseña</label
								>
								<input
									type="password"
									class="form-control input-login"
									id="exampleFormControlInput1"
									placeholder="******"
								/>
							</div>
						</div>

						<div
							class="d-flex justify-content-between align-items-center border-0"
						>
							<div class="check form-control border-0">
								<input
									type="checkbox"
									name="recuerdame"
									id="recuerdame"
								/>
								<span class="text p-2">¿Recuerdame?</span>
							</div>
							<div class="ml-0  w-100 text-rigth">
								<a href="#">¿Olvidaste tú contraseña?</a>
							</div>
						</div>
						<div class="w-100 text-center ">
							<button
								type="submit"
								class="btn btn-form-submit mt-3"
							>
								Iniciar Sesión
							</button>
						</div>
					</div>

					<div class="card-footer border-0 mt-3 w-100">
						<div class="text-center ">
							<p>¿O iniciar sesión con otras cuentas?</p>
						</div>
						<div
							class="social-log d-flex align-items-center w-100 text-center position-relative"
						>
							<img :src="Gmail" alt="" />
							<img :src="Facebook" alt="" />
							<img :src="Instagram" alt="" />
							<img :src="Linkedin" alt="" />
						</div>
						<div class="text-center ">
							<p>
								¿No tienes una cuenta?
								<span>
									<a href="#">
										Haga clic aquí para registrarte.
									</a>
								</span>
							</p>
						</div>
					</div>
				</div>
			</div>
		</div>

		<div class="col col-6">
			<div
				class="top-0 my-auto text-center  d-lg-flex d-none h-100 pe-0 position-relative end-0 justify-content-center flex-column"
			>
				<div
					class="img-login  bg-gradient-primary h-100 d-flex flex-column justify-content-center overflow-hidden"
				></div>
			</div>
		</div>
	</div>
</template>

<style scoped>
.card-header, .card-footer{
	background-color: #fff;
}
.form-login{
	position: relative;
	left: 20%;
	width: 650px;
	padding: 2rem;
	margin: 0px auto;
}
.form-login .card .card-body input{
}
.input-login {
	border: 1px solid var(--primary) !important;
	padding: 8px 16px !important;
	border-radius: 5px !important;
	display: flex;
	align-items: center;
}

.img-login{
	width: 100%;
	height: 100vh !important;
	padding: 0px;
    background-image: url(../assets/img/login-img.png);
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
.social-log{
	position: relative;
	left: 35%;
	right: 30%;
}
</style>
