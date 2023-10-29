<script lang="ts">
	import '../app.postcss';
	import { AppShell } from '@skeletonlabs/skeleton';
	import Nav from './nav.svelte';
</script>

<!-- App Shell -->
<AppShell>
	<svelte:fragment slot="header"><Nav /></svelte:fragment>
	<!-- Page Route Content -->
	<slot />
</AppShell>
