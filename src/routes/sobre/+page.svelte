<script>
	let professionals = [
		{
			id: 1,
			name: 'Maria Silva',
			specialty: 'Limpeza',
			description: 'Experiente em limpeza geral e detalhada.',
			photo: 'tome.png'
		},
		{
			id: 2,
			name: 'Joãna Pereira',
			specialty: 'Lavagem de Roupa',
			description: 'Especialista em cuidados com tecidos delicados.',
			photo: 'tome2.png'
		},
		{
			id: 3,
			name: 'Carlos Costa',
			specialty: 'Cozinha',
			description: 'Chef de cozinha com experiência em diversas culinárias.',
			photo: 'tome3.png'
		},
		{
			id: 4,
			name: 'Marnie Oliveira',
			specialty: 'Jardinagem',
			description: 'Amante da natureza, cuida de jardins e plantas com carinho.',
			photo: 'tome4.png'
		},
		{
			id: 5,
			name: 'Fernanda Souza',
			specialty: 'Babá',
			description: 'Cuidadora dedicada com vasta experiência em cuidar de crianças.',
			photo: 'tome5.png'
		},
		{
			id: 6,
			name: 'Ricardo Mendes',
			specialty: 'Manutenção',
			description: 'Habilidoso em reparos e manutenção de casa.',
			photo: 'tome6.png'
		}
	];
</script>

<p>
	nosso site é especializado em encontrar e fornecer melhores servoços domesticos com proficionais
	qualificados e dedicados ao seus deveres
	<br />
	SEGUE UMA LISTA DE ALGUNS DOS PROFISSIONAIS:
</p>

<h1>Profissionais de Serviços Domésticos</h1>
<ul class="professional-list">
	{#each professionals as professional}
		<li class="professional-item">
			<img src={professional.photo} alt={professional.name} />
			<h2>{professional.name}</h2>
			<p><strong>Especialidade:</strong> {professional.specialty}</p>
			<p>{professional.description}</p>
		</li>
	{/each}
</ul>

<style>
	.professional-list {
		display: grid;
		grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
		gap: 20px;
		list-style-type: none;
		padding: 0;
	}
	.professional-item {
		border: 1px solid #ccc;
		padding: 10px;
		border-radius: 5px;
		text-align: center;
	}
	.professional-item img {
		border-radius: 50%;
		width: 100px;
		height: 100px;
	}
</style>
