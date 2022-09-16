<template>
  <v-app-bar flat class="px-12" style="background-color: white;" app>
    <img @click="$router.push('/')" style="cursor: pointer;" src="https://uploads-ssl.webflow.com/5f6ce074a62cf885680ba383/5f8a5d5c39466ae063c674c5_bridgecare%20logo_color.svg" loading="lazy" alt="BridgeCare logo" height="40px">
    <v-spacer />
    <v-menu rounded bottom offset-y left open-on-hover>
        <template #activator="{on}">
            <v-btn text x-large v-on="on">
                <span style="text-transform: capitalize;">Products</span>
                <v-icon>mdi-chevron-down</v-icon>
            </v-btn>
        </template>
        <v-sheet ripple>
            <v-list>
                <v-list-item @click="$router.push(link.link)" style="cursor: pointer;" ripple v-for="(link, i) in links" :key="i">
                    <v-list-item-content>
                        <v-list-item-title><b>{{link.text}}</b></v-list-item-title>
                        <v-list-item-subtitle>{{link.subText}}</v-list-item-subtitle>
                    </v-list-item-content>
                </v-list-item>
            </v-list>
        </v-sheet>
    </v-menu>
    <v-btn @click="$router.push('/request-a-demo')" text x-large>
        <span style="text-transform: capitalize;">Request a Demo</span>
    </v-btn>
  </v-app-bar>
</template>

<script>
let links = require('/static/Pages.json')
export default {
    data(){return{
        links
    }}
}
</script>

<style>

</style>