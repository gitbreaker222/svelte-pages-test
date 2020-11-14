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
		width: 11cm;
		border-radius: 3px;
		text-align: center;
		box-shadow: 0 0 2px #ccc;
		background: #f1f1f1;
	}

	h1 {
		color: rebeccapurple;
		text-transform: uppercase;
		font-size: 4rem;
		font-weight: 100;
		line-height: 1.1;
		margin: 4rem auto;
		max-width: 14rem;
	}

	@media (min-width: 480px) {
		h1 {
			max-width: none;
		}

		p {
			max-width: none;
		}
	}
</style>