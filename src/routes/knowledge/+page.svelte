<script>
	let items = ['HTML', 'CSS', 'UM POUQUINHO DE PROGRAMAÇÃO', 'BANCO DE DADOS', 'USABILIDADE', 'SEGURANÇA', 'INFRA'];
</script>

<svelte:head>
	<title>Um pouco do que eu sei...</title>
	<meta name="description" content="Um pouco do que eu sei..." />
</svelte:head>

<div class="text-center">
	<h1 class="text-3xl mb-3">Um pouco do que eu sei...pra testar o hover do tailwind!</h1>

	{#each items as item}
	  <p class="rounded-full bg-slate-800 mb-2 text-white p-2 hover:bg-cyan-600">{item}</p>
	{/each}

	<p class="mb-8">Quer saber mais, só me chamar!</p>
	
</div>