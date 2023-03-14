<div class="grid-groups">

    <ul class="groups">
        <li class="groups__item">
            <a class="groupRedirect" href="#">
                <div class="groupRedirect__img"></div>
                <span class="groupRedirect__groupName">Rick Rollers</span>
            </a>
        </li>
        
    </ul>
    <!--
        {#each cats as cat}

        {/each}
    -->

    
</div>  
<script>
    
</script>
<style lang="scss">
    @media screen and (max-width: $mobileMaxScreenWidth){
        .grid-groups{
            background-color: #000;
            grid-column: 2/25;
            grid-row: 6/25;
            display: flex;
            display: -ms-flexbox;
            display:  -webkit-flex;
            align-items: center;
            flex-direction: column;
        }
        
        .groupTitle{
            color:$primaryColour;
            font-family: 'GoodTimes';

        }

        .groups{
            overflow-y: scroll;
            display: flex;
            display: -webkit-flex;
            display: -ms-flexbox;
            flex-direction: column;
            list-style: none;
            padding:0;
            margin-top:1.5rem;
        }

        .groups__item{
            padding: 0;
            margin: 0;
        }

        .groupRedirect{
            display: -ms-flexbox;
            display: flex;
            display: -webkit-flex;
            flex-direction: row;
            text-decoration: none;
            color:$primaryColour;
            font-family: "GoodTimes";
            font-size: .9rem;
            height: 3.5rem;
            width:80vw;
            border-radius: 2rem;
            background-color: $grey;
        
        }

        .groupRedirect__img{
            width:2.5rem;
            height:2.5rem;
            border: solid .1rem $primaryColour;
            border-radius: 50%;
            align-self: center;
            margin-left: 1rem;
        }
        .groupRedirect__groupName{
            align-self: center;
            margin-left: 1rem;
        }
    }
</style>
