<script>
    import '../app.css';
    import Header from './Header.svelte';
    /** @type {{ data: import('./$types').LayoutData, children: import('svelte').Snippet }} */
    let { data, children } = $props();
</script>

<Header />

{@render children()}
