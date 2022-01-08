<script>
	import { socialinks } from './home/social-links';
	export let marginTop = 2;
</script>

<div
	style="margin-top:{marginTop}rem"
	class="animate__animated animate__zoomInUp animate__delay-1s"
>
	{#each socialinks as sc}
		<a rel="nofollow noopener noreferrer" target="_blank" href={sc.URL}>
			<i class="fab {sc.icon}" />
		</a>
	{/each}
</div>

<style>
	div {
		width: 100%;
		display: flex;
		flex-direction: row;
		justify-content: center;
	}
	.fab {
		color: #fff;
		font-size: 30px;
		padding-right: 10px;
		padding-left: 10px;
		transition: color 1s;
	}
	.fa-facebook:hover {
		color: #5377f3;
		transition: color 1s;
	}
	.fa-instagram:hover {
		color: #e986d8;
		transition: color 1s;
	}
</style>
