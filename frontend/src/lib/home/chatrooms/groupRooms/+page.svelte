<div class="groupChats" id="groupChats">

  <div class="topNavbar">
    <SearchBar />
    
    <div class="closebtn" on:click={() => {closeSide();}}>
      <i class="closeIcon fa-solid fa-xmark"></i>
    </div>
    
  </div>
 
  <RoomList title="Groups" />
</div>

<script>
  import SearchBar from "$lib/home/searchBar/+page.svelte";
  
  import RoomList from "$lib/home/chatrooms/roomList/+page.svelte";
  function closeSide() {
    document.getElementById("groupChats").style.width = "0";
  }

</script>

<style lang="scss">
  @media screen and (max-width: $mobileMaxScreenWidth) {
    .groupChats {
      display: grid;
      display: -ms-grid;
      display: -moz-grid;

      height: 100%;
      width: 0;
      position: fixed;
      z-index: 1;
      top: 0;
      left: 0;
      background-color: #000;
      overflow-x: hidden;
      transition: 0.5s;

      grid-template-columns: repeat(25, 1fr);
      grid-template-rows: repeat(25, 1fr);
      grid-column: repeat(25, 1fr);
      grid-row: repeat(25, 1fr);
    }

    .topNavbar{
      grid-column: 2/25;
      grid-row: 2/4;
      display: flex;
      display: -webkit-flex;
      display: -ms-flexbox;
      flex-direction: row;
      padding:0;
      margin:0;
      align-items: center;
      justify-content: space-evenly;
    }
    .closebtn{
      text-align: center;
      color:$primaryColour;
      padding: 0;
      width:2rem;
      height: 2rem;
      font-size: 1rem;
      margin: 0;
      border: .15rem solid $primaryColour;
      border-radius: 50%;
    }
    .closeIcon{
      margin-top:25%;
    }
    
    

  }
</style>
