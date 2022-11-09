<template>
    <div class="title">
        <h1>{{titolo}}</h1>
    </div>
</template>

<script>
    export default {
        name: 'AppTitle',
        data() {
            return {
                titolo: 'La mia prima app con Vite!'
            }
        }
    }
</script>

<style lang="css">
    .title {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 150px;
    }

    h1 {
        color: white;
        font-weight: bold;
    }

</style>