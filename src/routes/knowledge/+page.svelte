<script>
	let items = ['HTML', 'CSS', 'JAVASCRIPT', 'NODEJS', 'REACT', 'MONGODB', 'SQLSEVER', 'MYSQL', 'USABILIDADE', 'ACESSIBILIDADE', 'BOOTSTRAP', 'MATERIAL-UI', 'TAILWIND', 'SEGURANÇA', 'INFRA'];
</script>

<svelte:head>
	<title>Um pouco do que eu sei...</title>
	<meta name="description" content="Um pouco do que eu sei..." />
</svelte:head>

<div class="text-center">
	<h1 class="title text-3xl font-medium md:text-4xl mb-4">Quem é Felipe Huggler?</h1>
	<img src="/images/felipe-huggler.jpg" class="m-auto rounded-full mb-10" alt="Felipe Huggler Luz" />

	<p class="mb-6">Um pouco do que eu aprendi no decorrer da minha carreira... e pra testar o hover do tailwind :)</p>

		<ul class="container m-auto grid grid-cols-1 md:grid-cols-3 gap-4 mb-4">

	{#each items as item}
	  <li class="rounded-full bg-slate-800 mb-2 text-white p-2 hover:bg-cyan-600">{item}</li>
	{/each}
</ul>

	<p class="mb-8">Quer saber mais, só me chamar!</p>

	<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 m-auto mb-6">
		<path stroke-linecap="round" stroke-linejoin="round" d="M19.5 13.5L12 21m0 0l-7.5-7.5M12 21V3" />
	  </svg>
	  
	
</div>