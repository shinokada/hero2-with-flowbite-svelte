<script>
	import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
	import { Home, ChevronDoubleRight } from 'svelte-heros-v2';
</script>

<Breadcrumb
	aria-label="Solid background breadcrumb example"
	class="bg-gray-50 py-3 px-5 dark:bg-gray-900"
>
	<BreadcrumbItem href="/" home>
		<svelte:fragment slot="icon">
			<Home />
		</svelte:fragment>Home</BreadcrumbItem
	>
	<BreadcrumbItem href="/">
		<svelte:fragment slot="icon">
			<ChevronDoubleRight />
		</svelte:fragment>
		Projects</BreadcrumbItem
	>
	<BreadcrumbItem>
		<svelte:fragment slot="icon">
			<ChevronDoubleRight />
		</svelte:fragment>
		Flowbite Svelte</BreadcrumbItem
	>
</Breadcrumb>
