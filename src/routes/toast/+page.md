---
layout: docLayout
---

<script>
	import { Toast, Heading } from 'flowbite-svelte';
	import { Camera } from 'svelte-heros-v2';
	 import ExampleDiv from '../ExampleDiv.svelte';
</script>

<Heading class="mb-2" tag="h1" customSize="text-3xl">Toast</Heading>

<ExampleDiv>
<Toast>
	<svelte:fragment slot="icon">
		<Camera />
	</svelte:fragment>
	Dismissable user notification.
</Toast>
</ExampleDiv>

```html
<Toast>
	<svelte:fragment slot="icon">
		<Camera />
	</svelte:fragment>
	Dismissable user notification.
</Toast>
```