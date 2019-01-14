<template>
  <v-flex xs12 md4>
    <div class="text-xs-center">
      <v-avatar size="125px">
        <img
          class="img-circle elevation-7 mb-1"
          :src="require('../assets/perfil.jpg')"
        >
      </v-avatar>
      <div class="headline">Matheus <span style="font-weight:bold">Fonseca</span></div>
      <div class="subheading text-xs-center grey--text pt-1 pb-3">Fullstack Developer</div>
      <v-layout justify-space-between>
        <a href="javascript:;" class="body-2">Home</a>
        <a href="javascript:;" class="body-2">Previous Experiences</a>
        <a href="javascript:;" class="body-2">Github</a>
        <a href="javascript:;" class="body-2">Contact me</a>
      </v-layout>
    </div>
  </v-flex>
</template>

<script>
export default {
  data: () => ({

  })
}
</script>

<style>

</style>
