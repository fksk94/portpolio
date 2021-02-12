<template>
  <v-container>
    <v-icon
      style="position:fixed; left:30px; top:45%;"
      size="60px"
      color="#444444"
      class="event-back-button-hover"
      @click="gotoMain"
    >
      mdi-arrow-left-bold-box-outline
    </v-icon>
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
  },
  methods: {
    gotoMain: function () {
      this.$router.push({name:"Home"})
    }
  }
}
</script>

<style>

</style>