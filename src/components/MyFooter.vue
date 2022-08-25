<template>
<footer class="">
    <div class="row p-3 footer-top">
        <div class="col-2">
        <h3 class="text-white">Dc comics</h3>
        <ul>
            <li>text</li>
            <li>text</li>
            <li>text</li>
            <li>text</li>
        </ul>
            <h3 class="text-white">Dc comics</h3>
        <ul>
            <li>text</li>
            <li>text</li>
            <li>text</li>
            <li>text</li>
        </ul>
    </div>
    <div class="col-2">
            <h3 class="text-white">Dc comics</h3>
        <ul>
            <li>text</li>
            <li>text</li>
            <li>text</li>
            <li>text</li>
        </ul>
    </div>
    <div class="col-2">
            <h3 class="text-white">Dc comics</h3>
        <ul>
            <li>text</li>
            <li>text</li>
            <li>text</li>
            <li>text</li>
        </ul>
    </div>
    <div class="col-6">
        <img class="logo-bg-breand" src="../assets/img/dc-logo-bg.png" alt="">
    </div>
    </div>
    <div class="footer-bottom p-4 d-flex justify-content-between align-items-center">
        <div class="follow">
            <a class="text-white button-footer p-2" href="#">SING-UP NOW!</a>
        </div>
        <div>
            <a class="me-3" href="#">FOLLOW US</a>
            <a class="me-3" href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>
            <a class="me-3" href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>
            <a class="me-3" href="#"><img src="../assets/img/footer-youtube.png" alt=""></a>
            <a class="me-3" href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
            <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>
        </div>
    </div>
</footer>


</template>

<script>
export default {
 //   data : function(){
 //     return {
 //       comicsLink : [
 //             {
 //                 text : 'characters' ,
 //                 href : '#'
 //             },
 //             {
 //                 text : 'comics' ,
 //                 href : '#'
 //             },
 //             {
 //                 text : 'movies' ,
 //                 href : '#'
 //             },
 //             {
 //                 text : 'tv' ,
 //                 href : '#'
 //             },
 //             {
 //                 text : 'games' ,
 //                 href : '#'
 //             },
 //             {
 //                 text : 'collectibles' ,
 //                 href : '#'
 //             },
 //             {
 //                 text : 'videos' ,
 //                 href : '#'
 //             },
 //             {
 //                 text : 'fans' ,
 //                 href : '#'

 //             },
 //             {
 //                 text : 'news' ,
 //                 href : '#'
 //             },
 //         ],
 //         shopLink : [
 //             {
 //                 text : 'shop DC' ,
 //                 href : '#'
 //             },
 //             {
 //                 text : 'shop DC collectibles' ,
 //                 href : '#'
 //             },
 //         ],
 //     }
 }
</script>

<style lang="scss" scoped>
@import "../styles/variables.scss";
footer{
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: repeat-x;
}
.footer-top{
    height: 480px;
}
li{
    list-style: none;
    }
a{
    text-decoration: none;
}
.logo-bg-breand{
    overflow: hidden;
}
.footer-bottom{
    height: 100px;
    background-color: rgb(46, 46, 46);
}
.button-footer{
    border: 2px solid  $colorBrand ;
}
.follow a{
    color: $colorBrand;
}

</style> 