<script>
  export let friends;
</script>

<ul class="friendScrollBar__items">
  <li class="friendScrollBar__item">
    <button class="addFriend">
         <i class="plus fa-solid fa-plus" />
    </button>
    <p class="username">Add</p>
  </li>

  {#each friends as friend}
    <li class="friendScrollBar__item">
      <div class="profilePic"></div>
      <p class="username">{friend.username}</p>
    </li>
  {/each}
  <li class="friendScrollBar__item">
    <div class="extraPadding"></div>
  </li>
  
</ul>

<style lang="scss">
  .friendScrollBar__items {
    overflow-x: scroll;
    padding: 0;
    margin: 0;
    grid-column: 1/50;
    grid-row: 5/20;
    list-style: none;
    display: flex;
    flex-direction: row;

  }
  .plus{
    text-align: center;
    color:$textColour;
  }
  .addFriend {
    display: block;
    margin: auto;
    text-align: center;
    width: 3.25rem;
    height: 3.25rem;
    border-radius: 50%;
    border: 0.15rem solid $primaryColour;
    background-color: $primaryColour;
    margin-right: 0.3rem;
  }

  .friendScrollBar__item{
    display: block;
    text-align: center;
    margin-right: .3rem;
  }
  .profilePic {
    margin: auto;
    border-radius: 50%;
    width: 3rem;
    height: 3rem;
    border: 0.15rem solid $primaryColour;
    
  }

  .username {
    color: $textColour;
    font-size: 1rem;
  }

  .extraPadding{
    margin:auto;
    width:3rem;
    height: 2rem;
  }
</style>
