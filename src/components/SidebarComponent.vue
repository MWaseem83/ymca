<template>
    <div class="px-5">
        <div style="margin-left: 150px; margin-right: 150px">
            <div style="width: 250px">
                <template>
                    <div class="p-3">
                        <nav class="mb-3">
                            <b-nav vertical>
                                <b-nav-item active @click="hide">
                                    Active
                                </b-nav-item>
                                <b-nav-item href="#link-1" @click="hide">
                                    Link
                                </b-nav-item>
                                <b-nav-item href="#link-2" @click="hide">
                                    Another Link
                                </b-nav-item>
                                <b-nav-item-dropdown text="CHILD CARE" right>
                                    <b-dropdown-item href="#">
                                        EN
                                    </b-dropdown-item>
                                    <b-dropdown-item href="#">
                                        ES
                                    </b-dropdown-item>
                                    <b-dropdown-item href="#">
                                        RU
                                    </b-dropdown-item>
                                    <b-dropdown-item href="#">
                                        FA
                                    </b-dropdown-item>
                                </b-nav-item-dropdown>
                                <b-nav-item-dropdown
                                    text="CHILD CARE"
                                    class="open"
                                >
                                    <b-dropdown-item href="#" open>
                                        EN
                                    </b-dropdown-item>
                                    <b-dropdown-item href="#">
                                        ES
                                    </b-dropdown-item>
                                    <b-dropdown-item href="#">
                                        RU
                                    </b-dropdown-item>
                                    <b-dropdown-item href="#">
                                        FA
                                    </b-dropdown-item>
                                </b-nav-item-dropdown>
                            </b-nav>
                        </nav>
                    </div>
                </template>
            </div>
        </div>
    </div>
</template>
