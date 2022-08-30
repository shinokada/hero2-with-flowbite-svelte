---
layout: docLayout
---

<script>
	import { Alert, Heading } from 'flowbite-svelte';
	import { InformationCircle } from 'svelte-heros-v2';
	import ExampleDiv from '../ExampleDiv.svelte';
</script>

<Heading class="mb-2" tag="h1" customSize="text-3xl">Alert</Heading>

<ExampleDiv>
	<Alert class="mb-2">
		<svelte:fragment slot="icon">
			<InformationCircle class="text-blue-700 flex-shrink-0 w-5 h-5 mr-3" />
		</svelte:fragment>
		<span class="font-medium">Info alert!</span> Change a few things up and try submitting again.
	</Alert>
	<Alert color="red" class="mb-2">
		<svelte:fragment slot="icon">
			<InformationCircle class="text-red-700 flex-shrink-0 w-5 h-5 mr-3" />
		</svelte:fragment>
		<span class="font-medium">Danger alert!</span> Change a few things up and try submitting again.
	</Alert>
	<Alert color="green" class="mb-2">
		<svelte:fragment slot="icon">
			<InformationCircle class="text-green-700 flex-shrink-0 w-5 h-5 mr-3" />
		</svelte:fragment>
		<span class="font-medium">Success alert!</span> Change a few things up and try submitting again.
	</Alert>
	<Alert color="yellow" class="mb-2">
		<svelte:fragment slot="icon">
			<InformationCircle class="text-yellow-700 flex-shrink-0 w-5 h-5 mr-3" />
		</svelte:fragment>
		<span class="font-medium">Warning alert!</span> Change a few things up and try submitting again.
	</Alert>
	<Alert color="gray" class="mb-2">
		<svelte:fragment slot="icon">
			<InformationCircle class="text-gray-500 flex-shrink-0 w-5 h-5 mr-3" />
		</svelte:fragment>
		<span class="font-medium">Dark alert!</span> Change a few things up and try submitting again.
	</Alert>
</ExampleDiv>

```html
<script>
	import { Alert } from 'flowbite-svelte';
	import { InformationCircle } from 'svelte-heros-v2';
</script>

<Alert class="mb-2">
	<svelte:fragment slot="icon">
		<InformationCircle class="text-blue-700 flex-shrink-0 w-5 h-5 mr-3" />
	</svelte:fragment>
	<span class="font-medium">Info alert!</span> Change a few things up and try submitting again.
</Alert>
<Alert color="red" class="mb-2">
	<svelte:fragment slot="icon">
		<InformationCircle class="text-red-700 flex-shrink-0 w-5 h-5 mr-3" />
	</svelte:fragment>
	<span class="font-medium">Danger alert!</span> Change a few things up and try submitting again.
</Alert>
<Alert color="green" class="mb-2">
	<svelte:fragment slot="icon">
		<InformationCircle class="text-green-700 flex-shrink-0 w-5 h-5 mr-3" />
	</svelte:fragment>
	<span class="font-medium">Success alert!</span> Change a few things up and try submitting again.
</Alert>
<Alert color="yellow" class="mb-2">
	<svelte:fragment slot="icon">
		<InformationCircle class="text-yellow-700 flex-shrink-0 w-5 h-5 mr-3" />
	</svelte:fragment>
	<span class="font-medium">Warning alert!</span> Change a few things up and try submitting again.
</Alert>
<Alert color="gray" class="mb-2">
	<svelte:fragment slot="icon">
		<InformationCircle class="text-gray-500 flex-shrink-0 w-5 h-5 mr-3" />
	</svelte:fragment>
	<span class="font-medium">Dark alert!</span> Change a few things up and try submitting again.
</Alert>
```