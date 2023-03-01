<form class="messageInputBox" id="msgBox">
  <input contenteditable="true" class="msgBox__input" type="text" />
  <button class="msgBox__btn" form="msgBox">
    <i class="sendArrow fa-solid fa-paper-plane"></i>
  </button>
</form>

<style lang="scss">
  @media screen and (max-width: $mobileMaxScreenWidth){
  .messageInputBox {
    grid-column: 1/21;
    grid-row: 36/42;
    background-color: $grey;
    display: grid;
    grid-template-columns: repeat(100, 1fr);
    grid-template-rows: repeat(100, 1fr);
  }

  .msgBox__btn {
    grid-column: 81/99;
    grid-row: 15/90;
    border-radius: 50%;
    background: $linearGradientPrimary;
    border: .15rem $primaryColour solid ;
  
  }

  .msgBox__input {
    grid-column: 3/80;
    grid-row: 15/90;
    border-radius: 2rem;
    padding-left: 1rem;
    padding-right: 1rem;
    border: $primaryColour .15rem solid;
    background-color: $backgroundColour;
    outline: none;
    color:$textColour;
  }

  .sendArrow{
    text-align:center;
    color:#fff;
    font-size: 1.75rem;
  }
  }
</style>
