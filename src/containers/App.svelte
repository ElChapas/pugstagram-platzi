<script>
    import { onMount } from 'svelte';
    import Header from '../components/Header.svelte';
    import Main from '../components/Main.svelte';
    import Timeline from '../components/Timeline.svelte';
    import Sidebar from '../components/Sidebar.svelte';

    let data = {};

    onMount( async () => {
        const response = await fetch('https://us-central1-pugstagram-co.cloudfunctions.net/data')
        data = await response.json()
    })

    
</script>

<style>
    :global(body) {
        background-color: white;
        color: #203D44;
        font-family: 'Lato', sans-serif;
        margin:0;
        padding: 0
    }

    :global(h1, h2, h3) {
        margin: 0;
        padding: 0;
    }
    
    :global(li) {
        list-style: none;
        color: black
    }
</style>

<Header />
<Main>
    <Timeline posts={data.posts} />
    <Sidebar {...data.user} />
</Main>