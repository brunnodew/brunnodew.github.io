<script>
	let np, nt, ns;
	let nf = $state(0);

	function calcularnota() {
		nf = (5 * np + 3 * ns + 2 * nt) / 10;
	}
</script>

<h1>Boletim Escolar</h1>

Nota da prova:
<input type="number" bind:value={np} min="0" max="10" />
<br />

Nota do trabalho:
<input type="number" bind:value={nt} min="0" max="10" />
<br />

Nota do seminário:
<input type="number" bind:value={ns} min="0" max="10" />
<br />

<button onclick={calcularnota}> Calcular a nota final!</button>

<p>Tua nota final é: {nf}</p>

{#if nf >= 8.5}
	<p>Aprovado!😀</p>
{:else if 7 < nf}
	<p>Aprovado 🙂</p>
{:else if 5 < nf}
	<p>recuperação 😐</p>
{:else if 2.5 < nf}
	<p>recuperação ☹️</p>
{:else}
	<p>reprovado 😭</p>
{/if}
