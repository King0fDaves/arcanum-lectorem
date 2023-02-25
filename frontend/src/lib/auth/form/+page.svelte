<div class="loginForm__form">
<form class="grid-loginForm__form">
    <Title title={title} />
    <InputFields fields={fields} />
    <Button btnTitle={btnTitle}/>

    <p class="redirect">{redirectMessage} <a class="redirectLink" href='/{redirectLink}'>{redirectTitle}</a> </p>
</form>

</div>
<script>
    import Title from "$lib/auth/title/+page.svelte";
    import Button from "$lib/auth/button/+page.svelte";
    import InputFields from"$lib/auth/inputFields/+page.svelte";

    export let title;
    export let btnTitle;
    export let fields;

    export let redirectMessage;
    export let redirectLink;
    export let redirectTitle;
    
</script>

<style lang="scss">
    .grid-loginForm__form{
        display:grid;
        grid-template-columns: repeat(15, 2rem);
        grid-template-rows: repeat(15, 2rem);
    }

    .redirect{
        text-align:center;
        grid-row:13/14;
        grid-column:1/16;
    }

    .redirectLink{
        text-decoration:none;
        color:$primaryColour;
    }
</style>