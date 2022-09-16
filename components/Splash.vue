<template>
  <div class="splash">
    <v-container class="content">
      <v-row style="height: 100%;" justify="start" align="center">
          <v-col cols="8">
              <h2>Child care data and the technology solutions for governmenmt agencies.</h2>
              <p class="my-10">We’re a team of user experience driven technologists. We listen to our stakeholders, involve them in our design process, and are quick to react to changes. Ready for modern integrated technology?</p>
              <v-btn @click="$router.push('/request-a-demo')" color="secondary" x-large right rounded>
                  <span style="text-transform: capitalize;" class="mr-12">request demo</span>
                  <v-icon right>mdi-arrow-right</v-icon>
              </v-btn>
          </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<style lang="scss" scoped>
.splash{
    position: relative;
    background-color: #38beb5;
    position: relative;
    height: 70vh;
    .content{
      height: 100%;
      z-index: 1;
      position: relative;
      color: white;
      h2{
        font-size: 3.25em;
      }
      p{
        font-size: 1.5em;
      }
    }
    &::before{
      pointer-events: none;
      top: 0;
      left: 0;
      float: left;
      content: "";
      height: 100%;
      width: 100%;
      z-index: 0;
      display: block;
      position: absolute;
      background-image: url('https://uploads-ssl.webflow.com/5f6ce074a62cf885680ba383/5f878ed94033fde0ec6c5936_Background%20Layer%20(1).png');
      opacity: .25;
    }
    &::after{
      pointer-events: none;
      top: 0;
      left: 0;
      float: left;
      content: "";
      height: 100%;
      width: 100%;
      z-index: 0;
      display: block;
      position: absolute;
      background-image: url('https://uploads-ssl.webflow.com/5f6ce074a62cf885680ba383/609f183e753ed49b9eb896d9_ILLUSTRATION%20(6).png');
      background-size: contain;
      background-position: right center;
    }
}
</style>