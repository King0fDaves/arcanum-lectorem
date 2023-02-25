<div class="grid-loginForm__btn">
    <input class="loginForm__btn" type="submit" value={btnTitle}/> 
</div>
<script>
    export let btnTitle;
</script>

<style lang="scss">

    .grid-loginForm__btn{
        grid-column:3/14;
        grid-row:11/12;
    }
    .loginForm__btn{
        margin:auto;
        bottom:3px;
        display: block;
        height: 3rem;
        width:15rem;
        border: none;
        outline: none;
        background: $linearGradientPrimary;
        font-size:1.5rem;
        color:$backgroundColour;
        box-shadow: .6rem 1rem #000;

        @media screen and (max-width: $mobileMaxScreenWidth){
            box-shadow:none;

            &:hover{
                background:none;
                background-color: $grey;
                color: #fff;   
            }
        }

        @media screen and (min-width: $tabletMinScreenWidth){

            &:hover{
                animation-name: buttonShadowTransitionOn;
                animation-duration: .5s;
                box-shadow: none;
                background:none;
                background-color: $grey;
                color: #fff;   
            }

            &:not(:hover){
                animation-name: buttonShadowTransitionOff;
                animation-duration: .5s;
                box-shadow: .6rem 1rem #000;
                background-color: $primaryColour;
                
            }
        }
    }
</style>