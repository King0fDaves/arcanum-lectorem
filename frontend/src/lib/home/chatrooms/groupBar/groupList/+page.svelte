<ul class="groupScrollBar__items">
  
    {#each groups as group}
      <a href="#room" on:click={scrollIntoView} class="groupScrollBar__item">
        <div class="groupPic"></div>
        <p class="groupName">{group.name}</p>
      </a>
    {/each}
    <li class="groupScrollBar__item">
      <div class="extraPadding"></div>
    </li>
  </ul>

<script>
    export let groups;

    function scrollIntoView({ target }) {
		const element = document.querySelector(target.getAttribute('href'));
        console.log(target) 
		if (!element) return;
        element.scrollIntoView()
    };
</script>

<style lang="scss">
    @media screen and (max-width: $mobileMaxScreenWidth){

    .groupScrollBar__items {
        overflow-y: scroll;
        padding: 0;
        margin: 0;
        list-style: none;
        display: flex;
        flex-direction: column;
        padding-bottom: 1rem;
  }

  .groupScrollBar__item{
    display: flex;
    flex-direction: row;
    margin-bottom: .5rem;
    background-color: $backgroundColour;
    border: none;
    outline: none;

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
    
    width:70vw;
    color:$textColour;
  }
  .extraadding{
    width:3rem;
    height:3rem;
  }
}
</style>

