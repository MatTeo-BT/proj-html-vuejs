<template>
    <main>
        <section class="experiences">
            <h1>Luxury Spa Experiences</h1>
            <i class="fa-brands fa-envira fa-flip-horizontal fs-2"></i>
            <p class="fs-4 fst-italic"> Morbi pharetra, quam id consequat imperdiet, lectus est tincidunt massa, eu
                posuere
                leo nibh
                non fermentum
            </p>
            <hr>
            <span>Vestibulum ne velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat
                volutpat.
                Fusce laoreet mi leo. Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit
                pretium
                nec.
                Aliquam erat volutpat. Fusce laoreet mi leo.
            </span>
            <button>OUR APPROACH</button>
        </section>
        <section class="emoji-container">
            <div>
                <i class="fa-solid fa-hands fa-flip-horizontal emoji"></i>
                <p>Massages</p>
            </div>
            <div>
                <i class="fa-regular fa-face-smile emoji end"></i>
                <p>Therapy</p>
            </div>
            <div>
                <i class="fa-solid fa-heart emoji "></i>
                <p>Relaxing</p>
            </div>
            <div>
                <i class="fa-regular fa-moon emoji end"></i>
                <p>Meditation</p>
            </div>
            <div>
                <i class="fa-regular fa-snowflake emoji"></i>
                <p>Natural Beauty</p>
            </div>
        </section>
        <section class="treatments-container">
            <div class="card">
                <img class="card-img" src="../assets/images/face_and_body_treatments-new.jpg"
                    alt="face-and-body-treatments">
            </div>
            <div class="treatments-plan">
                <h1>Face & Body Treatments</h1>
                <p>Pellentesque nec felis efficitur, sagittis eros et, pharetra risus. <br>
                    Sed at lacus a ex imperdiet
                    disgnissim vehicula quam.
                    Vestibulum ante ipsum primis.
                </p>
                <article class="single-plan p-3">
                    <div>
                        <i class="fa-solid fa-square-minus"></i>
                        <span>Oil Massage</span>
                    </div>
                    <p class="p-1">$62 For 2 Hours - Lorem ipsum dolor sit amet</p>
                </article>
                <article class="single-plan p-3">
                    <div>
                        <i class="fa-solid fa-square-plus"></i>
                        <span>Manicure</span>
                    </div>
                    <p class="p-1">$62 For 2 Hours - Lorem ipsum dolor sit amet</p>
                </article>
                <article class="single-plan p-3">
                    <div>
                        <i class="fa-solid fa-square-plus"></i>
                        <span>Aromatherapy</span>
                    </div>
                    <p class="p-1">$62 For 2 Hours - Lorem ipsum dolor sit amet</p>
                </article>
            </div>
        </section>
        <section class="available-service">
            <h2>OUR TREATMENTS</h2>
        </section>
    </main>
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

main {
    font-family: $main-font;
}

section.experiences {
    @include flex(column, center, center);
    margin: 0 auto;
    width: 50%;
    margin-top: 8rem;

    h1 {
        color: $grey-color;
        font-size: 73px;
    }

    i {
        color: $icon-color;
        padding: 1.5rem;
    }

    p {
        color: $icon-color;
        text-align: center;
        margin-bottom: 2rem;
    }

    hr {
        width: 110px;
        border: 1px solid $icon-color;
    }

    span {
        text-align: center;
        margin: 2rem 0 3rem 0;
    }

    button {
        border: 2px solid $icon-color;
        color: $icon-color;
        border-radius: 50px;
        padding: .5rem 2rem;
        background-color: white;
        font-family: Arial, Helvetica, sans-serif
    }

    button:hover {
        color: #33A7B9;
        border: 2px solid #33A7B9
    }
}


section.emoji-container {
    @include flex(row, center, center);
    margin: 0 auto;
    width: 70%;
    height: 300px;

    div {
        @include flex(column, start, center);
        padding: 5rem;

        p {
            color: $grey-color;
            padding: .7rem;
        }
    }

    .emoji {
        color: $icon-color;
        font-size: 3.7rem;

    }

    .end {
        margin-top: 8rem;
    }
}

section.treatments-container {
    @include flex(row, center, center);
    height: 1000px;
    background-color: $treatments-bg-color;

    div.treatments-plan h1 {
        color: $grey-color;
        font-size: 60px;


    }

    div.treatments-plan {
        margin: 1rem 6rem;
        width: 40%;

        p {
            text-align: left;
        }

        article.single-plan {

            border: 1px solid $icon-color;
            background-color: white;
            width: 40%;
            margin-bottom: 1.5rem;


            i,
            p {
                padding: 1rem 0;

            }

            i {
                color: $icon-color;
            }

            div {
                @include flex(row, start, center)
            }
        }
    }

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