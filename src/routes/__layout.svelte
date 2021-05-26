<script lang="ts">
import '../app.css';
import '$lib/themes/main.css';
import Header from '$lib/layout/Header.svelte';
</script>

<Header />

<main>
    <slot />
</main>

<style>
main {
    position: relative;
    top: var(--header-height);
    display: flex;
    flex-flow: row nowrap;
    align-items: center;
    justify-content: center;
}
</style>
