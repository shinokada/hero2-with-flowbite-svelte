---
layout: docLayout
---

<script>
	import { AccordionItem, Heading } from 'flowbite-svelte';
	import { ArrowDownCircle, ArrowUpCircle } from 'svelte-heros-v2';
	import ExampleDiv from '../ExampleDiv.svelte';
</script>

<Heading class="mb-2" tag="h1" customSize="text-3xl">Accordion</Heading>

<ExampleDiv>
	<AccordionItem id="1">
		<h2 slot="header">Header 2-1</h2>
		<div slot="arrowup">
			<ArrowUpCircle />
		</div>
		<div slot="arrowdown">
			<ArrowDownCircle />
		</div>
		<div slot="body">
			<p class="mb-2 text-gray-500 dark:text-gray-400">
				Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint
				explicabo ...
			</p>
		</div>
	</AccordionItem>
	<AccordionItem id="2">
		<h2 slot="header">Header 2-2</h2>
		<div slot="arrowup">
			<ArrowUpCircle />
		</div>
		<div slot="arrowdown">
			<ArrowDownCircle />
		</div>
		<div slot="body">
			<p class="mb-2 text-gray-500 dark:text-gray-400">
				Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint
				explicabo ...
			</p>
		</div>
	</AccordionItem>
</ExampleDiv>

```html
<script>
	import { AccordionItem } from 'flowbite-svelte';
	import { ArrowDownCircle, ArrowUpCircle } from 'svelte-heros-v2';
</script>

<AccordionItem id="1">
	<h2 slot="header">Header 2-1</h2>
	<div slot="arrowup">
		<ArrowUpCircle />
	</div>
	<div slot="arrowdown">
		<ArrowDownCircle />
	</div>
	<div slot="body">
		<p class="mb-2 text-gray-500 dark:text-gray-400">
			Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint
			explicabo ...
		</p>
	</div>
</AccordionItem>
<AccordionItem id="2">
	<h2 slot="header">Header 2-2</h2>
	<div slot="arrowup">
		<ArrowUpCircle />
	</div>
	<div slot="arrowdown">
		<ArrowDownCircle />
	</div>
	<div slot="body">
		<p class="mb-2 text-gray-500 dark:text-gray-400">
			Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint
			explicabo ...
		</p>
	</div>
</AccordionItem>
```
