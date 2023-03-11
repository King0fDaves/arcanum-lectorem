<form class="searchbar" action="">
  <span><i class="searchbar__icon fa-sharp fa-solid fa-magnifying-glass"></i></span> <input class="searchbar__input" type="text" />
</form>

<style lang="scss">
    @media screen and (max-width: $mobileMaxScreenWidth){

    .searchbar{    
    
        @include sharpBorderCorners(1rem);
        @include inputField(9rem, 2rem, .75rem);
    
        display: flex;
        display: -ms-flexbox;
        display: -webkit-flex;
        align-items: center;
        flex-direction: row;
    }
    .searchbar__icon{
        color: $primaryColour;
    }
    .searchbar__input{
        position: fixed;
        background:none;
        border:none;
        outline: none;
        width:8rem;
        height: 2rem;
        margin-left: 1.25rem;
        color:#fff;
    }

}

</style>
