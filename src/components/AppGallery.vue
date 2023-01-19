<script>
export default {
    name: 'Gallery',
    data() {
        return {
            images: ['antonio_1.svg', 'mario_1.jpg']
        }
    },
    methods: {
        buildImage(image) {
            const url = new URL(`../assets/img/${image}`, import.meta.url);
            return url.href;
        }
    }
}

</script>


<template>
    <ul>
        <li v-for="image in images">
        <img :src="buildImage(image)" alt="">
        </li>
    </ul>
    
</template>

<style scoped>
ul{
    display: flex;
    list-style: none;
    justify-content: center;
}
img{
    width: 100%;
    height: 250px;
}     
</style>