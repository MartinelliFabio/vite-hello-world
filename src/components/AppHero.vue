<template>
    <div class="jumbo">
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
                
            }
        }
    }
</script>

<style lang="css">
    .jumbo {
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        height: 350px;
        text-align: center;
        background-color: blue; 
    }

</style>