<template>
    <div class="comic-container col-2">
        <img :src="thumb" :alt="series">
        <h6>{{ series }}</h6>
    </div>
</template>

<script>
export default {
    props: {
        thumb: String,
        price: String,
        series: String,
        type: String,
},
}
</script>

<style lang="scss" scoped>
.comic-container{
    img{
        width: 120px;
        height: 120px;
        object-fit: cover;
        object-position: top;
    }
}
 </style> 