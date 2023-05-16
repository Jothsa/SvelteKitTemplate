<script lang="ts">
  import '$styles/index.css';
  import { onMount } from 'svelte';
  import { page } from '$app/stores';
  import type { LayoutData } from './$types';
  export let data: LayoutData;
</script>

<svelte:head>
  <title>{$page.data.title}</title>
</svelte:head>

<h1>{$page.data.title}</h1>
<slot />
