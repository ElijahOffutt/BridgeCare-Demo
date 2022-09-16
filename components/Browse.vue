<template>
  <v-container class="py-12 my-12">
    <v-row justify="center">
        <v-col cols="12">
            <v-row dense no-gutters>
                <v-col cols="12">
                    <br />
                    <h3 style="font-size: 2em;">Browse other Modules</h3>
                    <br />
                </v-col>
                <v-col cols="6" v-for="(link, i) in links" :key="i">
                    <v-list-item @click="$router.push(link.link)" style="cursor: pointer;" ripple>
                        <v-list-item-content>
                            <v-list-item-title><b>{{link.text}}</b></v-list-item-title>
                            <v-list-item-subtitle>{{link.subText}}</v-list-item-subtitle>
                        </v-list-item-content>
                    </v-list-item>
                </v-col>
            </v-row>
        </v-col>
    </v-row>
  </v-container>
</template>

<script>
let links = require('/static/Pages.json')
export default {
    data(){return{
        links
    }}
}
</script>