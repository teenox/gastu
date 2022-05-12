<template>
  <div class="banner-wrapper" :style="image">
    <v-container>
      <!-- -----------------------------------------------
            Start Banner
        ----------------------------------------------- -->
      <v-row justify="center">
        <v-col cols="12" md="7" lg="6" class="d-flex align-center">
          <Search />
        </v-col>
        <v-col cols="12" md="5" lg="6">
          
        </v-col>
      </v-row>

      <!-- -----------------------------------------------
            End Banner
        ----------------------------------------------- -->
    </v-container>
  </div>
</template>
<script>
import homeImg from "assets/images/banner/home-image.jpg"
export default {
  name: "Banner",
  data() {
    return {
      image: { backgroundImage: `url(${homeImg})` },
    };
  },
  components: {
    Search: () => import("@/components/custom/search/Search")
  }
};
</script>

<style lang="scss" scoped>
  .banner-wrapper {
    margin-bottom: 150px
  }
</style>