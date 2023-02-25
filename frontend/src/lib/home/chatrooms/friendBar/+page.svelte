<div class="grid-friendScrollBar">
    <div class="friendScrollBar">
        <p class="friendScrollBar__title">Friends<p/>
        
        <FriendList friends={friends}/>

    </div>
    
</div>

<script>
    import FriendList from '$lib/home/chatrooms/friendBar/friendList/+page.svelte';
    
    let friends = [
        {username:"Bob"},
        {username:'Henry'},
        {username:'KingOfDaves'},
        {username:'Shariear'},
        {username:'Josh'},
        {username:'Philip'},
        {username:'Ragavaan'}
    ]
</script>

<style lang="scss">
    @media screen and (max-width: $mobileMaxScreenWidth){
        
        
        .grid-friendScrollBar {
            padding: 0;
            margin:0;    
            grid-column: 2/21;
            grid-row: 5/11;  
        }

        .friendScrollBar{
            display: grid;
            grid-template-columns: repeat(48, .5rem);
            grid-template-rows: repeat(20, .5rem);

        }
        .friendScrollBar__title{
            padding: 0;
            margin: 0;
            grid-row: 1/2;
            color:$primaryColour;
            font-size: 1.1rem;
        }
    }

</style>
