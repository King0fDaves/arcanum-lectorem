<nav class="mainNavbar">
    <ul class="navbar">
      <li class="navbarItem">
        <a href="#" class="routes"><i class="icon fa-solid fa-house"></i></a> 
      </li>
      <li class="navbarItem">
        <a href="#" class="routes"> <i class="icon fa-solid fa-envelope"></i></a>
      </li>
    
      <li class="navbarItem">
        <a href="#" class="routes"><i class="icon plus fa-thin fa-plus"></i></a>
      </li>

      <li class="navbarItem">
        <a href="#" class="routes"><i class="icon fa-solid fa-gear"></i></a>
      </li>

      <li class="navbarItem">
        <a href="#" class="routes"><i class="icon fa-solid fa-right-from-bracket"></i></a>
      </li>
      
    </ul>
  </nav>
  
  <style lang="scss">
    @media screen and (max-width: $mobileMaxScreenWidth){
        
  
        .mainNavbar {
          overflow-y: hidden;
          padding: 0;
          margin: 0;
          justify-self: flex-end;
          
          display: flex;
          display: -ms-flexbox;
          display: -webkit-flex;

          margin-top: auto;
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
        align-items: center;
        width:100vw;
        height:4rem;
        background-color: black;
        border-radius: 2rem;

        align-self: center;
        
      }
  
      .routes{
  
        padding: 0%;
        text-decoration: none;
        color: #fff;
        text-align: center;
      }
  
      .icon{
        font-size: 1.5rem;
      }

      .plus{
        font-size: 2.5rem;
      }
  
      .selected{
          color:#fff;
          border-radius: 50%;
          background-color: $primaryColour;
          padding: .75rem;
      }
    }
  </style>
  