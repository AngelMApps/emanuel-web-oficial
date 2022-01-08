<script>
	// your script goes here
	import CompParallax from '../../components/parallax_comp.svelte';
	import Footer from '../../components/footer.svelte';
	import Navbar from '../../components/Navbar.svelte';
</script>

<!-- markup (zero or more items) goes here -->
<svelte:head>
	<title>Niños</title>
</svelte:head>
<Navbar />
<main>
	<div class="container-text">
		<h1 class="animate__animated animate__bounceInDown">CULTO DE NIÑOS</h1>
		<hr />
		<div>
			<p class="parraf-cont animate__animated animate__backInLeft">
				«Pero Jesús dijo: Dejad que los niños vengan a mi, y no se lo impidáis; porque de los tales
				es el reino de los cielos» Mateo 19:14.
			</p>
		</div>
	</div>
	<CompParallax iURL="../images/kids1.jpg" sHeight="50" sPadding="10" bright="0.3" />

	<div class="div-info">
		<img class="img1 animate__animated animate__fadeInLeft" alt="logo" src="../images/kids3.png" />
		<p class="parraf2-cont animate__animated animate__backInLeft">
			Instruimos con amor, enseñanzas y canciones a los niños en los caminos del señor, logrando que
			cada uno de ellos conozca a través de historias los milagros de Jesús.
		</p>
	</div>
	<CompParallax iURL="../images/kids3.jpg" sHeight="47" sPadding="10" bright="0.2" />
	<div class="div-info" style="background-color: rgba(136, 184, 255, 0.753);">
		<img class="img2 animate__animated animate__fadeInLeft" alt="logo" src="../images/kids4.png" />

		<p class="parraf3-cont animate__animated animate__backInLeft">
			Nuestras reuniones son los domingos desde las 10:30 am hasta las 12:00 pm
		</p>
	</div>
	<CompParallax iURL="../images/kids4.jpg" sHeight="47" sPadding="10" bright="0.2" />
	<Footer />
</main>

<style>
	/* your styles go here */
	@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@600&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Grandstander:ital,wght@1,300&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Chicle&display=swap');
	main {
		position: absolute;
		top: 0;
		width: 100%;
		padding: 0;
		margin: 0;
		z-index: 0;
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
	p {
		color: #fff;
		margin-top: 1rem;
		padding: 0px 40px;
		font-size: 20pt;
		text-align: center;
		font-family: 'Grandstander', cursive;
		line-height: 2rem;
	}
	.div-info {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: center;
		left: 15%;
		right: 15%;
		position: absolute;
		z-index: 1;
		height: 25rem;
		border-radius: 35px;
		padding: 2.5rem;
		margin-top: 10rem;
		background-color: rgba(136, 255, 245, 0.753);
		box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
	}
	img {
		height: 20rem;
		margin-right: 10px;
	}
	.parraf2-cont {
		font-size: 35px;
		color: #fff;
		line-height: 2.5rem;
	}
	.parraf3-cont {
		font-size: 40px;
		color: #fff;
		line-height: 3rem;
	}

	@media only screen and (max-width: 1050px) {
		.parraf2-cont {
			font-size: 25pt;
			color: #fff;
			line-height: 2.5rem;
		}
		.parraf3-cont {
			font-size: 30pt;
			color: #fff;
			line-height: 3rem;
		}
	}
	@media only screen and (max-width: 940px) {
		.parraf2-cont {
			font-size: 26px;
			color: #fff;
			line-height: 2.5rem;
		}
		.parraf3-cont {
			font-size: 26px;
			color: #fff;
			line-height: 3rem;
		}
		.img1 {
			height: 17rem;
		}
		.img2 {
			height: 17rem;
		}
	}
	@media only screen and (max-width: 810px) {
		.parraf2-cont {
			font-size: 26pt;
			color: #fff;
			line-height: 2.5rem;
		}
		.parraf3-cont {
			font-size: 26pt;
			color: #fff;
			line-height: 3rem;
		}
		.img1 {
			display: none;
		}
		.img2 {
			display: none;
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
			padding: 10px;
		}
	}
	@media only screen and (max-width: 685px) {
		.parraf2-cont {
			font-size: 22pt;
		}
		.parraf3-cont {
			font-size: 22pt;
			color: #fff;
			line-height: 3rem;
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
			padding: 10px;
		}

		.parraf2-cont {
			font-size: 20pt;
		}
		.parraf3-cont {
			font-size: 20pt;
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
			padding: 10px;
		}

		.parraf2-cont {
			font-size: 18pt;
		}
		.parraf3-cont {
			font-size: 18pt;
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
			background-color: rgba(136, 255, 245, 0.753);
			box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
		}

		.parraf2-cont {
			font-size: 16pt;
		}
		.parraf3-cont {
			font-size: 16pt;
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
			background-color: rgba(136, 255, 245, 0.753);
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
			padding: 10px;
		}
		.parraf2-cont {
			font-size: 14pt;
		}
		.parraf3-cont {
			font-size: 16pt;
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
			padding: 10px;
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
			background-color: rgba(136, 255, 245, 0.753);
			box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
		}

		.parraf2-cont {
			font-size: 13pt;
		}
		.parraf3-cont {
			font-size: 15pt;
		}
	}
	@media only screen and (max-width: 394px) {
		.parraf3-cont {
			font-size: 15pt;
		}
	}
	@media only screen and (max-width: 388px) {
		.parraf2-cont {
			font-size: 11pt;
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
			padding: 10px;
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
			background-color: rgba(136, 255, 245, 0.753);
			box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
		}

		.parraf3-cont {
			font-size: 14pt;
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
			padding: 10px;
		}
		.parraf3-cont {
			font-size: 14pt;
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
			padding: 10px;
		}
		.parraf3-cont {
			font-size: 14pt;
		}
	}
</style>
