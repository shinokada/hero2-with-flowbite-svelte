---
layout: docLayout
---

<script>
  import { Hr, P, Heading } from 'flowbite-svelte';
  import { PaperClip } from 'svelte-heros-v2';
  import ExampleDiv from '../ExampleDiv.svelte';
</script>

<Heading class="mb-2" tag="h1" customSize="text-3xl">Hr</Heading>

<ExampleDiv class="text-center p-8">
  <P>Track work across the enterprise throug ...</P>
  <Hr class="my-8 " width="w-64" height="h-1" middleBgColor="dark:bg-gray-800" icon>
    <PaperClip class="w-5 h-5 text-gray-700 dark:text-gray-300" />
  </Hr>
  <P>Deliver great service experiences fast - without ...</P>
</ExampleDiv>

```html
<script>
  import { Hr, P } from 'flowbite-svelte';
  import { PaperClip } from 'svelte-heros-v2';
</script>

<P>Track work across the enterprise throug ...</P>
<Hr class="my-8 " width="w-64" height="h-1" middleBgColor="dark:bg-gray-800" icon>
  <PaperClip class="w-5 h-5 text-gray-700 dark:text-gray-300" />
</Hr>
<P>Deliver great service experiences fast - without ...</P>
```
