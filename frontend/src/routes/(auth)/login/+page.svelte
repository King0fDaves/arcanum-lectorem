<Form 
    title="Login" 
    btnTitle="Login" 
    fields={fields} 
    redirectMessage={redirectMessage} 
    redirectLink={redirectLink}
    redirectTitle={redirectTitle}    
/>

<script>
    import Form from '$lib/auth/form/+page.svelte';
    
    let fields = [
            {name:"Username", type:"text"},
            {name:'Password', type:"password"}
        ] 

    let redirectMessage = "Don't Have an Account? ";
    let redirectLink = 'sign-up';
    let redirectTitle = 'Sign Up'

    
</script>   