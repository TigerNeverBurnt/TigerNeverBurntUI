<template>
    <div id="app">
        <v-app id="inspire">
                <v-container fluid fill-height>
                    <v-layout align-content-space-around>
                        <v-flex>
                                <v-toolbar dark color="primary">
                                    <v-toolbar-title>Editor</v-toolbar-title>
                                    <v-spacer></v-spacer>
                                    <v-tooltip bottom>
                                        <v-btn
                                                icon
                                                large
                                                :href="source"
                                                target="_blank"
                                                slot="activator"
                                        >
                                            <v-icon large>code</v-icon>
                                        </v-btn>
                                        <span>Source</span>
                                    </v-tooltip>
                                </v-toolbar>
                                <v-textarea
                                        full-width=true
                                        auto-grow
                                        autofocus=true
                                        solo
                                        counter=1000
                                        name="input"
                                        clearable=true
                                        value="The Woodman set to work at once, and so sharp was his axe that the tree was soon chopped nearly through."
                                ></v-textarea>
                        </v-flex>
                    </v-layout>
                </v-container>
        </v-app>
    </div>

</template>

<script>
    import {mapState} from 'vuex'

    var timeout = null;
    export default {
        computed: {
            message: {
                get() {
                    return this.$store.state.main_text
                },
                set(value) {
                    clearTimeout(timeout);
                    timeout = setTimeout(() => {
                        this.$store.dispatch('SetMainText', value);
                    }, 2000);

                }
            }
        }
    }
</script>

<style>
</style>
