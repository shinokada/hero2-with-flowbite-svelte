<script>
	import { Toast } from 'flowbite-svelte';
	import { Camera } from 'svelte-heros-v2';
</script>

<Toast>
	<svelte:fragment slot="icon">
		<Camera />
	</svelte:fragment>
	Dismissable user notification.
</Toast>
