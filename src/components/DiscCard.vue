<template>
    <div class="disc-container">
        <div class="img">
            <img :src="image" alt="">
        </div>
        <p>{{title}}</p> 
        <p>{{author}}</p> 
        <p>{{date}}</p> 
    </div>
</template>

<script>
export default {
    props: {
        title: String,
        image: String,
        author: String,
        date: String,
    }
}
</script>

<style lang="scss" scoped>
.disc-container{
    width: calc(100% / 5);
    padding: 25px;
    text-align: center;
    background-color: grey;
    color: white;

    img{
        width: 100%;
    }
}
</style>