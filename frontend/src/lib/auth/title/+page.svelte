<div class="grid-loginForm__title">
    <h2 class="loginForm__title">{title}</h2>
</div>
<script>
    export let title;
</script>

<style lang="scss">

.grid-loginForm__title{
    grid-column:3/14;
}

.loginForm__title{
    display:flex;
    display: -ms-flexbox;
    display: -webkit-flex;
        
    flex-direction:column;
    justify-content: center;
    align-items: center;
    color:$primaryColour;
    text-align: center;
    font-size:2.25rem;
    letter-spacing:1rem;
    font-family:'GoodTimes'

}

</style>