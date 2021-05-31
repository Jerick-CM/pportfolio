<template>
  <v-container class="red pa-0 ma-0" fluid no-gutters>
    <v-sheet min-height="" class="black">
      <v-container class=""
        ><v-row no-gutters>
          <v-col cols="12" sm="12" lg="9" class="text-center"
            ><label
              class="font-lulu white--text"
              :class="{
                'fs-1.1': $vuetify.breakpoint.smAndDown,
                'fs-3': $vuetify.breakpoint.mdAndUp,
              }"
              >JERICK C. MANGALUS</label
            >
          </v-col>
          <v-col cols="12" sm="12" lg="3" class="text-center mt-7"
            ><label
              class="text-right white--text"
              :class="{
                'fs-0-5': $vuetify.breakpoint.smAndDown,
                'fs-1-0': $vuetify.breakpoint.mdAndUp,
              }"
              >[ Center for Humane Technology ]
            </label>
          </v-col>
        </v-row>

        <v-row>
          <v-spacer class=""> </v-spacer>
          <v-col md="10" lg="8">
            <v-btn
              class="hidden-sm-and-down white--text"
              v-for="link in links"
              :key="link.label"
              text
            >
              {{ link.label }}
            </v-btn>

            <v-card class="mx-auto hidden-md-and-up" tile>
              <v-list dense>
                <v-list-item-group v-model="selectedItem" color="primary">
                  <v-list-item v-for="(item, i) in links" :key="i">

                    <v-list-item-content>
                      <v-list-item-title
                        v-text="item.label"
                      ></v-list-item-title>
                    </v-list-item-content>
                  </v-list-item>
                </v-list-item-group>
              </v-list>
            </v-card>
          </v-col>
          <v-spacer class=""></v-spacer>
        </v-row>
      </v-container>
    </v-sheet>
    <v-sheet min-height="30vh" class="white"> </v-sheet>
    <v-sheet min-height="30vh" class="grey"> </v-sheet>
    <v-sheet min-height="30vh" class="white"> </v-sheet>
    <v-sheet min-height="30vh" class="blue"> </v-sheet>
    <v-sheet min-height="" class="black">
      <v-container class="">
        <v-row>
          <v-spacer class=""> </v-spacer>
          <v-col md="10" lg="8">
            <v-btn
              class="hidden-sm-and-down white--text"
              v-for="link in links"
              :key="link.label"
              text
            >
              {{ link.label }}
            </v-btn>

            <v-card class="mx-auto hidden-md-and-up" tile>
              <v-list dense>
                <v-list-item-group v-model="selectedItem" color="primary">
                  <v-list-item v-for="(item, i) in links" :key="i">
                    <v-list-item-content>
                      <v-list-item-title
                        v-text="item.label"
                      ></v-list-item-title>
                    </v-list-item-content>
                  </v-list-item>
                </v-list-item-group>
              </v-list>
            </v-card>
          </v-col>
          <v-spacer class=""></v-spacer>
        </v-row>
      </v-container>
    </v-sheet>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    selectedItem: 1,
    items: [
      { text: 'Real-Time', icon: 'mdi-clock' },
      { text: 'Audience', icon: 'mdi-account' },
      { text: 'Conversions', icon: 'mdi-flag' },
    ],
    links: [
      { label: 'ABOUT' },
      { label: 'MEDIA' },
      { label: 'PODCAST' },
      { label: 'DOCUMENTARY' },
      { label: 'CONTACT' },
      { label: 'JOIN THE MOVEMENT' },
    ],

    model: 6,
    rounded: ['0', 'sm', 'md', 'lg', 'xl', 'pill', 'circle'],
  }),
  computed: {
    radius() {
      let rounded = 'rounded'
      const value = this.rounded[this.model]

      if (value !== 'md') {
        rounded += `-${value}`
      }

      return rounded
    },
  },
}
</script>

<style lang="scss" scoped>
.no-background-hover::before {
  background-color: transparent !important;
}
</style>
<style scoped>
.text-justify {
  text-align: justify;
  text-justify: inter-word;
}
.name {
  font-family: 'Lulu', sans-serif;
}
.font-lulu {
  font-family: 'Lulu', sans-serif;
}
.font-avenir {
  font-family: 'Avenir', sans-serif;
}

.ff-a {
  font-family: Arial, Helvetica, sans-serif;
}
.v-slide-group__content.v-tabs-bar__content {
  background-color: black !important;
}
.v-slide-group__content.v-tabs-bar__content {
  background-color: black;
}
.img-container {
  text-align: center;
  display: block;
}
</style>
