<div class="groupChats" id="groupChats">
    <button class="closebtn" on:click={() => {closeSide()}}>&times;</button>
</div>

<script>
    function closeSide() {
        document.getElementById("groupChats").style.width = "0";
    }
</script>
<style lang="scss">

@media screen and (max-width: $tabletMaxScreenWidth){
    .groupChats {
        height: 100%; 
        width: 0; 
        position: fixed; 
        z-index: 1;
        top: 0; 
        left: 0;
        background-color: #000; 
        overflow-x: hidden; 
        transition: 0.5s; 
  }
}
  
    
</style>