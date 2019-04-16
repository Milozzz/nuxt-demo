<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
      xs12
      sm8
      md6
    >
      <div class="text-xs-center">
        <h1>firstName</h1>
        <h1>lastName</h1>
        <h1>number</h1>
      </div>
    </v-flex>
  </v-layout>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    VuetifyLogo
  },
  mounted() {
    console.log(this.$route)
  },
}
</script>
<style>
  .text-xs-center{
    margin-top:200px;
  }
</style>
