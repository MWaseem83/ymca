<template>
    <div style="width: 100%">
        <div style="width: 100%">
            <div class="side-menu-wrapper" style="width: 100%">
                <div style="width: 100%">
                    <section class="dropdown-wrapper">
                        <div
                            @click="isBranchVisible = !isBranchVisible"
                            class="dropdown-head d-flex"
                        >
                            <svg
                                xmlns="http://www.w3.org/2000/svg"
                                viewBox="0 0 24 24"
                                fill="currentColor"
                                width="25"
                                height="25"
                                color="#bbbbbb"
                                style="
                                    overflow: hidden;
                                    transition: transform 0.5s;
                                "
                                :class="isBranchVisible ? '' : 'rotate270'"
                            >
                                <path
                                    d="M11.9999 13.1714L16.9497 8.22168L18.3639 9.63589L11.9999 15.9999L5.63599 9.63589L7.0502 8.22168L11.9999 13.1714Z"
                                ></path>
                            </svg>
                            <h4>BRANCH</h4>
                        </div>
                        <Transition :duration="180">
                            <div
                                v-if="isBranchVisible"
                                class="dropdown-popover"
                                style="
                                    overflow: hidden;
                                    /* visibility: visible; */
                                    /* max-height: 0px; */
                                    /* transition: all 0.1s ease-in-out; */
                                    /* transition: opacity 0.5s; */
                                    /* transition: max-height 0.5s; */
                                "
                            >
                                <div
                                    class="options"
                                    style="
                                        /* transition: all 0.1s ease-in-out; */
                                        overflow: hidden;
                                        /* transition: opacity 0.5s; */
                                    "
                                >
                                    <ul class="filtercheckblock">
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Andover/North Andover
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Lawrence
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Methuen
                                            </b-form-checkbox>
                                        </ol>
                                    </ul>
                                </div>
                            </div>
                        </Transition>
                    </section>
                </div>
                <div style="width: 100%">
                    <section class="dropdown-wrapper">
                        <div
                            @click="isAgeVisible = !isAgeVisible"
                            class="dropdown-head d-flex"
                        >
                            <svg
                                xmlns="http://www.w3.org/2000/svg"
                                viewBox="0 0 24 24"
                                fill="currentColor"
                                width="25"
                                height="25"
                                color="#bbbbbb"
                                style="
                                    overflow: hidden;
                                    transition: transform 0.5s;
                                "
                                :class="isAgeVisible ? '' : 'rotate270'"
                            >
                                <path
                                    d="M11.9999 13.1714L16.9497 8.22168L18.3639 9.63589L11.9999 15.9999L5.63599 9.63589L7.0502 8.22168L11.9999 13.1714Z"
                                ></path>
                            </svg>
                            <h4>AGE</h4>
                        </div>
                        <Transition :duration="180">
                            <div
                                v-if="isAgeVisible"
                                class="dropdown-popover"
                                style="
                                    overflow: hidden;
                                    /* visibility: visible; */
                                    /* max-height: 0px; */
                                    /* transition: all 0.1s ease-in-out; */
                                    /* transition: opacity 0.5s; */
                                    /* transition: max-height 0.5s; */
                                "
                            >
                                <div
                                    class="options"
                                    style="
                                        /* transition: all 0.1s ease-in-out; */
                                        overflow: hidden;
                                        /* transition: opacity 0.5s; */
                                    "
                                >
                                    <ul class="filtercheckblock">
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Parent/Child
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Preschool (Ages 3-5)
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Youth (Ages 6-12)
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Teens (Ages 13-18)
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Adult
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Seniors (Ages 65+)
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Families
                                            </b-form-checkbox>
                                        </ol>
                                    </ul>
                                </div>
                            </div>
                        </Transition>
                    </section>
                </div>
                <div style="width: 100%">
                    <section class="dropdown-wrapper">
                        <div
                            @click="isAtcIntrstVisible = !isAtcIntrstVisible"
                            class="dropdown-head d-flex"
                        >
                            <svg
                                xmlns="http://www.w3.org/2000/svg"
                                viewBox="0 0 24 24"
                                fill="currentColor"
                                width="25"
                                height="25"
                                color="#bbbbbb"
                                style="
                                    overflow: hidden;
                                    transition: transform 0.5s;
                                "
                                :class="isAtcIntrstVisible ? '' : 'rotate270'"
                            >
                                <path
                                    d="M11.9999 13.1714L16.9497 8.22168L18.3639 9.63589L11.9999 15.9999L5.63599 9.63589L7.0502 8.22168L11.9999 13.1714Z"
                                ></path>
                            </svg>
                            <h4>Activity/Interest</h4>
                        </div>
                        <Transition :duration="180">
                            <div
                                v-if="isAtcIntrstVisible"
                                class="dropdown-popover"
                                style="
                                    overflow: hidden;
                                    /* visibility: visible; */
                                    /* max-height: 0px; */
                                    /* transition: all 0.1s ease-in-out; */
                                    /* transition: opacity 0.5s; */
                                    /* transition: max-height 0.5s; */
                                "
                            >
                                <div
                                    class="options"
                                    style="
                                        /* transition: all 0.1s ease-in-out; */
                                        overflow: hidden;
                                        /* transition: opacity 0.5s; */
                                    "
                                >
                                    <ul class="filtercheckblock">
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Active Living Center
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Arts/Dance/Music
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Aquatics
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Competitive Swimming
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Events
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Group/Personal Training
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Gymnastics
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                PHealth and Wellness
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Parties/Rentals
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Special Interest/Cooking
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Sports
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Inclusion
                                            </b-form-checkbox>
                                        </ol>
                                    </ul>
                                </div>
                            </div>
                        </Transition>
                    </section>
                </div>
                <div style="width: 100%">
                    <section class="dropdown-wrapper">
                        <div
                            @click="isDayWeekVisible = !isDayWeekVisible"
                            class="dropdown-head d-flex"
                        >
                            <svg
                                xmlns="http://www.w3.org/2000/svg"
                                viewBox="0 0 24 24"
                                fill="currentColor"
                                width="25"
                                height="25"
                                color="#bbbbbb"
                                style="
                                    overflow: hidden;
                                    transition: transform 0.5s;
                                "
                                :class="isDayWeekVisible ? '' : 'rotate270'"
                            >
                                <path
                                    d="M11.9999 13.1714L16.9497 8.22168L18.3639 9.63589L11.9999 15.9999L5.63599 9.63589L7.0502 8.22168L11.9999 13.1714Z"
                                ></path>
                            </svg>
                            <h4>Day of Week</h4>
                        </div>
                        <Transition :duration="180">
                            <div
                                v-if="isDayWeekVisible"
                                class="dropdown-popover"
                                style="
                                    overflow: hidden;
                                    /* visibility: visible; */
                                    /* max-height: 0px; */
                                    /* transition: all 0.1s ease-in-out; */
                                    /* transition: opacity 0.5s; */
                                    /* transition: max-height 0.5s; */
                                "
                            >
                                <div
                                    class="options"
                                    style="
                                        /* transition: all 0.1s ease-in-out; */
                                        overflow: hidden;
                                        /* transition: opacity 0.5s; */
                                    "
                                >
                                    <ul class="filtercheckblock">
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Sunday
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Monday
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Tuesday
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Wednesday
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Thursday
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Friday
                                            </b-form-checkbox>
                                        </ol>
                                        <ol class="checkboxmargin">
                                            <b-form-checkbox>
                                                Saturday
                                            </b-form-checkbox>
                                        </ol>
                                    </ul>
                                </div>
                            </div>
                        </Transition>
                    </section>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: "SideMenuComponent",
    data() {
        return {
            searchQuery: "",
            isBranchVisible: true,
            isAgeVisible: true,
            isAtcIntrstVisible: true,
            isDayWeekVisible: true,
        };
    },
    mounted() {},
};
</script>
<style>
.options {
    width: 100%;
    /* color: aqua; */
    ul {
        list-style: none;
        text-align: left;
        padding-left: 0px;
        li {
            padding: 10px;
        }
    }
}
.dropdown-wrapper {
    position: relative;
    /* transition: transform 0.5s; */
}
.dropdown-popover {
    /* position: absolute;
    top: 0px; */
    color: black;
    width: 100%;
}
.dropdown-head h4 {
    font-size: 1.1rem;
    font-weight: 700;
    text-transform: uppercase;
    color: #0061af;
    position: relative;
    margin-bottom: 0em;
    padding: 2px 0 0px 0px;
}
.dropdown-head {
    margin: 5px 20px 0px 20px;
    border-bottom: 1px solid #dddddd;
}
.dropdown-head h4:hover {
    color: #646466;
}
/* .dropdown-header svg {
    background: linear-gradient(
        135deg,
        rgb(2, 3, 129) 0%,
        rgb(40, 116, 252) 100%
    );
} */
.rotate270 {
    transition: transform 0.5s;
    transform: rotate(-90deg);
}
.side-menu-wrapper {
    width: 100%;
    background-color: #f5f5f5;
    box-shadow: rgba(0, 0, 0, 0.2) 4px 4px 20px 0px;
    z-index: 1;
    padding: 15px 0 10px 0px;
}
/* .v-enter-active {
    transition: transform 0.5s ease;
}
.v-leave-active {
    transition: transform 0.5s ease;
} */
.filtercheckblock {
    margin: 0.5em 0.5em 0em 0.5em;
}
.checkboxmargin {
    padding: 0px 0px 5px 15px;
}
.checkboxmargin input {
    margin: 0px 5px 0px 0px;
    scale: 1.1;
}
.checkboxmargin label {
    font-size: 0.9rem;
    font-weight: 400;
    color: rgb(100, 100, 102);
}
</style>
