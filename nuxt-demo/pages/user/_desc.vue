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
        <h1 v-if='desc[0]'>firstName: {{desc[0].substring(0,1).toUpperCase()+desc[0].substring(1)}}</h1>
        <h1 v-if='desc[0]'>lastName: {{desc[1].substring(0,1).toUpperCase()+desc[1].substring(1)}}</h1>
        <h1>user id: {{desc[2]}}</h1>
      </div>
    </v-flex>
  </v-layout>
</template>

<script>

// get the router information

export default {
  data(){
    return{
      desc:[]
    }
  },
  components: {
  },
  mounted() {
    this.desc=this.$route.params.desc.split("-") // split with "-" and get name and id
  },
}
</script>
<style>
.text-xs-center{
  margin-top:200px;
}
</style>
