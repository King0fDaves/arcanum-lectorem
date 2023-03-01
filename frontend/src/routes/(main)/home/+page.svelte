<svelte:head>
	<link rel="stylesheet" href="src/styles/layouts/_home.scss" />
</svelte:head>
<section id="chatrooms" class="chatroomsSection">
    <SearchBar />
    <SettingsNav />
    <FriendBar />
    <GroupBar />
    <RoomGroupButton />
</section>

<section id="room" class="roomSection">
    <RoomsHeader />
    <Messages />
    <MessageInputBox />
</section>

<section id="info" class="infoSection">

</section>

<script>
    //chatrooms
    import SearchBar from '$lib/home/chatrooms/searchBar/+page.svelte';
    import SettingsNav from '$lib/home/chatrooms/settingsNav/+page.svelte';
    import FriendBar from '$lib/home/chatrooms/friendBar/+page.svelte';
    import GroupBar from '$lib/home/chatrooms/groupBar/+page.svelte';
    import RoomGroupButton from '$lib/home/chatrooms/roomGroupButton/+page.svelte';


    //rooms
    import RoomsHeader from '$lib/home/room/roomsHeader/+page.svelte';
    import MessageInputBox from '$lib/home/room/messageInputBox/+page.svelte';
    import Messages from '$lib/home/room/messages/+page.svelte';

</script>

<style lang="scss">
    section{
        padding: 0%;
        overflow-y: hidden;
    }
</style>