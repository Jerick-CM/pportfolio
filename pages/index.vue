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
              >[ Technology R&D ]
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
    <v-sheet min-height="30vh" class="white">
      <v-container class="">
        <v-row no-gutters class="mt-5">
          <v-col cols="12" sm="12" lg="12">
            <v-layout justify-center align-center>
              <v-avatar
                :size="150"
                class="text-center black"
                v-if="$vuetify.breakpoint.smAndDown"
              >
                <v-img
                  class="text-center"
                  src="/images/cartoon-darken.jpg"
                ></v-img>
              </v-avatar>

              <v-avatar :size="350" class="text-center black" v-else>
                <v-img
                  class="text-center"
                  src="/images/cartoon-darken.jpg"
                ></v-img>
              </v-avatar> </v-layout
          ></v-col>
        </v-row>
        <v-row no-gutters class="mt-5">
          <v-col
            cols="12"
            sm="12"
            lg="12"
            class="font-avenir fs-1-4 text-justify grey--text"
          >
            What is dark in programming is, when you get and successfully fix
            and build something you are happy, but if get too long to do your
            plany the frustration builds up.
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>

    <v-sheet min-height="30vh" class="grey">
      <v-container class="">
        <v-row no-gutters class="mt-5">
          <v-col cols="12" sm="12" lg="12">
            <p
              for=""
              class="fs-1-1 white--text text-justify"
              v-for="(item, i) in para"
              :key="i"
            >
              {{ item.phrase }}
            </p>
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>
    <v-sheet min-height="30vh" class="white">
      <v-container class="">
        <v-row no-gutters class="mt-5">
          <v-col cols="12" sm="12" lg="12">
            <p for="" class="fs-1-1 text-center grey--text">
              Learn more, get involved, and take action!
            </p>
          </v-col>
        </v-row>
        <v-row no-gutters class="mt-5">
          <v-col cols="12" sm="12" lg="12" class="text-center">
            <v-btn class="font-avenir">Join the movement</v-btn>
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>

    <v-sheet min-height="30vh" class="blue">
      <v-container class="">
        <v-row no-gutters class="mt-5">
          <v-col cols="12" sm="12" lg="4">
            <v-layout justify-center align-center>
              <v-avatar color="primary" size="150" class="text-center">
                <v-img class="text-center" src="/images/box.png"></v-img>
              </v-avatar>
            </v-layout>
          </v-col>
          <v-col cols="12" sm="12" lg="8">
            <p
              for=""
              class="fs-1-1 white--text text-justify"
              v-for="(item, i) in quotes"
              :key="i"
            >
              {{ item.phrase }}
            </p>
          </v-col>
        </v-row>
        <v-row no-gutters class="mt-5">
          <v-col cols="12" sm="12" lg="12" class="text-center"> </v-col>
        </v-row> </v-container
    ></v-sheet>

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
    para: [
      {
        phrase:
          'Developers evolve all the time. That a simple work of repetition is not possible.',
      },
      { phrase: 'Life is always a battle of resolve. ' },
      { phrase: 'Big brains with no life ORGATE No brains with slack life. ' },
      {
        phrase:
          'Nobody warns the world community that passwords cannot be used the same for every website you register, using the same password for sites you trust makes you become vulnerable from being hacked.',
      },
      {
        phrase:
          "Raise your hand if you've been coding while waiting or just listening to a movie or tv series.",
      },
      {
        phrase:
          'start sitting at what you need to  code the hardest part is bringing oneself to do it.',
      },
      { phrase: 'Maybe the only way to get good is practice.' },
    ],
    quotes: [
      {
        phrase: 'Nothing ever go smoothly at the first time with programming.',
      },
      { phrase: 'Hard work is the sum of daily efforts. ' },
      { phrase: 'Strength is built in weakness.  - sand chronicles.' },
      {
        phrase:
          "Don't fight what we hate, save what we love  - star wars the last jedi. ",
      },
      { phrase: "Knowledge isn't always power, sometimes it is a burden ." },
      { phrase: 'The future is Open.' },
      { phrase: 'Faith in others is often misplaced.' },
      {
        phrase:
          'In web development it really necessary to learn from the best.',
      },
      {
        phrase: ' Internet is the world audience.',
      },
    ],
    selectedItem: 0,

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
/* img {
  height: 100vh;
} */
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
