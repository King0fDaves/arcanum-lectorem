<div class="grid-roomHeader">
    <ChatroomsNav />
    <RoomInfo />
</div>

<script>
    import ChatroomsNav from '$lib/home/room/roomsHeader/chatroomsNav/+page.svelte';
    import RoomInfo from '$lib/home/room/roomsHeader/roomInfo/+page.svelte';

</script>

<style lang="scss">
    @media screen and (max-width: $mobileMaxScreenWidth){
    .grid-roomHeader{
        grid-column: 1/21;
        grid-row:1/5;
        display: grid;
        background-color: $grey;
        grid-template-columns: repeat(20, 1fr);
        grid-template-rows: repeat(5,1fr);
    }
    }
</style>