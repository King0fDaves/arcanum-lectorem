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

			display: -moz-grid;
			display: -ms-grid;
			display: grid;

			-ms-grid-columns: repeat(25, 1fr);
			-ms-grid-rows: repeat(25, 1fr);

			grid-template-columns: repeat(25, 1fr);
			grid-template-rows: repeat(25, 1fr);

      }
	}
</style>