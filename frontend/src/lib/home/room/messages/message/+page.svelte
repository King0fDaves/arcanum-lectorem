<li class="chatlog__item">
  <div class="topComponents">
    <div class="profilePic"></div> 
    <div class="messageInfo">
      <span class="username">{username}</span>
      <span class="time">{date}</span>
    </div>
    
  </div>

  <div class="textDirection">
    <p class="text">{text}</p>
  </div>
</li>

<script>
  export let username;
  export let date;
  export let text;
</script>

<style lang="scss">
    @media screen and (max-width: $mobileMaxScreenWidth) {
  .chatlog__item {
    display: block;    
    height: auto;
  
    

    min-height: 5rem;
  }
  .topComponents {
    margin-top: .5rem;
    display: grid;
    grid-template-columns: repeat(20, 1fr);
  }
  .textDirection {
    display: block;
    margin-left: .8rem;
  }
  .profilePic {
    grid-column: 2/3;
    border-radius: 50%;
    width: 3rem;
    height: 3rem;
    border: 0.15rem solid $primaryColour;
  }
  .messageInfo{
    grid-column: 4/5;
  }
  .text{
    font-size: .8rem;
  }
}
</style>
