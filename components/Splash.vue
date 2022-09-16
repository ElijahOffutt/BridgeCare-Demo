<template>
  <div class="splash">
    <v-row justify="center">
        <v-col class="8">
            <h2>Child care data and the technology solutions for governmenmt agencies.</h2>
            <p>We’re a team of user experience driven technologists. We listen to our stakeholders, involve them in our design process, and are quick to react to changes. Ready for modern integrated technology?</p>
            <v-btn x-large right rounded>
                <span >request demo</span>
                <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
        </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  props: ['type', 'content'],
  computed: {
    Height () {
      return 'some height for now'
    }
  }
}
</script>

<style lang="scss" scoped>
.splash{
    padding: 200px 0;
    position: relative;
}
</style>