<svelte:head>
	<link rel="stylesheet" href="src/styles/layouts/_home.scss" />
</svelte:head>
<section class="chatroomsSection">
    <SearchBar />
    <SettingsNav />
    <FriendBar />
    <GroupBar />
</section>

<section class="roomSection">

</section>

<section id="info" class="infoSection">

</section>

<script>
    import SearchBar from '$lib/home/chatrooms/searchBar/+page.svelte';
    import SettingsNav from '$lib/home/chatrooms/settingsNav/+page.svelte';
    import FriendBar from '$lib/home/chatrooms/friendBar/+page.svelte';
    import GroupBar from '$lib/home/chatrooms/groupBar/+page.svelte';
</script>

<style lang="scss">
    .chatroomSection{
        overflow-y: hidden;
    }
</style>