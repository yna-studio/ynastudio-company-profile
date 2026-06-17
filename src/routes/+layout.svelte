<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import { resolve } from '$app/paths';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>YNA Studio</title>
	<meta name="description" content="Digitalisasi yang Tepat, Bisnis Makin Hebat. YNA Studio bantu meNgembangkan bisnis anda. Dengan
		pengalaman bertahun-tahun di berbagai bidang INdustri. portofolio KAMI berbicara tentang
		keberagaman dan fleksibilitas pekerjaan kami" />
</svelte:head>
<header>
	<nav aria-label="Global" class="mx-auto flex max-w-full items-center justify-between p-6 lg:px-8">
		<div class="flex lg:flex-1">
			<!-- This will not trigger the lint error -->
			<a href={resolve('/')} class="-m-1.5 p-1.5">
				<span class="sr-only">Your Company</span>
				<img src="/images/YNA Studio Logo.png" alt="Logo of YNA Studio" class="h-12 w-auto" />
			</a>
		</div>
	</nav>
</header>
<main>
	{@render children()}
</main>
