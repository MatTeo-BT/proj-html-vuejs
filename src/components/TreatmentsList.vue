<template>
    <section class="service-container">
        <Card v-for="service in listTreatments" :immagine="service.img" :title="service.title"
            :subtitle="service.subtitle" />
    </section>
</template>


<script>
import Card from "./Card.vue";
export default {
    name: `TreatmentsList`,
    data() {
        return {
            listTreatments: [
                {
                    img: "../assets/images/Layer-1-new-400x440.jpg",
                    title: "Hydrotherapy",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                },
                {
                    img: "../assets/images/Layer-2-new-400x440.jpg",
                    title: "Massage",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                },
                {
                    img: "../assets/images/Layer-3-new-400x440.jpg",
                    title: "Aromatherapy",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                },
                {
                    img: "../assets/images/Layer-4-new-400x440.jpg",
                    title: "Heat Therapy",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                },
                {
                    img: "../assets/images/Layer-5-new-400x440.jpg",
                    title: "Skin Care",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                },
                {
                    img: "../assets/images/Layer-6-new-400x440.jpg",
                    title: "Spa Days",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                },
                {
                    img: "../assets/images/Layer-7-new-400x440.jpg",
                    title: "Beauty Treatments",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                }, {
                    img: "../assets/images/layer8-new-400x440.jpg",
                    title: "Residential",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                },

            ]
        }
    },
    components: {
        Card,
    }
}
</script>


<style lang="scss">
@use '../styles/general.scss' as *;
@use "../styles/partials/mixins.scss" as *;
@use "../styles/partials/variables" as *;

section.service-container {
    @include flex(row, start, start);
    flex-wrap: wrap;
}
</style>