---
layout: docLayout
---

<script>
  import { Breadcrumb, BreadcrumbItem, Heading } from 'flowbite-svelte';
  import { Home, ChevronDoubleRight } from 'svelte-heros-v2';
  import ExampleDiv from '../ExampleDiv.svelte';
</script>

<Heading class="mb-2" tag="h1" customSize="text-3xl">Breadcrumb</Heading>

<ExampleDiv>
  <Breadcrumb
    aria-label="Solid background breadcrumb example"
    class="bg-gray-50 py-3 px-5 dark:bg-gray-900">
    <BreadcrumbItem href="/" home>
      <svelte:fragment slot="icon">
        <Home />
      </svelte:fragment>Home</BreadcrumbItem>
    <BreadcrumbItem href="/">
      <svelte:fragment slot="icon">
        <ChevronDoubleRight />
      </svelte:fragment>
      Projects</BreadcrumbItem>
    <BreadcrumbItem>
      <svelte:fragment slot="icon">
        <ChevronDoubleRight />
      </svelte:fragment>
      Flowbite Svelte</BreadcrumbItem>
  </Breadcrumb>
</ExampleDiv>

```html
<script>
  import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
  import { Home, ChevronDoubleRight } from 'svelte-heros-v2';
</script>

<Breadcrumb
  aria-label="Solid background breadcrumb example"
  class="bg-gray-50 py-3 px-5 dark:bg-gray-900">
  <BreadcrumbItem href="/" home>
    <svelte:fragment slot="icon">
      <Home />
    </svelte:fragment>Home</BreadcrumbItem>
  <BreadcrumbItem href="/">
    <svelte:fragment slot="icon">
      <ChevronDoubleRight />
    </svelte:fragment>
    Projects</BreadcrumbItem>
  <BreadcrumbItem>
    <svelte:fragment slot="icon">
      <ChevronDoubleRight />
    </svelte:fragment>
    Flowbite Svelte</BreadcrumbItem>
</Breadcrumb>
````
