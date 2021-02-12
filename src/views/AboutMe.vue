<template>
  <v-container>
    <v-row>
      <v-col
        cols="6"
      >
        <Info/>
      </v-col>
      <v-col
        cols="6"
      >
        <Photo/>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import Photo from "@/components/aboutme/Photo.vue"
import Info from "@/components/aboutme/Info.vue"


export default {
  name:'AboutMe',
  components: {
    Photo,
    Info
  }

}
</script>

<style>

</style>