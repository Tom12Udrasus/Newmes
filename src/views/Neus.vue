<template>
  <v-card class="mx-auto" max-width="1000">
    <!-- <v-system-bar color="indigo darken-2" dark>
      <v-spacer></v-spacer>

      <v-icon>mdi-window-minimize</v-icon>

      <v-icon>mdi-window-maximize</v-icon>

      <v-icon>mdi-close</v-icon>
    </v-system-bar>-->

    <v-toolbar  dark>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <!-- <v-toolbar-title>Discover</v-toolbar-title> -->

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
    </v-toolbar>

    <v-container fluid>
      <v-row dense>
        <v-col v-for="card in cards" :key="card.title" :cols="card.flex">
          <v-card>
            <v-img
              :src="card.src"
              class="white--text align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="400px"
            >
              <v-card-title v-text="card.title"></v-card-title>
            </v-img>

            <v-card-actions>
              <v-spacer></v-spacer>

              <v-btn icon>
                <v-icon>mdi-heart</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-bookmark</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-share-variant</v-icon>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid>
      <v-row dense>
        <v-col v-for="card in cards1" :key="card.title" :cols="card.flex">
          <v-card>
            <v-img
              :src="card.src"
              class="white--text align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="400px"
            >
              <v-card-title v-text="card.title"></v-card-title>
            </v-img>

            <v-card-actions>
              <v-spacer></v-spacer>

              <v-btn icon>
                <v-icon>mdi-heart</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-bookmark</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-share-variant</v-icon>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <v-container fluid>
      <v-row dense>
        <v-col v-for="card in cards2" :key="card.title" :cols="card.flex">
          <v-card>
            <v-img
              :src="card.src"
              class="white--text align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="400px"
            >
              <v-card-title v-text="card.title"></v-card-title>
            </v-img>

            <v-card-actions>
              <v-spacer></v-spacer>

              <v-btn icon>
                <v-icon>mdi-heart</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-bookmark</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-share-variant</v-icon>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid>
      <v-row dense>
        <v-col v-for="card in cards3" :key="card.title" :cols="card.flex">
          <v-card>
            <v-img
              :src="card.src"
              class="white--text align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="400px"
            >
              <v-card-title v-text="card.title"></v-card-title>
            </v-img>

            <v-card-actions>
              <v-spacer></v-spacer>

              <v-btn icon>
                <v-icon>mdi-heart</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-bookmark</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-share-variant</v-icon>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-card>
</template>

<script>
export default {
  data: () => ({
    cards: [
      {
        title: "Pre-fab homes",
        src: "https://cdn.vuetifyjs.com/images/cards/house.jpg",
        flex: 12
      },
      {
        title: "Favorite road trips",
        src: "https://cdn.vuetifyjs.com/images/cards/road.jpg",
        flex: 6
      },
      {
        title: "Best airlines",
        src: "https://cdn.vuetifyjs.com/images/cards/plane.jpg",
        flex: 6
      }
    ],
    cards1: [
      {
        title: "Pre-fab homes",
        src: "http://msuedu.ru/u/526/Mess/1031108455.jpg",
        flex: 12
      },
      {
        title: "Favorite road trips",
        src:
          "https://top15moscow.ru/storage/news/August2018/6z2DFAq93vMjTkzfVT7T.jpg",
        flex: 6
      },
      {
        title: "Best airlines",
        src:
          "https://i.pinimg.com/originals/dc/6e/27/dc6e2719cb75207df1ba4968389951c9.jpg",
        flex: 6
      }
    ],
    cards2: [
      {
        title: "Pre-fab homes",
        src:
          "https://www.rosphoto.com/images/u/articles/1406/4_svetlana_shupenko.jpg",
        flex: 12
      },
      {
        title: "Favorite road trips",
        src:
          "https://lubimova-sun.com/wp-content/uploads/2019/12/3D-3d-papel-parede.jpg",
        flex: 6
      },
      {
        title: "Best airlines",
        src:
          "https://i.pinimg.com/originals/8e/29/ee/8e29ee3e29c69748a6b1c87b3c7a4bdd.jpg",
        flex: 6
      }
    ],
    cards3: [
      {
        title: "Pre-fab homes",
        src: "https://voka.me/wp-content/uploads/2017/05/11-1.jpg",
        flex: 12
      },
      {
        title: "Favorite road trips",
        src: "https://i.ytimg.com/vi/E4jCiHztpMM/maxresdefault.jpg",
        flex: 6
      },
      {
        title: "Best airlines",
        src:
          "https://images11.cosmopolitan.ru/upload/custom/f44/f44dd98b716091b640ec54736bc4fada.jpg",
        flex: 6
      }
    ]
  })
};
</script>