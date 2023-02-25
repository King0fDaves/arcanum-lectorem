<Form 
    title="Sign Up" 
    btnTitle="Sign Up" 
    fields={fields} 
    redirectMessage={redirectMessage} 
    redirectLink={redirectLink}
    redirectTitle={redirectTitle}
/>

<p> Already Have An Account? </p>

<script>
    import Form from '$lib/auth/form/+page.svelte';
    
    let redirectMessage = "Already Have an Account? ";
    let redirectLink = 'login';
    let redirectTitle = 'Login'

    let fields = [
            {name:"Create Username", type:"text"},
            {name:'Ctreate Password', type:"password"}
        ] 
</script>   

<style lang="scss"> 
    .redirect{
        color:$textColour
    }
</style>