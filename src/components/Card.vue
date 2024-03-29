<template>
    <div class="card-service">
        <img :src="getImagePath(`../assets/${immagine}`)" alt="immagine prodotto">
        <div class="container">
            <h4>{{ title }}</h4>
            <hr>
            <p>{{ subtitle }}</p>
        </div>
    </div>
</template>


<script>
export default {
    name: `Card`,
    props: {
        immagine: String,
        title: String,
        subtitle: String

    },
    data() {
        return {
            imageName: 'immagine'
        };
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    }


}
</script>


<style lang="scss">
@use '../styles/general.scss' as *;
@use "../styles/partials/mixins.scss" as *;
@use "../styles/partials/variables" as *;

.card-service {
    transition: 0.3s;
    width: calc(100% / 4);
    border: 1px solid white;

    .container {
        padding: 4rem 1rem;

        p {
            width: 70%;
            color: $grey-color;
        }

        h4,
        hr {
            color: $icon-color;
        }

    }


    img {
        width: 100%;
        height: 90%;
    }
}
</style>