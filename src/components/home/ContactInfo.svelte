<script>
</script>

<main>
	<div class="div-info">
		<p>Pastores:</p>
		<strong>Angel Mora y Susi Huamanchay</strong>
		<img alt="logo" src="../images/pastores.svg" />
		<p>Encuéntranos:</p>
		<div class="div-contacts">
			<iframe
				src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3899.3183106615256!2d-76.93774208561517!3d-12.226713448601942!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9105bbe8aadf5343%3A0x26663f263fd980de!2sIglesia%20Emanuel!5e0!3m2!1ses-419!2spe!4v1640474999248!5m2!1ses-419!2spe"
				width="100%"
				height="340"
				style="border:0;"
				allowfullscreen=""
				title="mapa"
				loading="lazy"
			/>
		</div>
		<div class="div-numbers">
			<p>Contáctanos:</p>
			<a class="div-number" id="number1" href="tel:+51984135388">
				<i class="fas fa-phone-alt" />
				<h5>984135388</h5>
			</a>
			<a class="div-number" id="number2" href="tel:+51954222499">
				<i class="fas fa-phone-alt" />
				<h5>954222499</h5>
			</a>
		</div>
	</div>
</main>

<!-- markup (zero or more items) goes here -->
<style>
	@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@600&display=swap');

	.div-contacts {
		display: flex;
		flex-direction: row;
		justify-content: space-evenly;
		align-items: center;
		width: 100%;
	}
	.div-numbers {
		padding-top: 1rem;
	}
	.div-number {
		margin-left: 5px;
		color: #fff;
		transition: color 1s;
		display: flex;
		flex-direction: row;
		align-items: center;
		text-decoration: none;
	}
	a:hover {
		color: rgb(129, 114, 102);
	}
	h5 {
		font-size: 30px;
	}
	.fas {
		margin-right: 5px;
		font-size: 25px;
	}
	.div-info {
		display: flex;
		flex-direction: column;
		justify-content: flex-start;
		align-items: center;
		left: 15%;
		right: 15%;
		position: absolute;
		z-index: 1;
		height: 63rem;
		border-radius: 35px;
		padding: 2.5rem;
		margin-top: 6rem;
		background-color: rgba(129, 188, 218, 0.1);
		box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
	}
	p {
		color: #fff;
		text-align: center;
		font-size: 30px;
		font-weight: 200;
		margin: 0;
		padding: 0;
	}
	strong {
		color: #fff;
		text-align: center;
		font-size: 30px;
		margin: 0;
		font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		font-weight: 500;
	}
	img {
		height: 20rem;
	}
	@media only screen and (max-width: 649px) {
		strong {
			color: #fff;
			text-align: center;
			font-size: 25px;
			margin: 0;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
			font-weight: 500;
		}
	}
	@media only screen and (max-width: 555px) {
		strong {
			color: #fff;
			text-align: center;
			font-size: 25px;
			margin: 0;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
			font-weight: 500;
		}
		.div-info {
			display: flex;
			flex-direction: column;
			justify-content: flex-start;
			align-items: center;
			left: 15%;
			right: 15%;
			position: absolute;
			z-index: 1;
			height: 63rem;
			border-radius: 35px;
			padding: 2.5rem;
			margin-top: 6rem;
			background-color: rgba(129, 188, 218, 0.1);
			box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
		}
		h5 {
			font-size: 25px;
		}
		.fas {
			margin-right: 5px;
			font-size: 25px;
		}
	}
	@media only screen and (max-width: 430px) {
		strong {
			color: #fff;
			text-align: center;
			font-size: 20px;
			margin: 0;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
			font-weight: 500;
		}
		.div-info {
			display: flex;
			flex-direction: column;
			justify-content: flex-start;
			align-items: center;
			left: 15%;
			right: 15%;
			position: absolute;
			z-index: 1;
			height: 60rem;
			border-radius: 35px;
			padding: 2.5rem;
			margin-top: 6rem;
			background-color: rgba(129, 188, 218, 0.1);
			box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
		}
		img {
			height: 17rem;
		}
	}
	@media only screen and (max-width: 365px) {
		strong {
			color: #fff;
			text-align: center;
			font-size: 20px;
			margin: 0;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
			font-weight: 500;
		}
		.div-info {
			display: flex;
			flex-direction: column;
			justify-content: flex-start;
			align-items: center;
			left: 15%;
			right: 15%;
			position: absolute;
			z-index: 1;
			height: 55rem;
			border-radius: 35px;
			padding: 2.5rem;
			margin-top: 6rem;
			background-color: rgba(129, 188, 218, 0.1);
			box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
		}
		img {
			transition: height 1s;
			height: 12rem;
		}
	}
	@media only screen and (max-width: 290px) {
		strong {
			color: #fff;
			text-align: center;
			font-size: 20px;
			margin: 0;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
			font-weight: 500;
		}
		.div-info {
			display: flex;
			flex-direction: column;
			justify-content: flex-start;
			align-items: center;
			left: 15%;
			right: 15%;
			position: absolute;
			z-index: 1;
			height: 58rem;
			border-radius: 35px;
			padding: 2.5rem;
			margin-top: 6rem;
			background-color: rgba(129, 188, 218, 0.1);
			box-shadow: -1px 2px 2px 2px rgba(0, 0, 0, 0.2);
		}
		img {
			transition: height 1s;
			height: 12rem;
		}
	}
</style>
