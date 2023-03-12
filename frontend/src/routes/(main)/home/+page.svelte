<section class="homepage">

	<Chatrooms />
	
</section>

<script>
	import Chatrooms from "$lib/home/chatrooms/+page.svelte"
</script>

<style lang="scss">
    @media screen and (max-width: $tabletMaxScreenWidth){
		.homepage{
			overflow-y: hidden;
			overflow-x: hidden;
			padding: 0;
			margin: 0;
			width:100vw;
			height:81vh;

			display: flex;
			display: -ms-flexbox;
			display: -webkit-flex;
			flex-direction: row;

			

      }
	}
</style>