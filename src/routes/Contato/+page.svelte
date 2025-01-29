<script>
	let contacts = [
		{
			id: 1,
			name: 'Maria Silva',
			phone: '(11) 91234-5678',
			email: 'maria.silva@example.com',
			specialty: 'Limpeza'
		},
		{
			id: 2,
			name: 'Joãna Pereira',
			phone: '(11) 92345-6789',
			email: 'joana.pereira@example.com',
			specialty: 'Lavagem de Roupa'
		},
		{
			id: 3,
			name: 'Carlos Costa',
			phone: '(11) 93456-7890',
			email: 'carlos.costa@example.com',
			specialty: 'Cozinha'
		},
		{
			id: 4,
			name: 'Marnie Oliveira',
			phone: '(11) 94567-8901',
			email: 'marnie.oliveira@example.com',
			specialty: 'Jardinagem'
		},
		{
			id: 5,
			name: 'Fernanda Souza',
			phone: '(11) 95678-9012',
			email: 'fernanda.souza@example.com',
			specialty: 'Babá'
		},
		{
			id: 6,
			name: 'Ricardo Mendes',
			phone: '(11) 96789-0123',
			email: 'ricardo.mendes@example.com',
			specialty: 'Manutenção'
		}
	];
</script>

<h1>Contatos dos Profissionais</h1>
<ul class="contact-list">
	{#each contacts as contact}
		<li class="contact-item">
			<h2>{contact.name}</h2>
			<p><strong>Especialidade:</strong> {contact.specialty}</p>
			<p><strong>Telefone:</strong> {contact.phone}</p>
			<p><strong>E-mail:</strong> <a href={'mailto:' + contact.email}>{contact.email}</a></p>
		</li>
	{/each}
</ul>

<style>
	.contact-list {
		list-style-type: none;
		padding: 0;
	}
	.contact-item {
		border: 1px solid #ccc;
		margin: 10px 0;
		padding: 10px;
		border-radius: 5px;
	}
</style>
