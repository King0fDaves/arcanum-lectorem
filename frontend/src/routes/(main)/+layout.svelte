<svelte:head>
	<link rel="stylesheet" href="src/styles/layouts/_mainLayout.scss" />
</svelte:head>



<section class="mainPage">
  <slot />
</section>

<MainNavigation />

<script>
  import MainNavigation from "$lib/main/mainNavigation/+page.svelte";  
  import Chatrooms from "$lib/home/chatrooms/+page.svelte";  

</script>

<style lang="scss">
@media screen and (max-width: $tabletMaxScreenWidth){

  .mainPage {
    overflow-y: hidden;
    padding: 0;
    margin: 0;
  
    grid-column: 1/26;
    grid-row: 1/23;

  }
  
  .mainNavbar {
    overflow-y: hidden;
    padding: 0;
    margin: 0;
    background-color: $darkGrey;
    grid-row: 23/26;
    grid-column: 1/26;
}


}


</style>