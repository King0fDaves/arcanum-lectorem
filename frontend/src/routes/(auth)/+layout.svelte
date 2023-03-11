<svelte:head>
	<link rel="stylesheet" href="src/styles/layouts/_auth.scss" />
</svelte:head>


<section class="headerSection">
    <header>
        <h1 class="header__title">
            <i class="fa-regular fa-eye"></i>
            Arcanum Lectorem 
        </h1>
    </header>
</section>

<section class="mainSection">
    <div class="loginForm">
        <slot />
    </div>
</section>

<section class="footerSection">
    <footer >
        <p class="footer__paragraph">Copyright &#169; David Gosoe All Rights Reserved</p> 
    </footer>
</section>


<style lang="scss">
    .header__title{
        font-family: 'GoodTimes';
        color:$primaryColour;
        text-align:center;
        font-size:2rem;
    }

    .footer__paragraph{
        text-align:center;
    }

    .loginForm{
        
        margin:auto;
        display: flex;
        display: -ms-flexbox;
        display: -webkit-flex;
        justify-content: center;
        align-items: center;
        width:30rem;
        height:28rem;
        background-color:$darkGrey;

        @include sharpBorderCorners(3rem);

        @media screen and (max-width: $mobileMaxScreenWidth){
            background:none
        }
    }

</style>