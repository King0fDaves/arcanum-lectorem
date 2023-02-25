<div class="grid-searchbar__form">
    <form class="searchbar__form" action="">
        <input class="searchbar__input" placeholder="Search" type=text />
    </form>
</div>



<style lang="scss">
    .grid-searchbar__form{
        grid-column: 2/10;
        grid-row: 3/4;
    }

    .searchbar__input{    
        
        @include inputField(12rem, 2rem, .75rem);
        &::placeholder{
            color:$primaryColour;
            font-family: 'GoodTimes';
        }

        @include sharpBorderCorners(1rem)
    }    
</style>
