<template>
<footer class="">
    <div class="row pt-3 px-3 footer-top">
        <div class="col-2">
        <h5 class="text-white">DC COMICS</h5>
        <ul class="p-0">
            <li v-for="(link , index) in comicsLink" :key="index">
                <a class="text-muted" :href="link.href">{{ link.text }}</a>
            </li>
        </ul>
            <h5 class="text-white">SHOP</h5>
        <ul class="p-0">
            <li v-for="(link , index) in shopLink" :key="index">
                <a class="text-muted" :href="link.href">{{ link.text }}</a>
            </li>
        </ul>
    </div>
    <div class="col-2">
            <h5 class="text-white">DC</h5>
        <ul class="p-0">
            <li v-for="(link , index) in shopLink" :key="index">
                <a class="text-muted" :href="link.href">{{ link.text }}</a>
            </li>
        </ul>
    </div>
    <div class="col-2">
            <h5 class="text-white">SITES</h5>
        <ul class="p-0">
            <li v-for="(link , index) in shopLink" :key="index">
                <a class="text-muted" :href="link.href">{{ link.text }}</a>
            </li>
        </ul>
    </div>
    <div class="col-6">
        <img class="logo-bg-brand">
    </div>
    </div>
    <div class="footer-bottom p-4 d-flex justify-content-between align-items-center">
        <div class="follow">
            <a class="text-white button-footer p-3" href="#">SING-UP NOW!</a>
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
    data : function(){
    return {
        comicsLink : [
            {
                text : 'Characters' ,
                href : '#'
            },
            {
                text : 'Comics' ,
                href : '#'
            },
            {
                text : 'Movies' ,
                href : '#'
            },
            {
                text : 'Tv' ,
                href : '#'
            },
            {
                text : 'Games' ,
                href : '#'
            },
            {
                text : 'Collectibles' ,
                href : '#'
            },
            {
                text : 'Videos' ,
                href : '#'
            },
            {
                text : 'Fans' ,
                href : '#'

            },
            {
                text : 'News' ,
                href : '#'
            },
        ],
            shopLink : [
                {
                    text : 'Shop DC' ,
                    href : '#'
                },
                {
                    text : 'Shop DC collectibles' ,
                    href : '#'
                },
            ],
            dcLink : [
            {
                    text: "Terms Of Use",
                    href: "#",
                },
                {
                    text: "Privacy policy (New)",
                    href: "#",
                },
                {
                    text: "Ad Choices",
                    href: "#",
                },
                {
                    text: "Advertising",
                    href: "#",
                },
                {
                    text: "Jobs",
                    href: "#",
                },
                {
                    text: "Subscriptions",
                    href: "#",
                },
                {
                    text: "Talent Workshops",
                    href: "#",
                },
                {
                    text: "CPSC Certificates",
                    href: "#",
                },
                {
                    text: "Ratings",
                    href: "#",
                },
                {
                    text: "Shop Help",
                    href: "#",
                },
                {
                    text: "Contact Us",
                    href: "#",
                },
        ],
sitesLink: [
                {
                    text: "DC",
                    href: "#",
                },
                {
                    text: "MAD Magazine",
                    href: "#",
                },
                {
                    text: "DC Kids",
                    href: "#",
                },
                {
                    text: "DC Universe",
                    href: "#",
                },
                {
                    text: "DC Power Visa",
                    href: "#",
                },
            ]
    }
    }
}
</script>

<style lang="scss" scoped>
@import "../styles/variables.scss";
footer{
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: repeat-x;
}
// .footer-top{
//     height: 480px;
// }
li{
    list-style: none;
    }
a{
    text-decoration: none;
}
.logo-bg-brand{
    overflow: hidden;
    background-image:   url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
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