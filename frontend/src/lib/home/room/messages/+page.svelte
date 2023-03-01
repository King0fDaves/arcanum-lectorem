

<ul class="chatlog">

    {#each messages as message}

        <Message username={message.username} date={message.date} text={message.text}/>
    {/each}
  
</ul>

<script>
   import Message from "$lib/home/room/messages/message/+page.svelte";
  let messages = [
    {username: 'KingOfDaves', date:'27/02/2023', text:'What is up my G'},
    {username: 'ShutUp', date:'28/9/2023', text:"Sorry I didn't get your message for 7 months"},
    {username:'KingOfDaves', date:'28/9/2023', text:'Its all good'},

  ]
</script>

<style lang="scss">
  @media screen and (max-width: $mobileMaxScreenWidth) {
    .chatlog {
      overflow-y: scroll;
      padding: 0;
      grid-row: 4/37;
      grid-column: 1/21;
      list-style: none;
    }
  }
</style>
