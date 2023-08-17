<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/svelte-logo.svg';
	import github from '$lib/images/github.svg';
</script>

<header class="flex justify-center">
	<nav class="flex justify-center">
		<ul class="relative p-0 m-0 flex justify-center content-center list-none h-12">
			<li aria-current={$page.url.pathname === '/' ? 'page' : undefined} class="relative h-full">
				<a href="/" class="flex h-full items-center uppercase px-2 font-bold text-sm">Home</a>
			</li>
			<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined} class="relative h-full">
				<a href="/about" class="flex h-full items-center uppercase px-2 font-bold text-sm">About</a>
			</li>
			<li aria-current={$page.url.pathname.startsWith('/knowledge') ? 'page' : undefined} class="relative h-full">
				<a href="/knowledge" class="flex h-full items-center uppercase px-2 font-bold text-sm">Knowledge</a>
			</li>
		</ul>
	</nav>

	<div class="absolute top-3 right-3">
		<a href="https://github.com/huggler" target="_blank" class="block">
			<img src={github} alt="GitHub Huggler" width="24" height="24" />
		</a>
	</div>
</header>

<style>
	li[aria-current='page']::before {
		--size: 6px;
		content: '';
		width: 0;
		height: 0;
		position: absolute;
		top: 0;
		left: calc(50% - var(--size));
		border: var(--size) solid transparent;
		border-top: var(--size) solid var(--color-theme-2);
	}

	nav a {
		color: var(--color-text);
		transition: color 0.2s linear;
	}

	a:hover {
		color: var(--color-theme-2);
	}
</style>
