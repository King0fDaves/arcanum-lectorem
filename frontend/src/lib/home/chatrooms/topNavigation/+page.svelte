<div class="topNavbar">
    <div class="searchbar">
      <SearchBar />
    </div>
    
    <button class="btn" on:click={() => openSide(openSideBar)}>
      <i class="{btnIcon}" />

    </button>
</div>

<script>
  let isFriendRoute = true;
  
  export let btnIcon;
  export let openSideBar;
  import SearchBar from "$lib/home/searchBar/+page.svelte";

  function openSide(openSide) {
    if(openSide === true){
      document.getElementById("groupChats").style.width = "100vw";
    }
    
    if(openSide === false){
      document.getElementById("groupChats").style.width = "0";
    }
  }
</script>

<style lang="scss" scoped>
  @media screen and (max-width: $mobileMaxScreenWidth) {
    .topNavbar {
      
      display: flex;
      display: -ms-flexbox;
      display: -webkit-flex;
      flex-direction: row;
      align-items: center;
    
      justify-content: space-between;
      align-items: center;

      margin-top:1rem;
      margin-bottom: 3rem;
      padding: 0;
    }

    .btn {
      height: 3rem;
      width: 3rem;
      border-radius: 50%;
      background: none;
      outline: none;
      font-size: 1.1rem;
      border: solid 0.15rem $primaryColour;
      color: #fff;
      margin-right: 1.5rem;
    }

    .searchbar{
      margin-left: 3rem;
    }
  }
</style>
