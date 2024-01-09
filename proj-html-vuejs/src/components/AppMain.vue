<template>
    <section class="experiences">
        <h1>Luxury Spa Experiences</h1>
        <i class="fa-brands fa-envira fa-flip-horizontal"></i>
        <p> Morbi pharetra, quam id consequat imperdiet, lectus est tincidunt massa, eu posuere leo nibh non fermentum</p>
        <hr>
        <p>Vestibulum ne velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat volutpat.
            Fusce laoreet mi leo. Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec.
            Aliquam erat volutpat. Fusce laoreet mi leo.
        </p>
        <button>OUR APPROACH</button>
    </section>
    <section class="emoji-container">
        <div class="emoji-start">
            <i class="fa-solid fa-hands fa-flip-horizontal"></i>
            <p>Massages</p>
        </div>
        <div class="emoji-end">
            <i class="fa-regular fa-face-smile"></i>
            <p>Therapy</p>
        </div>
        <div class="emoji-start">
            <i class="fa-solid fa-heart"></i>
            <p>Relaxing</p>
        </div>
        <div class="emoji-end">
            <i class="fa-regular fa-moon"></i>
            <p>Meditation</p>
        </div>
        <div class="emoji-start">
            <i class="fa-regular fa-snowflake"></i>
            <p>Natural Beauty</p>
        </div>
    </section>
</template>


<script>
export default {
    name: `AppMain`,

}
</script>


<style lang="scss">
@use '../styles/general.scss' as *;
@use "../styles/partials/mixins.scss" as *;
@use "../styles/partials/variables" as *;

section.experiences {
    @include flex(column, center, center);
    margin: 0 auto;
    width: 50%;

    button {
        border: 2px solid $icon-color;
        color: $icon-color;
        border-radius: 50px;
        padding: .5rem 2rem;
        background-color: white;
    }
}

section.emoji-container {
    @include flex(row, center, center);
    margin: 0 auto;
    width: 70%;
    height: 300px;
    border: 1px solid black;

    .emoji-start {
        @include flex(column, start, center);
        width: calc(100% / 3);
        color: $icon-color;
    }

    .emoji-end {
        @include flex(column, end, center);
        width: calc(100% / 2);
        color: $icon-color;
    }
}
</style>