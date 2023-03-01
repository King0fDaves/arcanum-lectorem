<div class="grid-groupScrollBar">
    <div class="groupScrollBar">
        <p class="groupScrollBar__title">Groups<p/>
        
        <GroupList groups={groups}/>

    </div>
    
</div>

<script>
    import GroupList from "$lib/home/chatrooms/groupBar/groupList/+page.svelte"

    let groups = [
        {name:'Rick Rollers'},
        {name:'Rick Rollers'},
        {name:'Rick Rollers'},
        {name:'Rick Rollers'},
        {name:'Rick Rollers'},
        {name:'Rick Rollers'},
        {name:'Rick Rollers'},
        {name:'Rick Rollers'},
        {name:'Rick Rollers'},
        {name:'Rick Rollers'},
        

        
    ]
</script>

<style lang="scss">
    @media screen and (max-width: $mobileMaxScreenWidth){

    .grid-groupScrollBar{
        overflow-y: scroll;
        padding:0;
        grid-column: 2/20;
        grid-row: 13/39;
        display: grid;

        grid-template-columns: repeat(10, 1fr);
        grid-template-rows: repeat(10, 1fr);
    }

    .groupScrollBar__title{
        padding: 0;
        position: sticky;    
        color:$primaryColour;
        font-size: 1.1rem;
    }
    }
</style>