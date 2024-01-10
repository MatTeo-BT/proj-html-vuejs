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
    <section class="treatments-container">
        <div class="card">
            <img class="card-img" src="../assets/images/face_and_body_treatments-new.jpg" alt="face-and-body-treatments">
        </div>
        <div class="treatments-plan">
            <h1>Face & Body Treatments</h1>
        </div>
    </section>
    <section class="available-service">
        <h2>OUR TREATMENTS</h2>
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

section.treatments-container {
    @include flex(row, center, center);
    height: 1000px;
    background-color: $treatments-bg-color;


    .card {
        box-shadow: 0 4px 4px 0 rgba(0, 0, 0, 0.2);
        transition: 0.3s;
        width: 550px;
        height: 80%;
        @include flex(row, center, center);

        .card-img {
            width: 88%;
            height: 90%;
        }
    }

    .card:hover {
        box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
    }
}

section.available-service {
    height: 200px;
    background-image: url(../assets/images/ptb_cta-new.jpg);
    width: 100%;
    color: white;
    @include flex(row, center, center)
}
</style>