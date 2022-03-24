<script>
    import '../app.css'
    import Header from '$lib/header.svelte';
    import Footer from '$lib/footer.svelte';
</script>

<Header></Header>
<div>
    <slot></slot>
</div>
<Footer></Footer>