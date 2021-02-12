<template>
  <v-container class="home">
    <v-row style="height:30%;">
      <v-col
        cols=12
        class="home"
      >
        <div
          class="home d-flex justify-center align-center"
        >
        </div>
      </v-col>
    </v-row>
    <v-row style="height:20%;">
      <v-col
        cols=12
        class="semi-home"
      >
        <div
          class="adjust-semi-home d-flex justify-center align-center"
        >
          <span
            class="event-main-button-hover"
            @click="gotoProjectsPage"
          >
            Projects
          </span>
        </div>
      </v-col>
    </v-row>
    <v-row style="height:20%;">
      <v-col
        cols=12
        class="semi-home"
      >
        <div
          class="adjust-semi-home d-flex justify-center align-center"
        >
          <span
            class="event-main-button-hover"
            @click="gotoAboutMePage"
          >
            About me
          </span>
        </div>
      </v-col>
    </v-row>
    <div
      style="position:fixed; bottom:35px; right:40px; font-size:18px; cursor:default;"
    >
      Portpolio made by Taewan
    </div>
  </v-container>
</template>

<script>
export default {
  name: 'Home',
  methods: {
    gotoProjectsPage: function () {
      this.$router.push({name:"Projects"})
    },
    gotoAboutMePage: function () {
      this.$router.push({name:"AboutMe"})
    }
  }
}
</script>

<style scoped>
@font-face {
    font-family: 'KOTRA_BOLD-Bold';
    src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_20-10-21@1.1/KOTRA_BOLD-Bold.woff') format('woff');
    font-weight: normal;
    font-style: normal;
}


.adjust-semi-home {
  height:100%;
  width:100%;
}

.semi-home {
  height:100%;
  width:100%;
}

.home {
  height:100%;
  width:100%;
  font-family:'KOTRA_BOLD-Bold';
  font-size:60px;
}

.event-main-button-hover:hover {
  transition: 0.45s;
  transform: scale(1.1);
  color:#17d5a7;
  cursor: pointer;
}

</style>