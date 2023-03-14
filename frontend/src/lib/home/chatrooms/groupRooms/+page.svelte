<div class="groupChats" id="groupChats">
  <Rooms openSideBar={openSide} title="Groups" icon="fa-solid fa-x"/>
</div>

<script>
  let openSide = false;
  import Rooms from "$lib/home/chatrooms/rooms/+page.svelte";

</script>

<style lang="scss">
  @media screen and (max-width: $mobileMaxScreenWidth) {
    .groupChats {
     
    
      height: 83vh;
    
      width: 0;
      position: fixed;
      z-index: 1;
    
      background-color: #000;
      overflow-x: hidden;
      transition: 0.5s;

    }

    .topNavbar{
      display: flex;
      display: -ms-flexbox;
      display: -webkit-flex;
      flex-direction: row;
      align-items: center;
      justify-content: space-between;
      margin-top:-75vh;

      margin-bottom: 3rem;
      width:80vw;
    
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
