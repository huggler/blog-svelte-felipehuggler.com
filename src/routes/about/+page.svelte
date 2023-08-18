<script>
	import Profile from "../../components/Profile.svelte";
	let birthDay = 17;
	let birthMonth = 10;
	let birthYear = 1983;

	let currentDay = new Date().getDate();
	let currentMonth = new Date().getMonth() + 1; // Mês começa de 0 (janeiro) a 11 (dezembro)
	let currentYear = new Date().getFullYear();

	function calculateAge() {
    let age = currentYear - birthYear;

    if (birthMonth > currentMonth || (birthMonth === currentMonth && birthDay > currentDay)) {
      age--;
    }

    return age;
  }

</script>

<svelte:head>
	<title>Felipe Huggler - Um pouco sobre meu perfil pessoal e profissional</title>
	<meta name="description" content="Sobre Felipe Huggler" />
</svelte:head>

<div class="text-center">
	<Profile />
<div class="text-sm md:text-base">
		<p class="mb-10">
			Meu nome é Felipe Huggler e nasci em 17/101/1983 na cidade de Curitiba/PR e atualmente estou com {calculateAge()} anos de idade
		</p>
		<p class="mb-10">
			Atualmente moro em Piraju, cidade que fica no interior de São Paulo há 400km da capital.
		</p>
		<p class="mb-10">
			Eu tenho 3 filhos e um cachorro e moro junto com minha mulher, que é uma pessoa maravilhosa!
		</p>
		<p class="mb-10">
			Quando eu era criança o meu sonho era ser jogador de futebol, e eu realmente jogava muito bem, chegando a ser destaque em várias competições, porém, o destino não queria que eu seguisse essa carreira e com 10 anos de idade eu cai de um touro mecânico numa dessas festas de rodeio e eu tive uma lesão na coluna.
		</p>
		<p class="mb-10">
			Eu fui operado e graças a Deus, tudo ocorreu bem, porém, tive que abortar o sonho de ser jogador de futebol.
		</p>
		<p class="mb-10">
			Desde então eu comecei a me interessar por tecnologia e na programação foi algo que mexeu comigo.
		</p>
		<p class="mb-10">Era mais ou menos em 1996, na época do ICQ, AOL, Mirc, Internet discada... eu comecei a comprar revistas nas bancas de programação, aquelas que vinham com CD de demonstração.</p>
		<p class="mb-10">Na epóca a linguagem que eu inicie foi ASP, HTML e CSS e logo depois eu descobri que o que fazia a magia acontecer nas aplicações era Javascript!</p>
		<p class="mb-10">Quando eu tinha 18 anos, fui morar no Rio de Janeiro, onde iniciei minha carreira profissional.</p>
		<p class="mb-10">Trabalhei em uma agência de websites, onde eu era o responsável por todo o desenvovlvimento e lembro-me que na época os sites ainda eram feitos em tabelas, as aplicações em ASP e ACCESS...Meu Deus! rs</p>
		<p class="mb-10">Aos poucos eu fui migrando e acompanhando a evolução do mercado, comecei a me dedicar mais na parte do front, sobre tudo em Javascript.</p>
		<p class="mb-10">Dessa agência web, fui contratado para a CMA que é uma das líderes em desenvolvimento de aplicações para o mercado financeiro e depois dela passei pela <strong>XP Investimentos</strong> e <strong>MyCAP</strong></p>
		<p class="mb-10">Também trabalhei para <strong>B2W</strong> onde atuei como frontend das marcas Nike.com, CasasBahia.com, PontoFrio.com, Americanas.com, Shoptime, Submarino e SouBarato</p>
		<p class="mb-10">Trabalhei um tempo para o governo na <strong>ANCINE</strong> - Agencia Nacional do Cinema, onde comecei a programar em React.</p>
		<p class="mb-10">Passei uma fase trabalhando para uma startup chamada <strong>21k</strong> onde fiz o desenvolvimento sistemas de gestão pública, plataformas de redes sociais, aplicativos em React Native, Angular, Sass... e base de dados como Ne4j, Postgres, MySQL</p>
		<p class="mb-10">Em 2018 comecei a trilhar minha jornada como triatleta e me dedicar também aos esporte e em pararelo tocar a Odete.com.br, que é uma plataforma de profissionais diaristas.</p>
		<p class="mb-10">Meus útimos trabalhos foram para uma empresa chamada CellereIt (Campinas) e Woba(MG)</p>
		<p class="mb-10">Atualmente a Odete caminha sozinha e agora estou em busca de novos desafios!</p>
	</div>
</div>
