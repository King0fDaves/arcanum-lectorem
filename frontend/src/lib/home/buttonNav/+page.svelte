<a href="#room" on:click={scrollIntoView}>Click me</a>

<script>
    function scrollIntoView({ target }) {
		const element = document.querySelector(target.getAttribute('href'));
        console.log(target) 
		if (!element) return;
        element.scrollIntoView()
    };
</script>

<style lang="scss">
    a{
        width:4rem;
        height: 4rem;
        background-color: orange;
    }
</style>