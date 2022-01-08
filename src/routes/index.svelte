<script>
	import InfoSection from '../components/home/info.svelte';
	import Navbar from '../components/Navbar.svelte';
	import Footer from '../components/footer.svelte';
	import CompSocial from '../components/social_component.svelte';
	import CompParallax from '../components/parallax_comp.svelte';
	import CultosInfo from '../components/home/cultosInfo.svelte';
	import ContactInfo from '../components/home/ContactInfo.svelte';
</script>

<!-- markup (zero or more items) goes here 'about' -->
<svelte:head>
	<title>Iglesia Emanuel</title>
</svelte:head>
<Navbar />
<main>
	<div class="container-top__home">
		<h1 class="animate__animated animate__backInDown">BIENVENIDOS</h1>
		<h3 class="animate__animated animate__flipInX animate__slower">Somos la iglesia Emanuel</h3>
		<CompSocial />
	</div>
	<CompParallax iURL="../images/fondo2.jpg" sHeight="50" sPadding="10" />
	<InfoSection />
	<CompParallax iURL="../images/fondo3.jpg" sHeight="50" sPadding="10" />
	<CultosInfo />
	<CompParallax iURL="../images/fondo7.jpg" sHeight="60" sPadding="10" />
	<ContactInfo />
	<CompParallax iURL="../images/fondo9.jpg" sHeight="75" sPadding="10" bright="0.1" />

	<Footer />
</main>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@600&display=swap');
	main {
		position: absolute;
		top: 0;
		width: 100%;
		padding: 0;
		margin: 0;
		z-index: 0;
	}
	div {
		width: 100%;
	}
	.container-top__home {
		position: absolute;
		display: flex;
		flex-direction: column;
		align-items: center;
		top: 250px;
		left: 0;
		right: 0;
		z-index: 1;
		line-height: 2pt;
	}
	h1 {
		color: #fff;
		font-size: 80pt;
		font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
	}
	h3 {
		color: #fff;
		font-weight: 100;
		font-size: 20pt;
		text-align: center;
	}
	@media only screen and (max-width: 610px) {
		h1 {
			color: #fff;
			font-size: 60pt;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
	}
	@media only screen and (max-width: 500px) {
		h1 {
			color: #fff;
			font-size: 50pt;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		h3 {
			color: #fff;
			font-weight: 100;
			font-size: 16pt;
			text-align: center;
		}
	}
	@media only screen and (max-width: 392px) {
		h1 {
			color: #fff;
			font-size: 40pt;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		h3 {
			color: #fff;
			font-weight: 100;
			font-size: 14pt;
			text-align: center;
		}
	}
	@media only screen and (max-width: 300px) {
		h1 {
			color: #fff;
			font-size: 30pt;
			font-family: 'Oswald', Helvetica, sans-serif, Arial, sans-serif;
		}
		h3 {
			color: #fff;
			font-weight: 100;
			font-size: 13pt;
			text-align: center;
		}
	}
</style>
