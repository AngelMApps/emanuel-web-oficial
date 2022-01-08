<script>
	import CompParallax from '../../components/parallax_comp.svelte';
	import Footer from '../../components/footer.svelte';
	import Navbar from '../../components/Navbar.svelte';
</script>

<svelte:head>
	<title>Devocional</title>
</svelte:head>

<Navbar />
<main>
	<div class="container-text">
		<h1>Devocional</h1>
		<hr />
		<div>
			<p class="parraf-cont">
				" Dios mío, ¡tú eres mi Dios! Yo te buscaré de madrugada.<br />
				Mi alma desfallece de sed por ti; mi ser entero te busca<br />
				con ansias ... " (Salmos 63:1)
			</p>
		</div>
	</div>
	<CompParallax iURL="../images/cDevo.png" sHeight="47" />
	<div class="div-info">
		<h3>¿Qué es el tiempo de Devocional?</h3>
		<p class="parraf2-cont">
			Es el tiempo que le entregamos a <strong>Dios</strong> para que él nos llene de fuerzas y
			<br />
			así poder caminar firmes en cada situación que pueda ocurrirnos en el día.<br />
		</p>
	</div>
	<CompParallax iURL="../images/fondo6.png" bright="0.1" />

	<div class="div-info">
		<p class="parraf3-cont">
			Te invitamos a nuestras reuniones de <strong>DEVOCIONAL</strong><br />
			transmitidas a través de Facebook en vivo de lunes a domingo.
		</p>
		<h5>desde las 6:00am hasta las 7:00am</h5>
	</div>
	<CompParallax iURL="../images/cDevo.png" />
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
		white-space: nowrap;
		border-right: 4px solid;
		width: 8ch;
		margin: 0;
		color: #fff;
		font-size: 90pt;
		text-align: center;
		font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		animation: typing 1s steps(8), blink 0.5s infinite step-end alternate;
		overflow: hidden;
	}
	@keyframes typing {
		from {
			width: 0;
		}
	}
	@keyframes blink {
		50% {
			border-color: transparent;
		}
	}
	p {
		color: #fff;
		margin-top: 1rem;
		font-size: 20pt;
		text-align: center;
		line-height: 2rem;
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
	}
	@media only screen and (max-width: 610px) {
		h1 {
			margin: 0;
			color: #fff;
			font-size: 75pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}

		.parraf-cont {
			font-size: 15pt;
			line-height: 1.3rem;
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
	}
	@media only screen and (max-width: 540px) {
		h1 {
			margin: 0;
			color: #fff;
			font-size: 70pt;
			text-align: center;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		.parraf-cont {
			font-size: 13pt;
			line-height: 1.3rem;
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
			font-size: 12pt;
			line-height: 1.3rem;
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
			font-size: 10pt;
			line-height: 1.3rem;
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
			font-size: 18pt;
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
			font-size: 9pt;
			line-height: 1.3rem;
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
			font-size: 16pt;
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
			font-size: 9pt;
			line-height: 1.3rem;
		}
		.parraf3-cont {
			font-size: 14pt;
		}
		h5 {
			margin-top: 1rem;
			text-align: center;
			font-size: 20px;
			color: #a3b9f9;
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
			font-size: 9pt;
			line-height: 1.3rem;
		}
		.parraf3-cont {
			font-size: 14pt;
		}
		h5 {
			margin-top: 1rem;
			text-align: center;
			font-size: 17px;
			color: #a3b9f9;
		}
	}
</style>
