<script>
	import CompParallax from '../../components/parallax_comp.svelte';
	import Footer from '../../components/footer.svelte';
	import Navbar from '../../components/Navbar.svelte';
</script>

<svelte:head>
	<title>Dominical</title>
</svelte:head>

<Navbar />
<main>
	<div class="container-text ">
		<h1 class="animate__animated animate__bounceInDown ">Culto Dominical</h1>
		<hr />
		<div>
			<p class="parraf-cont animate__animated animate__fadeIn animate__slow">
				"Entrad por sus puertas con acción de gracias, por sus atrios con alabanza; Alabadle,
				bendecid su nombre. Porque Jehová es bueno; para siempre es su misericordia, Y su verdad por
				todas las generaciones" (Salmos 100:4-5)
			</p>
		</div>
	</div>
	<CompParallax iURL="../images/domingo1.jpg" sHeight="55" bright="0.1" />
	<div class="div-info">
		<h3>Culto Dominical</h3>
		<p class="parraf2-cont">
			Nos reunimos para agradecer toda la ayuda, protección y amor que <strong>Dios</strong>,
			nuestro padre, nos mostró en el transcurso de la semana y por que nos permitió tener un nuevo
			día de vida.
		</p>
	</div>
	<CompParallax iURL="../images/domingo2.jpg" sHeight="47" bright="0.1" />

	<div class="div-info">
		<p class="parraf3-cont">
			Te invitamos a nuestras reuniones <strong>DOMINICALES</strong> de agradecimiento en nuestra iglesia,
			también puedes participar en las transmisiones a través de Facebook en vivo todos los domingos.
		</p>
		<h5>desde las 10:00am hasta las 12:00pm</h5>
	</div>
	<CompParallax iURL="../images/domingo3.jpg" sHeight="47" bright="0.1" />
	<Footer />
</main>

<style>
	main {
		position: absolute;
		top: 0;
		width: 100%;
		padding: 0;
		margin: 0;
		z-index: 0;
	}

	.container-text {
		position: absolute;
		display: flex;
		flex-direction: column;
		align-items: center;
		top: 250px;
		left: 0;
		right: 0;
		z-index: 1;
	}
	.div-info {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		left: 15%;
		right: 15%;
		position: absolute;
		z-index: 1;
		height: 20rem;
		border-radius: 35px;
		padding: 2.5rem;
		margin-top: 10rem;
		background-color: rgba(129, 188, 218, 0.1);
		box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
	}
	hr {
		margin-top: 1rem;
		background-color: #fff;
		border: none;
		width: 10rem;
		height: 0.2rem;
	}
	h1 {
		margin: 0;
		color: #fff;
		font-size: 90pt;
		text-align: center;
		font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
	}
	p {
		color: #fff;
		margin-top: 1rem;
		font-size: 20pt;
		text-align: center;
		line-height: 2rem;
	}
	.parraf-cont {
		padding: 0px 80px;
	}
	h3 {
		margin: 0;
		color: #fff;
		font-size: 30pt;
		text-align: center;
		font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
	}
	h5 {
		margin-top: 1rem;
		text-align: center;
		font-size: 25px;
		color: #a3b9f9;
	}
	@media only screen and (max-width: 783px) {
		h3 {
			margin: 0;
			color: #fff;
			font-size: 30pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf2-cont {
			font-size: 17pt;
		}
	}
	@media only screen and (max-width: 750px) {
		.parraf-cont {
			font-size: 18pt;
		}
	}
	@media only screen and (max-width: 711px) {
		h1 {
			margin: 0;
			color: #fff;
			font-size: 80pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf-cont {
			font-size: 17pt;
		}
		.parraf3-cont {
			font-size: 19pt;
		}
		h5 {
			margin-top: 0;
		}
	}
	@media only screen and (max-width: 685px) {
		h3 {
			margin: 0;
			color: #fff;
			font-size: 30pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf2-cont {
			font-size: 14pt;
		}
		.parraf3-cont {
			font-size: 19pt;
		}
		h5 {
			font-size: 22px;
		}
	}
	@media only screen and (max-width: 612px) {
		h1 {
			margin: 0;
			color: #fff;
			font-size: 75pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}

		.parraf-cont {
			line-height: 2rem;
		}
		h3 {
			margin: 0;
			color: #fff;
			font-size: 25pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf2-cont {
			font-size: 12pt;
		}
		.parraf3-cont {
			font-size: 17pt;
		}
		h5 {
			font-size: 22px;
		}
	}
	@media only screen and (max-width: 547px) {
		.div-info {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			left: 15%;
			right: 15%;
			position: absolute;
			z-index: 1;
			height: 20rem;
			border-radius: 35px;
			padding: 2.5rem 1rem 2.5rem 1rem;
			margin-top: 10rem;
			background-color: rgba(129, 188, 218, 0.1);
			box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
		}
		h1 {
			margin: 0;
			color: #fff;
			font-size: 70pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf-cont {
			font-size: 15pt;
			line-height: 2rem;
		}
		h3 {
			margin: 0;
			color: #fff;
			font-size: 25pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf2-cont {
			font-size: 11pt;
		}
		.parraf3-cont {
			font-size: 16pt;
		}
		h5 {
			font-size: 18px;
		}
	}
	@media only screen and (max-width: 495px) {
		.div-info {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			left: 15%;
			right: 15%;
			position: absolute;
			z-index: 1;
			height: 20rem;
			border-radius: 35px;
			padding: 2.5rem 1rem 2.5rem 1rem;
			margin-top: 10rem;
			background-color: rgba(129, 188, 218, 0.1);
			box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
		}
		h3 {
			margin: 0;
			color: #fff;
			font-size: 25pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf2-cont {
			font-size: 11pt;
		}
	}
	@media only screen and (max-width: 475px) {
		.div-info {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			left: 15%;
			right: 15%;
			position: absolute;
			z-index: 1;
			height: 20rem;
			border-radius: 35px;
			padding: 2.5rem 1rem 2.5rem 1rem;
			margin-top: 10rem;
			background-color: rgba(129, 188, 218, 0.1);
			box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
		}
		h1 {
			margin: 0;
			color: #fff;
			font-size: 65pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf-cont {
			font-size: 14pt;
			line-height: 2rem;
		}
	}
	@media only screen and (max-width: 451px) {
		.parraf3-cont {
			font-size: 14pt;
		}
		h5 {
			font-size: 18px;
		}
	}
	@media only screen and (max-width: 440px) {
		h1 {
			margin: 0;
			color: #fff;
			font-size: 56pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf-cont {
			font-size: 13pt;
			line-height: 2rem;
		}
	}
	@media only screen and (max-width: 420px) {
		.div-info {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			left: 10%;
			right: 10%;
			position: absolute;
			z-index: 1;
			height: 20rem;
			border-radius: 35px;
			padding: 2.5rem 1rem 2.5rem 1rem;
			margin-top: 10rem;
			background-color: rgba(129, 188, 218, 0.1);
			box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
		}
		h3 {
			margin: 0;
			color: #fff;
			font-size: 20pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf2-cont {
			font-size: 10pt;
		}
	}
	@media only screen and (max-width: 394px) {
		.parraf3-cont {
			font-size: 13pt;
		}
		h5 {
			font-size: 18px;
		}
	}
	@media only screen and (max-width: 388px) {
		h3 {
			margin: 0;
			color: #fff;
			font-size: 20pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf2-cont {
			font-size: 9pt;
		}
	}
	@media only screen and (max-width: 370px) {
		h1 {
			margin: 0;
			color: #fff;
			font-size: 50pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf-cont {
			line-height: 2rem;
		}
	}
	@media only screen and (max-width: 358px) {
		.div-info {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			left: 5%;
			right: 5%;
			position: absolute;
			z-index: 1;
			height: 20rem;
			border-radius: 35px;
			padding: 2.5rem 1rem 2.5rem 1rem;
			margin-top: 10rem;
			background-color: rgba(129, 188, 218, 0.1);
			box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
		}
		h3 {
			margin: 0;
			color: #fff;
			font-size: 18pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf2-cont {
			font-size: 9pt;
		}
		.parraf3-cont {
			font-size: 13pt;
		}

		h5 {
			font-size: 18px;
		}
	}
	@media only screen and (max-width: 330px) {
		h1 {
			margin: 0;
			color: #fff;
			font-size: 40pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf-cont {
			font-size: 11pt;
			padding: 0px 15px;
			line-height: 2rem;
		}
		.parraf3-cont {
			font-size: 12pt;
		}
		h5 {
			font-size: 18px;
		}
	}
	@media only screen and (max-width: 290px) {
		h1 {
			margin: 0;
			color: #fff;
			font-size: 40pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf-cont {
			font-size: 10pt;
			padding: 0px 17px;
			line-height: 2rem;
		}
		.parraf3-cont {
			font-size: 12pt;
		}
		h5 {
			font-size: 17px;
		}
	}
</style>
