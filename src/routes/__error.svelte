<script context="module">
    export async function load({error, status}){
        return {
            props: {
                error, status
            }
        }
    }
    
</script>

<script>
    export let error;
    export let status;

    console.log({error, status})

</script>


<h1>
    
    {status}
</h1>
<p>
    {error.message}
    
</p>