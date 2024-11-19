<template>
    <b-col
        lg="4"
        md="6"
        xs="12"
        style="padding-right: 5px; padding-bottom: 45px"
    >
        <div class="d-flex fit-contents">
            <div class="d-flex rounded-3 cardcontainer">
                <a
                    href="https://mvymca.org/program/youth-basketball-league-ybl/"
                >
                    <!-- <b-card-group> -->
                    <b-card-img
                        :src="require('../assets/img/' + imagepath + '')"
                        img-alt="Image"
                        style="height: auto"
                        class="img-fluid align-items-bottom rounded-3"
                    >
                    </b-card-img>
                    <div class="overlay">
                        <h2 class="cardtext">{{ name }}</h2>
                    </div>
                </a>
            </div>
        </div>
    </b-col>
</template>
<script>
export default {
    name: "SingleCardComponent",
    props: { name: String, imagepath: String },
};
</script>
<style>
.cardcontainer {
    position: relative;
    /* width: 82%;
    height: 91%; */
    /* width: 100%; */
    overflow: hidden;
    text-align: center;
}
.overlay {
    width: 100%;
    height: 100%;
    position: absolute;
    overflow: hidden;
    top: 0;
    left: 0;
    transition: all 0.4s ease-in-out;
}
.overlay h2 {
    position: absolute;
    bottom: -9px;
    width: 100%;
    padding: 8px;
    color: #fff;
    background: rgba(0, 97, 175, 0.85);
    text-transform: uppercase;
    text-align: center;
    transition: all 0.4s ease-in-out;
    font-size: 17px;
}
.cardcontainer:hover .overlay {
    /*background-color: rgba(48, 152, 157, 0.4);*/
    background: rgba(0, 97, 175, 0.85);
}
.cardcontainer:hover h2 {
    transform: translateY(17px);
    margin: 0px;
}
</style>
