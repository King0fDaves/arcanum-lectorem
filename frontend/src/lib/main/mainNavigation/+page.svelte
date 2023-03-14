<nav class="mainNavbar">
  <ul class="navbar">
    <li class="navbarItem">
      <a href="/home" class="routes"><i class="icon fa-solid fa-house" /></a>
    </li>
    <li class="navbarItem">
      <a href="/invites" class="routes">
        <i class="icon fa-solid fa-envelope" /></a
      >
    </li>

    <li class="navbarItem">
      <a href="/room-options" class="routes"
        ><i class="icon plus fa-thin fa-plus" /></a
      >
    </li>

    <li class="navbarItem">
      <a href="/settings" class="routes"><i class="icon fa-solid fa-gear" /></a>
    </li>

    <li class="navbarItem">
      <a href="/login" class="routes"
        ><i class="icon fa-solid fa-right-from-bracket" /></a
      >
    </li>
  </ul>
</nav>

<style lang="scss">
  @media screen and (max-width: $mobileMaxScreenWidth) {
    .mainNavbar {
      grid-row: 23/26;
      grid-column: 1/26;
      overflow-y: hidden;
      overflow: -moz-hidden-unscrollable;
      padding: 0;
      margin: 0;
      justify-self: flex-end;

      display: flex;
      display: -ms-flexbox;
      display: -webkit-flex;

      margin-top: auto;
    }

    .navbar {
      display: flex;
      display: -ms-flexbox;
      display: -webkit-flex;
      padding: 0%;
      list-style: none;
      flex-direction: row;
      -ms-flex-direction: row;
      justify-content: space-around;
      align-items: center;
      width: 100vw;
      height: 4rem;
      background-color: black;
      border-radius: 2rem;

      align-self: center;
    }

    .routes {
      padding: 0%;
      text-decoration: none;
      color: #fff;
      text-align: center;
    }

    .icon {
      font-size: 1.5rem;
    }

    .plus {
      font-size: 2.5rem;
    }

    .selected {
      color: #fff;
      border-radius: 50%;
      background-color: $primaryColour;
      padding: 0.75rem;
    }
  }
</style>
