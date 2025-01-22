<script>
	let { children } = $props();
</script>

<nav class="navbar navbar-expand-sm bg-body-tertiary">
	<div class="container-fluid">
		<a class="navbar-brand" href="/#">DW4</a>
		<button
			class="navbar-toggler"
			type="button"
			data-bs-toggle="collapse"
			data-bs-target="#navbarSupportedContent"
			aria-controls="navbarSupportedContent"
			aria-expanded="false"
			aria-label="Toggle navigation"
		>
			<span class="navbar-toggler-icon"></span>
		</button>
		<div class="collapse navbar-collapse" id="navbarSupportedContent">
			<ul class="navbar-nav">
				<li class="nav-item">
					<a class="nav-link" href="/temperatura">temperatura</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/about">Sobre</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/Notas">calcular notas</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/Usuario">cadastro</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/custo.carro">Carros</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/idade">votar</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/idade2">carteira de motorista</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/conversaoLR">conversão para reais</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/frutas">lista de frutas</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/cores">mudar cores</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/lista-tarefas">lista de tarefas</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/cartas">cartas</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/coelhos">fibonacc</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/filmes">filmes</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/compras">compras</a>
				</li>
			</ul>
		</div>
	</div>
</nav>

{@render children()}
