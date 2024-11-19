<template>
    <div class="home">
        <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
        <NavbarComponent />
        <MainNavbarComponent />
        <!-- <SampleComponent msg="Welcome to Your Vue.js App" /> -->
        <div class="px-5 program-heading">
            <div style="margin-left: 150px; margin-right: 150px">
                <div class="d-flex justify-content-center">
                    <h1>Programs</h1>
                </div>
            </div>
        </div>
        <div class="px-5">
            <div style="margin-left: 150px; margin-right: 150px">
                <div
                    class="d-flex flex-column align-items-center program-sub-heading"
                >
                    <h2>Program Registration is now OPEN!</h2>
                    <h2>Register for your favorite program today!</h2>
                </div>
            </div>
        </div>
        <b-container>
            <b-row align-h="start">
                <b-col cols="12" md="3" lg="3">
                    <SideMenuComponent />
                </b-col>
                <b-col cols="12" md="9" lg="9">
                    <CardComponent />
                </b-col>
            </b-row>
        </b-container>
        <FooterComponent />
    </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
// import SampleComponent from "@/components/SampleComponent.vue";
import NavbarComponent from "@/components/NavbarComponent.vue";
import MainNavbarComponent from "@/components/MainNavbarComponent.vue";
import SideMenuComponent from "@/components/SideMenuComponent.vue";
import CardComponent from "@/components/CardComponent.vue";
import FooterComponent from "@/components/FooterComponent.vue";

export default {
    name: "ProgramView",
    components: {
        // SampleComponent,
        NavbarComponent,
        MainNavbarComponent,
        SideMenuComponent,
        CardComponent,
        FooterComponent,
    },
};
</script>
<style>
.program-sub-heading {
    color: rgb(27, 130, 198);
}
.program-heading {
    background-color: rgb(0, 172, 150);
    color: rgb(255, 255, 255);
}
</style>
