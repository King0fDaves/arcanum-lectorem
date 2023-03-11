<div class="grid-loginFormField">
    <div class="loginFormField">
        <label class="loginFormField__title">{fieldTitle}</label>
        <input class="loginFormField__input" type={fieldType}/>
    </div>
</div>

<script>
    export let fieldTitle;
    export let fieldType;
</script>

<style lang="scss">
    .grid-loginFormField{
    }
    .loginFormField{
        display:flex;
        display: -ms-flexbox;
        display: -webkit-flex;
        
        flex-direction:column;
        justify-content: center;
        align-items: center;
        margin-bottom:3vh;
    }

    .loginFormField__title{
        margin-bottom:3vh;
        margin-left:2rem;
        font-size: .75rem;
        font-family:'GoodTimes';
        color:$textColour;
    }

    .loginFormField__input{
        align-self: center;
        justify-content: center;
        @include inputField(15rem, 2rem, .75rem);
        @include sharpBorderCorners(1rem);

    }
    
</style>