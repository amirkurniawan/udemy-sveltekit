<script context="module">

    export async function load({page}){
        const Post = await import(`../../posts/${page.params.slug}.md`)
        
        return {
            props: {Post: Post.default, slug: page.params.slug}
        }
    }

</script>
<script>
    // export let slug;
    export let Post;
</script>

<!-- <h1>
    SLUG PAGE DUDE
</h1>
<p>this slug : {slug}</p> -->

<!-- <Post/> -->

<svelte:component this={Post}/>