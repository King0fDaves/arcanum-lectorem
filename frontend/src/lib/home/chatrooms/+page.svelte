<button class="btn" on:click={() => openGroupChat()}>Open Group Chat</button>
  <Group />
<script>
  import Group from "$lib/home/chatrooms/group/+page.svelte";

  function openGroupChat() {  
    document.getElementById("groupChats").style.width = "80vw";
  }
</script>

<style lang="scss">
  .btn {
    top: 0;
    position: fixed;
  }
</style>
