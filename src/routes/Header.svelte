<script>
	import { page } from '$app/stores';
</script>

<header class="bg-black text-white py-4 px-6 sticky top-0 z-10">
<div class="container mx-auto flex items-center justify-between">
	<div class="flex items-center gap-4">
	<img
		src="./images/isoneg.png"
		width="60"
		height="40"
		alt="Restaurant Logo"
		class="rounded-full"
		style="aspect-ratio: 60 / 40; object-fit: cover"
	/>
	<h1 class="text-xl font-bold">Soluwebstaurant</h1>
	</div>
	<ul class="container mx-auto flex justify-end">
		<li class=" mx-4" aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
			<a href="/">Home</a>
		</li>
		<li  class=" mx-4" aria-current={$page.url.pathname === '/carta' ? 'page' : undefined}>
			<a href="/most">Carta</a>
		</li>
		<li  class=" mx-4" aria-current={$page.url.pathname ==='/sverdle' ? 'page' : undefined}>
			<a href="/sesiones">sesiones</a>
		</li>
	</ul>

</div>
</header>
