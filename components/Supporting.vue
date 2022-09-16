<template>
  <v-container>
    <v-row justify="center">
        <v-col cols="12">
            <h2 class="supporting-title pt-12 mt-12">Supporting the child care ecosystem is complex,<br />that’s why we offer integrated solutions for<br />everyone involved.</h2>
        </v-col>
        <v-col cols="4" v-for="(section, i) in sections" :key="i">
            <v-row justify="center">
                <v-col class="shrink">
                    <v-img height="150px" width="150px" :src="section.image" />
                </v-col>
                <v-col cols="12">
                    <h4 class="section-title">{{section.title}}</h4>
                </v-col>
                <v-col cols="12">
                    <p class="section-paragraph">{{section.text}}</p>
                </v-col>
            </v-row>
        </v-col>
        <v-col cols="12" class="py-12" />
        <v-col cols="6">
            <v-img src="https://uploads-ssl.webflow.com/5f6ce074a62cf885680ba383/614c8f4de9b3331612b208fc_Family%20illustration.svg" />
        </v-col>
        <v-col cols="6" class="stats-col">
            <v-row class="stats-row" align="center" justify="center">
                <v-col class="shrink">
                    <h5>270+</h5> <br />
                    <span>Counties Using Bridgecare</span>
                </v-col>
                <v-col class="shrink">
                    <h5>270+</h5> <br />
                    <span>Counties Using Bridgecare</span>
                </v-col>
                <v-col class="shrink">
                    <h5>270+</h5> <br />
                    <span>Counties Using Bridgecare</span>
                </v-col>
            </v-row>
        </v-col>
        <v-col cols="12" class="py-12" />
    </v-row>
  </v-container>
</template>

<script>
export default {
    data(){return{
        sections: [
            {
                title: "Family Portal",
                image: "https://uploads-ssl.webflow.com/5f6ce074a62cf885680ba383/5f87ae0ff7e6832bd96527fd_Organization.png",
                text: "Connect local families with available child care openings and available subsidy programs."
            },
            {
                title: "Provider Portal",
                image: "https://uploads-ssl.webflow.com/5f6ce074a62cf885680ba383/5f87ae0fbc0d53dd2445d93a_Employer.png",
                text: "Allow providers to market their programs, manage enrollment, and maintain licensing status."
            },
            {
                title: "Admin Portal",
                image: "https://uploads-ssl.webflow.com/5f6ce074a62cf885680ba383/5f87ae0f381022e81d6f9e43_Government.png",
                text: "Use real-time data including supply and demand to make more effective policy and resource decisions."
            }
        ]
    }}
}
</script>

<style lang="scss">
.supporting-title{
    display: inline-block;
    width: 100%;
    text-align: center;
    font-size: 2em;
    font-weight: 500;
}
.section-title{
    font-size: 1.75em;
    text-align: center;
    line-height: 1;
}
.section-paragraph{
    text-align: center;
    font-weight: 300;
    font-size: 1.15em;
    padding: 0 20px;
}
.stats-col{
    background-color: #205c6f;
    border-radius: 25px;
    .stats-row{
        height: 100%;
    }
}
</style>