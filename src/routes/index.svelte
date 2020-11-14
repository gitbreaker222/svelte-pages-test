<script>
</script>

<div class="layout">
	<div class="card">
		<h1>Digital!</h1>
		<h2>On . leicht</h2>
	</div>
</div>

<style>
  .layout {
		flex: 1;
		display: grid;
		place-items: center;
	}

	.card {
		width: 100%;
		max-width: 11cm;
		border-radius: 3px;
		text-align: center;
		box-shadow: 0 0 2px #ccc;
		background: #f1f1f1;
	}

	h1 {
		color: rebeccapurple;
		text-transform: uppercase;
		font-size: 3rem;
		font-weight: 100;
		line-height: 1.1;
		margin: 2rem auto;
		max-width: 14rem;
	}

	@media (min-width: 480px) {
		h1 {
			font-size: 4rem;
		}
	}
	@media (min-height: 480px) {
		h1 {
			margin: 4rem auto;
		}
	}
</style>