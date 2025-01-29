<script>
	import Poema from '$lib/Poema.svelte';
	
    // Lista de serviços domésticos
    let services = [
        { id: 1, name: "Limpeza Geral", description: "Limpeza completa da casa" },
        { id: 2, name: "Lavagem de Roupa", description: "Lavagem e secagem de roupas" },
        { id: 3, name: "Cozinha", description: "Preparação de refeições" },
        { id: 4, name: "Jardinagem", description: "Cuidados com o jardim" },
        { id: 5, name: "Babá", description: "Cuidados infantis" },
        { id: 6, name: "Manutenção", description: "Reparos e manutenção geral" }
    ];
</script>

<style>
    .service-list {
        list-style-type: none;
        padding: 0;
    }
    .service-item {
        border: 1px solid #ccc;
        margin: 10px 0;
        padding: 10px;
        border-radius: 5px;
    }
</style>

<h1>Serviços Domésticos</h1>
<ul class="service-list">
    {#each services as service}
        <li class="service-item">
            <h2>{service.name}</h2>
            <p>{service.description}</p>
        </li>
    {/each}
</ul>


<h1>seja bem vindo a nosso site de serviços domésticos</h1>
<Poema /> 
 
