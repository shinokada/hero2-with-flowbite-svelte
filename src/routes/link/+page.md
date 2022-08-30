---
layout: docLayout
---

<script>
	import { P, A, Heading } from 'flowbite-svelte';
	import { ChevronDoubleRight } from 'svelte-heros-v2';
	import ExampleDiv from '../ExampleDiv.svelte';
</script>

<Heading class="mb-2" tag="h1" customSize="text-3xl">Link</Heading>

<ExampleDiv>
<P>
  500,000 people have made over a million apps with Glide. <A
		href="/"
		textColor="text-blue-600 dark:text-blue-500"
		aClass="inline-flex items-center font-medium  hover:underline"
	>
		Read their stories
		<ChevronDoubleRight />
	</A>
</P>
</ExampleDiv>

```html
<P>
  500,000 people have made over a million apps with Glide. <A
		href="/"
		textColor="text-blue-600 dark:text-blue-500"
		aClass="inline-flex items-center font-medium  hover:underline"
	>
		Read their stories
		<ChevronDoubleRight />
	</A>
</P>
```
