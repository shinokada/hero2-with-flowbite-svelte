<script>
  import {
    DarkMode,
    Navbar,
    NavBrand,
    NavHamburger,
    NavUl,
    NavLi,
    MegaMenu,
    NavDropdown
  } from 'flowbite-svelte';
  import '../app.postcss';
  let menu = [
    { name: 'Accordion', href: '/accordion' },
    { name: 'Alert', href: '/alert' },
    { name: 'Breadcrumb', href: '/breadcrumb' },
    { name: 'Carousel', href: '/carousel' },
    { name: 'Hr', href: '/hr' },
    { name: 'Link', href: '/link' },
    { name: 'Textarea', href: '/textarea' },
    { name: 'Toast', href: '/toast' },
    { name: 'Toolbar', href: '/toolbar' }
  ];
  let btnClass =
    'text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 focus:outline-none focus:ring-4 focus:ring-gray-200 dark:focus:ring-gray-700 rounded-lg text-sm p-2.5 fixed right-2 top-16 z-50';
</script>

<Navbar let:hidden let:toggle>
  <NavBrand href="/">
    <img
      src="https://flowbite-svelte.com//images/flowbite-svelte-icon-logo.svg"
      class="mr-3 h-6 sm:h-9"
      alt="Flowbite Logo" />
    <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white"
      >Svelte-Heros-v2 with Flowbite Svelte</span>
  </NavBrand>
  <NavHamburger on:click={toggle} />
  <NavUl {hidden}>
    <NavLi href="/">Home</NavLi>
    <NavDropdown name="Examples">
      <MegaMenu items={menu} let:item>
        <a href={item.href} class="hover:text-blue-600 dark:hover:text-blue-500">{item.name}</a>
      </MegaMenu>
    </NavDropdown>
    <NavLi href="https://flowbite-svelte.com/">Flowbite-Svelte</NavLi>
    <NavLi href="https://github.com/themesberg/flowbite-svelte">GitHub</NavLi>
  </NavUl>
</Navbar>

<DarkMode {btnClass} />
<main class="mx-auto p-24 xl:pb-24 lg:pb-16 lg:pl-64">
  <slot />
</main>
