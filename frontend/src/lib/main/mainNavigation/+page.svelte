<nav class="mainNavbar">
    <ul class="navbar">
      <li class="navbarItem">
        <a href="#" class="routes"><i class="icon selected fa-solid fa-house"></i></a> 
      </li>
      <li class="navbarItem">
        <a href="#" class="routes"> <i class="icon fa-solid fa-inbox"></i></a>
      </li>
      <li class="navbarItem">
        <a href="#" class="routes"><i class="icon fa-solid fa-music"></i></a>
      </li>

      <li class="navbarItem">
        <a href="#" class="routes"><i class="icon fa-solid fa-gear"></i></a>
      </li>
    </ul>
  </nav>
  
  <style lang="scss">
    @media screen and (max-width: $tabletMaxScreenWidth){
        .mainPage{
          overflow-y: hidden;
          padding: 0;
          margin: 0;
          grid-column: 1/26;
          grid-row: 1/23;
  
        }
  
        .mainNavbar {
          overflow-y: hidden;
          padding: 0;
          margin: 0;
          background-color: $grey;
          grid-row: 23/26;
          grid-column: 1/26;
      }
  
      .navbar{
        display: flex;
        display: -ms-flexbox;
        display: -webkit-flex;
        padding:0%;
        list-style: none;
        flex-direction: row;
        -ms-flex-direction: row;
        justify-content: space-around;
      }
  
      .routes{
  
        padding: 0%;
        text-decoration: none;
        color: #fff;
      }
  
      .icon{
        font-size: 2rem;
      }
  
      .selected{
          color:$primaryColour;
      }
    }
  </style>
  