<div class="grid-rooms {isFriendRoute ? ["friendDMs"]:['']}">
    <span class="roomTitle">{title}</span>

    <ul class="rooms">
        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>
        
        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>

        <li class="rooms__item">
            <a class="roomRedirect" href="#">
                <div class="roomRedirect__img"></div>
                <span class="roomRedirect__roomName">Rick Rollers</span>
            </a>
        </li>
        
        
    </ul>
    <!--
        {#each cats as cat}

        {/each}
    -->

    
</div>  

<script>
    export let title;
    export let isFriendRoute = false;
</script>

<style lang="scss">
    @media screen and (max-width: $mobileMaxScreenWidth){
        .grid-rooms{
            grid-column: 2/25;
            grid-row: 6/26;
            display: flex;
            display:-ms-flexbox;
            display: -webkit-flex;

            flex-direction: column;
            padding: 0;
            align-items: center;
            justify-content: center;

            max-height: 65vh;
      
        }
        
        .roomTitle{
            color:$primaryColour;
            font-family: 'GoodTimes';
            
        }

        .rooms{
            overflow-y: scroll;
            display: flex;
            display: -webkit-flex;
            display: -ms-flexbox;
            flex-direction: column;
            list-style: none;
            padding:0;
            margin-top:1.5rem;
        }

        .rooms__item{
            padding: 0;
            margin-bottom: .5rem;
        }

        .roomRedirect{
            display: -ms-flexbox;
            display: flex;
            display: -webkit-flex;
            flex-direction: row;
            flex-wrap: wrap;
            text-decoration: none;
            color:$primaryColour;
            font-family: "GoodTimes";
            font-size: .9rem;
            height: 3.5rem;
            width:80vw;
            border-radius: 2rem;
            background-color: $grey
        }

        .roomRedirect__img{
            width:2.5rem;
            height:2.5rem;
            border: solid .1rem $primaryColour;
            border-radius: 50%;
            align-self: center;
            margin-left: 1rem;
        }
        .roomRedirect__roomName{
            align-self: center;
            margin-left: 1rem;
        }

        .friendDMs{
        
        }
    }
</style>
