<script>
	import { DarkMode } from 'flowbite-svelte';
	import '../app.postcss';
</script>

<DarkMode />
<main class="flex justify-center p-16">
	<slot />
</main>
