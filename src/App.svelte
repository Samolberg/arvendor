<script>
    import Navbar from './Navbar.svelte';
    import Landing from './Landing.svelte';
    import Content from './Content.svelte';
    
    const navItems = [
        {
            link: "/",
            name: "Firmast"
        },
        {
            link: "/",
            name: "Teenused"
        },
        {
            link: "/",
            name: "Hinnakiri"
        },
        {
            link: "/",
            name: "Kontakt"
        }
    ]

</script>


<Navbar {navItems}/>
<Landing/>
<Content/>
   


