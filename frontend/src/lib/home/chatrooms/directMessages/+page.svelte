<div class="directMessages">
    <TopNavigation />
    <RoomList title="Friends" isFriendRoute={friendRoute} />
</div>

<script>
    import TopNavigation from "$lib/home/chatrooms/directMessages/topNavigation/+page.svelte";
    import RoomList from "$lib/home/chatrooms/roomList/+page.svelte";

    let friendRoute = true;
</script>

<style lang="scss">
    @media screen and (max-width: $mobileMaxScreenWidth){
        .directMessages{
            grid-column: 1/26;
            grid-row: 1/26;
            background-color: $backgroundColour;
            display: grid;
            display: -ms-grid;
            display: -moz-grid;

            grid-template-columns: repeat(25, 1fr);
            grid-template-rows: repeat(25, 1fr);
            
        }

        .friendsTitle{
            align-self: center;
            font-family: "GoodTimes";
            color:$primaryColour;
            margin-top:2rem;
            grid-row: 4/5;
            grid-column: 10/12;
        }

      
        .friendDMs{
            margin-top: 10rem;
        }
    }
    
</style>