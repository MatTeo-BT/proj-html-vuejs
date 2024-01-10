<template>
    <header>
        <section class="navigation">
            <nav>
                <ul>
                    <li><i class="fa-solid fa-house light-blue"></i></li>
                    <li><i class="fa-brands fa-pagelines"></i>
                        <span>TREATMENTS</span>
                        <p>Face & Body</p>
                    </li>
                    <li><i class="fa-solid fa-person"></i>
                        <span>ABOUT</span>
                        <p>Our Team</p>
                    </li>

                </ul>
            </nav>
            <div class="logo">
                <img src="../assets/images/avada-spa-logo-new.png" alt="avada-logo">
            </div>
            <nav>
                <ul>
                    <li><i class="fa-solid fa-heart"></i>
                        <span>JOURNAL</span>
                        <p>Tips & Tricks</p>
                    </li>
                    <li><i class="fa-solid fa-bookmark"></i>
                        <span>BOOK NOW</span>
                        <p>Special Offers</p>
                    </li>
                    <li><i class="fa-solid fa-plus"></i></li>
                </ul>
            </nav>
        </section>
        <section class="jumbo">
            <div class="fst-italic">
                <p>Give yourself permission</p>
            </div>
            <h1>Relax, Revive & Rejuvenate</h1>
            <button>EXPLORE TREATMENTS</button>
        </section>
    </header>
</template>


<script>
export default {
    name: `AppHeader`,
}
</script>


<style lang="scss">
@use '../styles/general.scss' as *;
@use "../styles/partials/mixins.scss" as *;
@use "../styles/partials/variables" as *;

section.navigation {
    @include flex(row, center, center);

    p {
        font-size: 10px;
    }

    ul {
        @include flex(row, center, center);
        list-style-type: none;

        li {
            @include flex(column, center, center);
            padding: .4rem 4rem;
            color: $icon-color;
            margin-top: 1rem;
        }

        li span,
        p {
            color: $grey-color;
        }

        li i {
            font-size: 18px;
        }
    }
}

.light-blue {
    color: #34A7B9;
}

section.jumbo {
    background-image: url(../assets/images/avada-spa-slider-image-1-new.jpg);
    width: 100%;
    height: 1000px;
    color: white;
    @include flex(column, center, center);
    font-family: $main-font;

    div p {
        font-size: 33px;
    }

    h1 {
        font-size: 80px;
    }

    button {
        padding: .6rem 2rem;
        background-color: $icon-color;
        border: none;
        border-radius: 3rem;
        color: white;
        font-family: Arial, Helvetica, sans-serif;
    }

    button:hover {
        background-color: #33A7B9
    }
}
</style>
