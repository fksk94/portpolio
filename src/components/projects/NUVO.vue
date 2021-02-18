<template>
  <div>
    <v-row>
      <v-col
        cols="12"
      >
        <ProjectTitle
          :projectTitle = "projectTitle"
        />
      </v-col>
    </v-row>
    <v-row style="margin-top:25px;">
        <v-col
        cols="6"
      >
        <Info/>
      </v-col>
      <v-col
        cols="6"
      >
        프로젝트 사진
      </v-col>
    </v-row>
  </div>
</template>

<script>
import ProjectTitle from "@/components/projects/entity/Title.vue"
import Info from "@/components/nuvo/Info.vue"


export default {
  name:"NUVO",
  data: function () {
    return {
      projectTitle: "N U V O",
    }
  },
  components: {
    Info,
    ProjectTitle,
  }

}
</script>

<style>

</style>