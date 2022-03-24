<script context="module">

    export async function load({page}){
        
        return {
            props: {slug: page.params.slug}
        }
    }

</script>
<script>
    export let slug;
</script>

<h1>
    SLUG PAGE DUDE
</h1>
<p>this slug : {slug}</p>