<template>
  <v-container
    style="width:100%; height:100%;"
  >
    <v-icon
      style="position:fixed; left:30px; top:45%;"
      size="60px"
      color="#444444"
      class="event-back-button-hover"
      @click="gotoMain"
    >
      mdi-arrow-left-bold-box-outline
    </v-icon>
    <v-row
      style="width:100%; height:100%;"
    >
      <v-col
        cols="6"
        style="width:100%; height:100%;"
      >
        <Info/>
      </v-col>
      <v-col
        cols="6"
        style="width:100%; height:100%;"
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