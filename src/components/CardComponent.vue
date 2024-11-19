<template>
    <div class="px-2">
        <div>
            <div style="background-color: white">
                <section class="d-flex" style="position: relative">
                    <b-row style="margin-bottom: 15px; padding: 10px">
                        <SingleCardComponent
                            v-for="card1 in cards"
                            :key="card1.id"
                            :name="card1.name"
                            :imagepath="card1.imagepath"
                        ></SingleCardComponent>
                    </b-row>
                </section>
            </div>
        </div>
    </div>
</template>
<script>
import image from "../assets/img/no_image.jpg";
import SingleCardComponent from "./SingleCardComponent.vue";
export default {
    name: "CardComponent",
    components: {
        SingleCardComponent,
    },
    mounted() {
        this.fetchdata();
    },
    data() {
        return {
            searchQuery: "",
            image,
            cards: [],
        };
    },
    methods: {
        async fetchdata() {
            const res = await fetch("cards.json");
            const val = await res.json();
            this.cards = val;
            console.log(val);
        },
    },
};
</script>
