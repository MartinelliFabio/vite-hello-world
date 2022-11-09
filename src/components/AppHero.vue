<template>
    <div v-if="selectedImage" class="jumbo" :style="{ background: 'linear-gradient(rgba(0, 0, 0, .2), rgba(0, 0, 0, .5)), url(' + selectedImage + ')', backgroundPosition: 'center', backgroundRepeat: 'no-repeat', backgroundSize: 'cover' }">
        <AppTitle/>
    </div>
</template>

<script>

import AppTitle from './AppTitle.vue';

    export default {
        name: 'AppHero',
        components: {
            AppTitle
        }, 
        data() {
            return {
                activeIndex: 0,
                image: [
                    'https://source.unsplash.com/random/',
                ],
                selectedImage: null
            }
        },
        methods: {
            randomItem (items) {
                return items[Math.floor(Math.random()*items.length)];
            },
        },
        computed() {
            
        },
        created() {
            this.selectedImage = this.randomItem(this.image)
        },
        mounted() {

        },

    }
</script>

<style lang="css">
    .jumbo {
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        height: 60vh;
        text-align: center;
        text-shadow: 2px 4px #000000;
    }

</style>