<template>
    <div class="px-5 topnavebottom">
        <div style="margin-left: 150px; margin-right: 150px">
            <b-navbar toggleable="lg">
                <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
                <div>
                    <b-collapse id="nav-collapse" is-nav>
                        <!-- Right aligned nav items -->
                        <b-navbar-nav
                            class="ms-auto main-nav-items gap-4 navbar-light"
                        >
                            <b-nav-item href="#">EVENTS</b-nav-item>
                            <b-nav-item href="#">SCHEDULES</b-nav-item>
                            <b-nav-item href="#">PROGRAMS</b-nav-item>
                            <b-nav-item-dropdown text="CHILD CARE" right>
                                <b-dropdown-item href="#">EN</b-dropdown-item>
                                <b-dropdown-item href="#">ES</b-dropdown-item>
                                <b-dropdown-item href="#">RU</b-dropdown-item>
                                <b-dropdown-item href="#">FA</b-dropdown-item>
                            </b-nav-item-dropdown>
                            <b-nav-item href="#">GET INVOLVED</b-nav-item>
                            <b-nav-item href="#">ABOUT US</b-nav-item>
                            <b-nav-item href="#">CAMPS</b-nav-item>
                        </b-navbar-nav>
                    </b-collapse>
                </div>
            </b-navbar>
        </div>
    </div>
</template>

<script>
export default {
    name: "MainNavbarComponent",
};
</script>
<style>
.topnavebottom {
    border-bottom: 6px solid rgb(0, 172, 150);
    background-color: rgb(245, 245, 245);
}
.main-nav-items {
    font-family: "Franklin Gothic Medium", "Arial Narrow", Arial,
        sans-serif Bold !important;
    font-size: 16px;
    font-weight: 700;
}
</style>
