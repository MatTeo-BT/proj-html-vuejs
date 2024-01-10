<template>
    <section class="reference ">
        <div>
            <p class="fst-italic">"If you want to relax, watch the clouds pass by if you're laying on the grass,
                or sit in front of the creek; just doing nothing and having those still moments is what really rejuvenates
                the body..."</p>
        </div>
        <h5>FRIEDA FRIEDSON, MASSEUSE</h5>
    </section>
    <section class="discount">
        <div class="discount-rate">
            <h2>25%</h2>
            <p>SPECIAL OFFER</p>
        </div>
        <div>
            <h1 class="fst-italic">Take some time. Treat yourself. You deserve it.</h1>
            <p>Book a treatment this mont and receive a 25% on all further treatments.</p>
        </div>
        <button class="fw-bold">BOOK NOW</button>

    </section>
</template>


<script>
export default {
    name: `UpperFooter`,
}
</script>


<style lang="scss">
@use '../styles/general.scss' as *;
@use "../styles/partials/mixins.scss" as *;
@use "../styles/partials/variables" as *;



section.reference {
    background-image: url(../assets/images/Home-quota-new.jpg);
    background-repeat: no-repeat;
    background-position: left;
    background-size: cover;
    width: 100%;
    height: 800px;
    color: white;
    @include flex(column, space-evenly, center);
    text-align: center;
    font-family: $main-font;

    h5 {
        font-family: Arial, Helvetica, sans-serif;
    }

    div {
        width: 20%;
        line-height: 2rem;
    }

}

section.discount {
    height: 400px;
    background-image: url(../assets/images/ptb_cta-new.jpg);
    width: 100%;
    color: white;
    @include flex(row, center, center);

    .discount-rate {
        border: 1px solid $icon-color;
        padding: 1.5rem;
        margin-right: 40px;

        h2 {
            font-size: 65px;
            text-align: center;
        }
    }

    button {
        border: none;
        color: white;
        padding: .5rem 2rem;
        background-color: $icon-color;
        border-radius: 30px;
        margin-left: 10rem;
    }
}
</style>