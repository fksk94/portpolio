<template>
  <div class="text-center">
    <v-icon
      style="position:fixed; left:30px; top:45%;"
      size="60px"
      color="#444444"
      class="event-back-button-hover"
      @click="gotoMain"
    >
      mdi-arrow-left-bold-box-outline
    </v-icon>
    <v-container>
      <v-row justify="center">
        <v-col cols="8">
          <v-container class="max-width">
            <NUVO
              v-if="page == 1"
            />
            <KGBros
              v-if="page == 2"
            />
            <Thesis
              v-if="page == 3"
            />
            <Network
              v-if="page == 4"
            />
            <FlowChart
              v-if="page == 5"
            />
            <RNCRUD
              v-if="page == 6"
            />
            <v-pagination
              v-model="page"
              class="my-4"
              :length="6"
              color="#17d5a7"
            ></v-pagination>
          </v-container>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import FlowChart from "@/components/projects/FlowChart.vue"
import Network from "@/components/projects/Network.vue"
import NUVO from "@/components/projects/NUVO.vue"
import KGBros from "@/components/projects/KGBros.vue"
import RNCRUD from "@/components/projects/RNCRUD.vue"
import Thesis from "@/components/projects/Thesis.vue"

export default {
  name:'Projects',
  components: {
    FlowChart,
    Network,
    NUVO,
    KGBros,
    RNCRUD,
    Thesis
  },
  data: function () {
    return {
      page: 1,
    }
  },
  methods: {
    gotoMain: function () {
      this.$router.push({name:"Home"})
    }
  }
}
</script>

<style scoped>

.event-back-button-hover:hover {
  transition: 0.45s;
  transform: scale(1.1);
  color:#17d5a7 !important;
  cursor: pointer;
}

</style>