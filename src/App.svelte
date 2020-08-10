<script>
    import Navbar from './Navbar.svelte';
    const items = [
        {
            link: "/",
            name: "Root"
        },
        {
            link: "/",
            name: "Other stuff"
        },
        {
            link: "/",
            name: "More stuff"
        },
    ]
</script>

<Navbar {items}/>
<body>
    {#each { length: 100 } as _, _}
    <h1>Hello world!<br/></h1>
    {/each}
</body>

<style>
  body {
    padding: 5%;
    padding-top: 60px;
  }
</style>
