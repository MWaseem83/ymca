<template>
    <div class="px-5">
        <b-navbar
            toggleable="lg"
            style="margin-left: 150px; margin-right: 150px"
        >
            <img alt="YMCA" src="../assets/ymcalogo.png" />
            <b-navbar-toggle target="top-nav-collapse"></b-navbar-toggle>
            <div class="ms-auto">
                <b-collapse id="top-nav-collapse" is-nav>
                    <!-- Right aligned nav items -->
                    <b-navbar-nav class="ms-auto top-nav-items">
                        <b-nav-item href="#">GIVE</b-nav-item>
                        <b-nav-item href="#">JOIN</b-nav-item>
                        <b-nav-item href="#">LOGIN</b-nav-item>
                        <div>
                            <b-nav-form class="position-relative">
                                <b-form-input
                                    class="d-inline search-box border-0 rounded-0 border-bottom border-2"
                                    placeholder="Search..."
                                    style="width: 120px"
                                ></b-form-input>
                                <b-icon
                                    icon="search"
                                    class="position-absolute top-50 end-0 translate-middle-y"
                                    style="width: 20px; height: 20px"
                                ></b-icon>
                                <!-- <b-button size="sm" class="my-2 my-sm-0" type="submit">
                                    Search
                                </b-button> -->
                            </b-nav-form>
                        </div>
                    </b-navbar-nav>
                </b-collapse>
                <div class="d-flex justify-content-end">
                    <div class="top-text-box">Merrimack Valley YMCA</div>
                </div>
            </div>
        </b-navbar>
    </div>
</template>

<script>
export default {
    name: "NavbarComponent",
};
</script>
<style>
.top-text-box {
    font-family: "Franklin Gothic Medium", "Arial Narrow", Arial,
        sans-serif Bold !important;
    font-size: 28px;
    font-weight: 700;
    color: rgb(0, 172, 150);
}
.top-nav-items {
    font-family: "Franklin Gothic Medium", "Arial Narrow", Arial,
        sans-serif Bold !important;
    font-size: 18px;
    font-weight: 900;
}
</style>
