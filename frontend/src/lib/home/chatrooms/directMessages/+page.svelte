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
            width:100vw;
			height:100vh;
            display: flex;
            display: -ms-flexbox;
            display: -webkit-flex;
            flex-direction: row;
            flex-wrap: wrap;
            background-color: $backgroundColour;
            align-items: center;
			justify-content: center;

        }

        .friendsTitle{
            align-self: center;
            font-family: "GoodTimes";
            color:$primaryColour;
            margin-top:2rem;
            grid-row: 4/5;
            grid-column: 10/12;
        }

      
    }
    
</style>