<template>
    <footer>
        <section class="logo"><img src="../assets/images/avada-spa-logo-new.png" alt="avada-logo"></section>
        <div class="copyright"> COPYRIGHT 2012 - 2020 | AVADA THEME BY THEMEFUSION | ALL RIGHTS RESERVED | POWERED BY
            WORDPRESS</div>
        <section class="social fs-5">
            <i class="fa-brands fa-facebook"></i>
            <i class="fa-brands fa-twitter"></i>
            <i class="fa-brands fa-instagram"></i>
            <i class="fa-brands fa-youtube"></i>
        </section>
    </footer>
</template>


<script>
export default {
    name: `AppFooter`,
}
</script>


<style lang="scss">
@use '../styles/general.scss' as *;
@use "../styles/partials/mixins.scss" as *;
@use "../styles/partials/variables" as *;

footer {
    @include flex(row, space-around, center);
    height: 150px;
    border-top: 10px solid #E9EAEE;

    .copyright {
        font-size: 11px;
        color: #BEBDBD;
    }

    section.social {
        @include flex(row, space-around, center);


        i {
            background-color: #E8E8E8;
            color: #BEBDBD;
            padding: 1rem;
            margin: 0 .5rem;

        }
    }
}
</style>