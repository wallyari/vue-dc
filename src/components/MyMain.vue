<template>
<main class="bg-dark">
    <!-- <div class="text-white px-3 p-5"> -->
        <!-- <h2> Content goes here</h2> -->
        <div class="hero_series">
            <img  src="../assets/img/jumbotron.jpg" alt="">
        </div>
        <div class="text-white px-5 py-5 container-fluid">
        <div class="px-5 row" >
            <comicsShop v-for="(comic, index) in comicsShopList" :key="index"
                :thumb="comic.thumb"
                :price="comic.price"
                :series="comic.series"
                :type="comic.type" />
        </div>
        <div class="text-white text-center  mt-3">
            <span class="btn-load-more px-5 py-2">LOAD MORE</span>
        </div>
    </div>
    <!-- <section>
        <div class="shopper d-flex p-5 text-white">
            <div class="pe-5">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                DIGITAL COMICS
            </div>
            <div class="pe-5">
                <img src="../assets/img/buy-comics-merchandise.png" alt="">
                DC MERCHANDISE
            </div>
            <div class="pe-5">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                COMIC SHOP LOCATOR
            </div>
            <div class="pe-5">
                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                SUBSCRIPTIONS
            </div>
            <div class="pe-5">
                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                DC POWER VISA
            </div>
        </div>
    </section> -->
</main>

</template>

<script>
import comicsShop from '../components/comicsShop.vue'

export default {
    components: {
    comicsShop,
    },
    data : function(){
        return{
            comicsShopList :[
                     {
                         "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                         "price": "$19.99",
                         "series": "Action Comics",
                         "type": "comic book"
                     },
                     {
                         "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                         "price": "$3.99",
                         "series": "American Vampire 1976",
                         "type": "comic book"
                     },
                     {
                         "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                         "price": "$16.99",
                         "series": "Aquaman",
                         "type": "graphic novel"
                     },
                     {
                         "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                         "price": "$2.99",
                         "series": "Batgirl",
                         "type": "comic book"
                     },
                     {
                         "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                         "price": "$3.99",
                         "series": "Batman",
                         "type": "comic book"
                     },
                     {
                         "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                         "price": "$2.99",
                         "series": "Batman Beyond",
                         "type": "comic book"
                     },
                     {
                         "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                         "price": "$3.99",
                         "series": "Batman/Superman",
                         "type": "comic book"
                     },
                     {
                         "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                         "price": "$4.99",
                         "series": "Batman/Superman Annual",
                         "type": "comic book"
                     },
                     {
                         "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                         "price": "$5.99",
                         "series": "Batman: The Joker War Zone",
                         "type": "comic book"
                     },
                     {
                         "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                         "price": "$6.99",
                         "series": "Batman: Three Jokers",
                         "type": "comic book"
                     },
                     {
                         "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                         "price": "$4.99",
                         "series": "Batman: White Knight Presents: Harley Quinn",
                         "type": "comic book"
                     },
                     {
                         "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                         "price": "$16.99",
                         "series": "Catwoman",
                         "type": "graphic novel"
                     }
             ]
       }
   }
 }
 </script>

<style lang="scss" scoped>
@import "../styles/variables.scss";
    .btn-load-more{
    background: $colorBrand;
    }
    
    .hero_series{
    img{
        object-fit: cover;
        object-position: top;
        height: 300px;
        width: 100%;
        }
    }
// @import "../styles/variables.scss";
// .shopper{
//     background-color: $colorBrand;
//     img{
//         width: 60px;
//         height: 60px;
//         object-fit: cover;

//     }
// }

</style> 