<div class="grid-inputFields">
    {#each fields as field}
        <InputField fieldTitle={field.name} fieldType={field.type} />        
    {/each}
</div>

<script>

    import InputField from '$lib/auth/inputField/+page.svelte';
    export let fields;

</script>

<style lang="scss">
    .grid-inputFields{
        grid-column:3/13;
        grid-row:4/10;
        
        display:flex;
        display: -ms-flexbox;
        display: -webkit-flex;
        
        flex-direction:column;  
        justify-content: center;
        align-items: center;
    }
</style>