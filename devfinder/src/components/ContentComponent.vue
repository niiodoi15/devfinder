<script setup>
import NavbarComponent from './NavbarComponent.vue';


</script>

<template>
    <NavbarComponent />
    <div class="content">
        <div class="searchbar">
            <form action="" class="search" >
                <div class="input-icons">
                    <i class="fa fa-search icon"></i>
                    <input class="input-field" type="text" value="Search GitHub username…">
                </div>
                <button class="btn">Search</button>
            </form>
        </div>
        <div class="bio">    
            <div class="pic">
                <img class="profilepic" src="../assets/002-sun.svg" alt="">
            </div>
            <div class="bioname">
                <h1 class="namedetails">The Octocat</h1>
                <p class="handle">@octocat</p>
                <p class="joined">Joined 25 Jan 2011</p>
            </div>
            <div class="biodetails">
                <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Donec odio. Quisque volutpat mattis eros.</p>
            </div>
            <div class="counters">
                <div class="repos">
                    <p class="title">Repos</p>
                    <p class="count">8</p>
                </div>
                <div class="repos">
                    <p class="title">Followers</p>
                    <p class="count">8</p>
                </div>
                <div class="repos">
                    <p class="title">Following</p>
                    <p class="count">8</p>
                </div>
            </div>
            
        </div>
    </div>
</template>

<style scoped>
    .content{
        margin: 35px 0 14px 0;
        display: flex;
        flex-direction: column;
        gap: 20px;
        border-radius: 15px;
    }
    .searchbar{
        border-radius: 15px;
        padding: 0 10px;
        background: #1E2A47;
    }
    .search{
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .input-icons i {
        position: absolute;
    }
    .input-icons {
        width: 100%;
        margin-bottom: 10px;
    }
         
    .icon {
        padding: 12px;
        color: #0079FF;
        min-width: 50px;
        height: 20px;
        text-align: center;
        margin-top: 11px;
    }
    .input-field {
        width: 100%;
        margin-top: 10px;
        padding: 10px 5px 10px 40px;
        text-align: center;
        background-color: transparent;
        border: none;
        color: #FFF;
        font-size: 13px;
        font-weight: 400;
        line-height: 25px;
        text-align: start;
    }
    .btn{
        /* width: 84px; */
        padding: 13px 16px;
        border-radius: 10px;
        background: #0079FF;
        border: none;
        color: #fff;
    }
    .bio{
        display: grid !important;
        border-radius: 15px;
        background: #1E2A47;
        gap: 34px 20px;
        padding: 7% 5%;
    }
    .pic{
        grid-column: 1 / 2;
    }
    .profilepic{
        width: 70px;
        height: 70px;
    }
    .bioname{
        grid-column: 2 / 12;
    }
    .namedetails{
        color: #FFF;
        font-size: 16px;
        font-weight: 700;
    }
    .handle{
        color: #0079FF;
        font-size: 13px;
        font-weight: 400;
    }
    .joined{
        color: #FFF;
        font-size: 13px;
        font-weight: 400;
    }
    .biodetails{
        grid-column: 1 / 12;
        color: #FFF;
        font-size: 13px;
        font-weight: 400;
        line-height: 25px; /* 192.308% */
    }
    .counters{
        grid-column: 1 / 12;
        padding: 15px 32px;
        display: flex;
        justify-content: space-between;
        border-radius: 10px;
        background: #141D2F;
    }
    .repos{
        display: flex;
        flex-direction: column;
        gap: 10px;
    }
    .repos .title{
        color: #FFF;
        text-align: center;
        font-size: 11px;
        font-weight: 400;
    }
    .repos .count{
        color: #FFF;
        font-size: 16px;
        font-weight: 700;
    }

</style>