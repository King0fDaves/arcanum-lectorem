<div class="backArrow">
    <a class="arrow" href="#chatrooms" on:click={scrollIntoView}><i class=" fa-sharp fa-solid fa-arrow-left"></i></a>
</div>


<script>
    function scrollIntoView({ target }) {
		const element = document.querySelector(target.getAttribute('href'));
        console.log(target) 
		if (!element) return;
        element.scrollIntoView()
    };
</script>

<style lang="scss">
    @media screen and (max-width: $mobileMaxScreenWidth){
    .backArrow{
        grid-column: 2/4;
        grid-row:3/4;
    }
    .arrow{
        text-decoration: none;
        color:$primaryColour;
        font-size: 1.75rem;
    }
    }
</style>