<template>
    <section class="service-container">
        <Card v-for="service in listTreatments" :image="service.img" :title="service.title" :subtitle="service.subtitle" />
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
                    img: "/images/Layer-1-new.jpg",
                    title: "Massage",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                },
                {
                    img: "/images/Layer-1-new.jpg",
                    title: "Aromatherapy",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                },
                {
                    img: "/images/Layer-1-new.jpg",
                    title: "Heat Therapy",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                },
                {
                    img: "/images/Layer-1-new.jpg",
                    title: "Skin Care",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                },
                {
                    img: "/images/Layer-1-new.jpg",
                    title: "Spa Days",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                },
                {
                    img: "/images/Layer-1-new.jpg",
                    title: "Beauty Treatments",
                    subtitle: "Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium. Aliquam erat volutpat. Fusce laoreet mi leo."

                }, {
                    img: "/images/Layer-1-new.jpg",
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