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

        
    ]
</script>

<style lang="scss">
    .grid-groupScrollBar{
            overflow-y: scroll;

        grid-column: 2/20;
        grid-row: 13/40;
        display: grid;

        grid-template-columns: repeat(10, 1fr);
        grid-template-rows: repeat(10, 1fr);
    }

    .groupScrollBar__title{
        padding: 0;
    
        color:$primaryColour;
        font-size: 1.1rem;
    }
</style>