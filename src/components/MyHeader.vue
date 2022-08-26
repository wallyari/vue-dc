<template>
<header class="container-fluid">
    <div class="d-flex py-3 px-5 justify-content-between">
        <div>
            <img class="logoBrand" src="../assets/img/dc-logo.png" alt="main-logo-dc">
        </div>  
        <nav>
            <ul class="d-flex justify-content-around text-uppercase">
                <li class="m-2" v-for="(link , index) in navLinks" :key="index">
                        <a :class="{active : link.active}" class="fw-bolder" :href="link.href" >{{ link.text }}</a>
                </li>
            </ul>
        </nav>
    </div> 
</header>

</template>

<script>
export default {   
    data : function(){
    return {
    navLinks : [
        {
            text : 'characters' ,
            href : '#',
            active : false
        },
        {
                text : 'comics' ,
                href : '#',
                active : true
            },
            {
                text : 'movies' ,
                href : '#',
                active : false
            },
            {
                text : 'tv' ,
                href : '#',
                active : false
            },
            {
                text : 'games' ,
                href : '#',
                active : false
            },
            {
                text : 'collectibles' ,
                href : '#',
                active : false
            },
            {
                text : 'videos' ,
                href : '#',
                active : false
            },
            {
                text : 'fans' ,
                href : '#',
                active : false
            },
            {
                text : 'news' ,
                href : '#',
                active : false
            },
            {
                text : 'shop' ,
                href : '#',
                active : false
            },

        ],
    }
}
}

</script>

<style lang="scss" scoped>
@import '../styles/variables.scss';

header{
    height: 100px;
    border: 1px solid blue;
    background-color:white;
}
.logoBrand{
    width: 5%;
    min-width: 70px;
    min-height: 70px;
}
nav{
    li{
        list-style: none;
        
        a{
            text-decoration: none;
            color: $colorTextNav;
            font-size: 0.7rem;
            padding: 40px 0;
        }


    }
}
.active{
    color: $colorBrand;
    border-bottom: 2px solid $colorBrand ;
}

</style> 