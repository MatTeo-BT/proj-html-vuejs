<template>
    <header>
        <section class="navigation">
            <nav>
                <ul>
                    <li><i class="fa-solid fa-house light-blue"></i> </li>
                    <li><i class="fa-brands fa-pagelines"></i>
                        <p>TREATMENTS</p>
                    </li>
                    <li><i class="fa-solid fa-person"></i></li>
                </ul>
            </nav>
            <div class="logo">
                <img src="../assets/images/avada-spa-logo-new.png" alt="avada-logo">
            </div>
            <nav>
                <ul>
                    <li><i class="fa-solid fa-heart"></i></li>
                    <li><i class="fa-solid fa-bookmark"></i></li>
                    <li><i class="fa-solid fa-plus"></i></li>
                </ul>
            </nav>
        </section>
        <section class="jumbo">
            <div>Give yourself permission</div>
            <div>Relax, Revive & Rejuvenate</div>
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

    ul {
        @include flex(row, center, center);
        list-style-type: none;

        li {
            @include flex(column, center, center);
            padding: 2rem;
            color: $icon-color;
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
}
</style>
