<div class="roomInfo">
    <div class="roomPic"></div>
    <div class="roomText">
        <p class="roomInfoText name">KingOfDaves</p>
        <p class="roomInfoText status">Online</p>
    </div>
</div>

<style lang="scss">
    @media screen and (max-width: $mobileMaxScreenWidth){
    .roomInfo{
        grid-column: 5/16;
        grid-row:2/5;
        display: flex;
        flex-direction: row;
    }

    .roomPic{
        border-radius: 50%;
        width: 3rem;
        height: 3rem;
        border: 0.15rem solid $primaryColour;
    }
    .roomText{
        display: block;
        float: left;
        margin-top: -.8rem;
        margin-left: .5rem;

    }
    .name{
        margin-top: 1.6rem;
        margin-bottom: .4rem;
    }
    .status{
        font-size: .75rem;
        margin-top: -.3rem;
    }
    }
</style>