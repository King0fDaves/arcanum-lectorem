<ul class="groupScrollBar__items">
  
    {#each groups as group}
      <li class="groupScrollBar__item">
        <div class="groupPic"></div>
        <p class="groupName">{group.name}</p>
      </li>
    {/each}
    <li class="groupScrollBar__item">
      <div class="extraPadding"></div>
    </li>
  </ul>

<script>
    export let groups;
</script>

<style lang="scss">
    .groupScrollBar__items {
        overflow-y: none;
        padding: 0;
        margin: 0;
        list-style: none;
        display: flex;
        flex-direction: column;
  }

  .groupScrollBar__item{
    display: flex;
    flex-direction: row;
    margin-bottom: .5rem;
  }

  .groupPic {
    margin: auto;
    border-radius: 50%;
    width: 3rem;
    height: 3rem;
    margin-right: .5rem;
    border: 0.15rem solid $primaryColour;
    
  }

  .groupName{
    display:block;
    width:70vw;
  }

  .extraadding{
    width:3rem;
    height:3rem;
  }
  
</style>

