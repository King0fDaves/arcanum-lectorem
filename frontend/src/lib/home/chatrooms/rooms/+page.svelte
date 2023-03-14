<div class="roomType">
    <TopNavigation btnIcon={icon} openSideBar={openSideBar} />
    <span class="roomType__title">{title}</span>
    <RoomList />
</div>
   

<script>

    export let openSideBar;
    export let title;
    export let icon;
    import TopNavigation from "$lib/home/chatrooms/topNavigation/+page.svelte";
    import RoomList from "$lib/home/chatrooms/roomList/+page.svelte";

</script>

<style lang="scss">
    @media screen and (max-width: $mobileMaxScreenWidth){
        .roomType{
            
    
            padding: 0;
            margin: 0;
            overflow: hidden;
            height: 85vh;
            width:100vw;
            overflow: -moz-hidden-unscrollable;

            display: flex;
            display: -ms-flexbox;
            display: -webkit-flex;

            flex-direction: column;
            -ms-flex-direction: column;
        }

        .roomType__title{
            padding:0;
            margin: 0;
            align-self: center;
            font-family: "GoodTimes";
            color:$primaryColour;
        }
    }

</style>