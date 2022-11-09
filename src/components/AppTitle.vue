<template>
    <div class="title">
        <h1>{{titolo}}</h1>
        <p>{{subTitle}}</p>
    </div>
</template>

<script>
    export default {
        name: 'AppTitle',
        data() {
            return {
                titolo: 'La mia prima app con Vite!',
                subTitle: 'Sottotitolo del Jumbotron'
            }
        }
    }
</script>

<style lang="css">
    .title {
        color: white;
    }

    h1 {
        font-weight: bold;
        margin-bottom: 20px;
        font-size: 50px;
    }

    p {
        font-size: 20px;
        font-weight: bold;
    }

</style>