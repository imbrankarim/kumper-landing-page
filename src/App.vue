<template>
  <v-app>
    <v-main class="background-apps">
      <div class="mt-16"></div>
      <v-row align="center">
        <v-col cols="12" sm="12" md="12" lg="7">
          <p class="title-apps font-weight-black ml-16 mr-16">
            Kumpulan Peraturan
          </p>
          <p class="desc-apps ml-16 mr-16">
            Aplikasi kumpulan peraturan terlengkap di Indonesia, cari aplikasi,
            pilih, unduh dan bagikan koleksi peraturan langsung dari aplikasi.
          </p>
          <!-- <div class="mt-8"></div> -->
          <v-img
            class="ml-12 mr-12"
            style="cursor: pointer"
            max-width="270px"
            @click="openStore()"
            :src="require('./assets/badge.png')"
          ></v-img>
        </v-col>
        <v-col cols="12" sm="12" md="12" lg="5" align="center">
          <!-- <v-img
            class="ml-16 mr-16"
            contain
            max-width="700px"
            :src="require('./assets/apps.png')"
          ></v-img> -->
          <v-carousel hide-delimiters show-arrows-on-hover cycle>
            <v-carousel-item>
              <v-img
                contain
                max-width="270px"
                :src="require('./assets/home.png')"
              ></v-img>
            </v-carousel-item>
            <v-carousel-item>
              <v-img
                contain
                max-width="270px"
                :src="require('./assets/peraturan.png')"
              ></v-img>
            </v-carousel-item>
            <v-carousel-item>
              <v-img
                contain
                max-width="270px"
                :src="require('./assets/detail.png')"
              ></v-img>
            </v-carousel-item>
          </v-carousel>
        </v-col>
      </v-row>
      <v-row class="ma-16">
        <v-spacer></v-spacer>
        <v-col cols="12" sm="4" md="3" lg="3">
          <v-card dark>
            <v-card-title>Beranda</v-card-title>
            <v-divider></v-divider>
            <v-list>
              <v-list-item>
                <v-list-item-content> Peraturan Terbaru </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content> Kategori Terbaru </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content> Instansi Peraturan </v-list-item-content>
              </v-list-item>
            </v-list>
          </v-card>
        </v-col>
        <v-col cols="12" sm="4" md="3" lg="3">
          <v-card dark>
            <v-card-title>Peraturan</v-card-title>
            <v-divider></v-divider>
            <v-list>
              <v-list-item>
                <v-list-item-content> Daftar Peraturan </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content> Pencarian Peraturan </v-list-item-content>
              </v-list-item>
            </v-list>
          </v-card>
        </v-col>
        <v-col cols="12" sm="4" md="3" lg="3">
          <v-card dark>
            <v-card-title>Detail</v-card-title>
            <v-divider></v-divider>
            <v-list>
              <v-list-item>
                <v-list-item-content> Detail Peraturan </v-list-item-content>
              </v-list-item>
              <v-list-item>
                <v-list-item-content> Unduh Peraturan </v-list-item-content>
              </v-list-item>
            </v-list>
          </v-card>
        </v-col>
        <v-spacer></v-spacer>
      </v-row>
      <div class="mb-16"></div>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  methods: {
    openStore() {
      window.open(
        "https://play.google.com/store/apps/details?id=com.nanolite.kumper",
        "_blank "
      );
    },
  },
};
</script>

<style scoped>
.title-apps {
  font-size: 5rem;
  font-family: cursive;
}
.desc-apps {
  font-size: 2.5rem;
}
.background-apps {
  background-image: url("./assets/background.jpg");
  background-size: cover;
}
</style>
