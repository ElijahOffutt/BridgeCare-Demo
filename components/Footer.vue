<template>
  <v-footer style="background-color: #f9f9f9;" class="py-10">
    <v-container class="Footer">
        <v-row>
            <v-col cols="3">
                <h3>Support</h3>
                <a href="">Request a Demo</a>
                <a href="">Contact Us</a>
            </v-col>
            <v-col cols="3">
                <h3>for providers &amp; families</h3>
                <a href="">Interested in using BridgeCare in your community? Let us know</a>
            </v-col>
            <v-spacer />
            <v-col class="grow">
                <img @click="$router.push('/')" style="cursor: pointer;" src="https://uploads-ssl.webflow.com/5f6ce074a62cf885680ba383/5f8a5d5c39466ae063c674c5_bridgecare%20logo_color.svg" loading="lazy" alt="BridgeCare logo" height="40px">
                <a href="">Privacy Policy</a>
                <a href="">Terms of Service</a>
                <span style="opacity: .35;">Copyright &copy; 2022 All rights reserved</span>
            </v-col>
        </v-row>
    </v-container>
  </v-footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.Footer{
    h3{
        margin-bottom: 20px;
        text-transform: capitalize;
    }
    a{
        display: inline-block;
        width: 100%;
        color: black;
        text-decoration: none;
    }
    .last{
        text-align: right;
        white-space: nowrap;
    }
}
</style>