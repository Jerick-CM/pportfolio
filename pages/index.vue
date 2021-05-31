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
    <v-sheet min-height="30vh" class="white">
      <v-container class="">
        <v-row no-gutters class="mt-5">
          <v-col cols="12" sm="12" lg="12">
            <v-layout justify-center align-center>
              <v-avatar color="primary" size="375" class="text-center">
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
            <p for="" class="fs-1-1 white--text text-justify">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Vestibulum in tellus consequat, faucibus massa quis, tempor
              tortor. Ut gravida nulla ante, nec mattis orci molestie in. Nunc
              iaculis eget mi eu elementum. Nam in luctus purus. Curabitur ut
              purus convallis, rhoncus metus porta, tempus risus. Cras semper
              ultrices massa, a tempus ante congue ut. Donec cursus semper
              placerat. Quisque luctus, enim vel suscipit fermentum, arcu quam
              ultricies ligula, id rutrum urna enim eu justo. Fusce venenatis
              fringilla turpis. Etiam nec quam arcu. Mauris eleifend turpis a
              condimentum dictum. Donec quis urna eu tortor efficitur semper non
              non ex. Nulla interdum aliquet tortor, eu vulputate lectus
              molestie eget. Nulla a purus nec nulla interdum vehicula in
              tincidunt purus. Ut ullamcorper, odio vitae egestas laoreet, augue
              nibh condimentum quam, eu finibus erat magna non metus. Nullam
              fringilla feugiat ante, et semper tellus luctus sed. Nam nisl
              erat, pulvinar vitae sem ac, scelerisque pulvinar justo.
              Pellentesque vitae dui enim. In hac habitasse platea dictumst.
              Pellentesque porta velit et leo vehicula, sit amet dictum lorem
              tincidunt. Morbi mollis leo odio, et iaculis dui pretium ac. In
              sit amet eros ut diam sodales ullamcorper sit amet quis tellus.
              Sed eget aliquet erat. Pellentesque eget ipsum velit. Pellentesque
              iaculis nisi id eleifend mattis. Sed accumsan mollis eleifend.
              Aliquam sit amet lectus bibendum, lacinia metus quis, bibendum
              diam. Praesent odio sem, bibendum non porta quis, hendrerit nec
              elit. Quisque eget arcu nulla. In vestibulum mauris vitae eros
              semper, id dapibus metus feugiat. Aliquam ornare, sapien at
              feugiat facilisis, libero nisi semper urna, quis porttitor nunc
              sem in justo. Etiam at sapien accumsan, convallis ligula ac,
              ultrices orci. Nunc iaculis nibh ipsum, at varius magna feugiat
              quis.
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
            <p for="" class="fs-1-1 white--text text-justify">
              Internet is the world audience.
            </p>
            <p for="" class="fs-1-1 white--text text-justify">
              Donec scelerisque eros vel tellus tempor, quis iaculis orci
              ultrices.
            </p>
            <p for="" class="fs-1-1 white--text text-justify">
              Nunc volutpat nisi quis ligula congue, vitae eleifend risus
              interdum.
            </p>
            <p for="" class="fs-1-1 white--text text-justify">
              Curabitur quis ligula malesuada, ornare quam eget, interdum felis.
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
img {
  height: 100vh;
}
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
