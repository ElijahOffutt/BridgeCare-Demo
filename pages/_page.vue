<template>
    <div class="page-wrap">
        <div class="page">
            <v-container>
                <v-row style="padding: 100px 0;" align="center" justify="center">
                    <v-col cols="6">
                        <h2>{{content.text}}</h2>
                        <p>{{content.content}}</p>
                        <ul>
                            <li v-for="(bullet, b) in content.bulletPoints" :key="b">{{bullet}}</li>
                        </ul>
                        <v-btn @click="$router.push('/request-a-demo')" class="mt-10" x-large flat rounded color="primary">
                            <span style="text-transform: capitalize;" class="mr-12">Learn More</span>
                            <v-icon>mdi-arrow-right</v-icon>
                        </v-btn>
                    </v-col>
                    <v-col cols="6">
                        <v-img :src="content.image" />
                    </v-col>
                </v-row>
            </v-container>
        </div>
        <Browse />
    </div>
</template>

<script>
let Pages = require('/static/Pages.json')
export default {
    computed: {
        content () {
            return Pages.find(item => item.link.match(this.$route.params.page))
        }
    }
}
</script>

<style lang="scss">
.page{
    background-color: #205c6f;
    background-image: url('https://uploads-ssl.webflow.com/5f6ce074a62cf885680ba383/614c8c58a3b036707e4f9069_Decorative%20vector%20(1).svg');
    background-position: bottom left;
    background-size: cover;
    background-attachment: fixed;
    color: white;
    h2 {
        font-size: 2.5em;
        margin-bottom: 20px;
    }
    p{
        font-size: 1.25em;
    }
}
</style>