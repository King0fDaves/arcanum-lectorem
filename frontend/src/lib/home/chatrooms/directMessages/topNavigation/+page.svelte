<div class="topNavbar">

  <div class="friendSearchbar">
    <SearchBar />
  </div>

  <button class="groupBtn" on:click={() => openGroupChat()}>
    <i class="fa-solid fa-users-line" />
  </button>

</div>

<script>

  import SearchBar from "$lib/home/searchBar/+page.svelte";

  function openGroupChat() {
    document.getElementById("groupChats").style.width = "100vw";
  }
</script>

<style lang="scss" scoped>
  @media screen and (max-width: $mobileMaxScreenWidth) {
    .topNavbar {
      margin-top: auto;      
      display: flex;
      display: -ms-flexbox;
      display: -webkit-flex;
      flex-direction: row;
      align-items: center;
      justify-content: space-between;
      margin-top: -5rem;
      width: 90vw;
  
    }

    .groupBtn{
      height:3rem;
      width:3rem;
      border-radius: 50%;
      background:none;
      outline:none;
      font-size: 1.1rem;
      border:solid .15rem $primaryColour;
      color:#fff;
      margin-right: 1.5rem;     

    }

    .friendSearchbar{
      margin-left: 2rem;
    }
  
  }
</style>
