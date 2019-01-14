<template>
<v-app light>
    <v-content>
      <v-container>
        <v-layout row wrap>
          <app-profile></app-profile>
          <app-experiences></app-experiences>
        </v-layout>
      </v-container>
    </v-content>
    <v-footer class="secondary" app>
      <v-layout row wrap align-center>
        <v-flex xs12>
          <div class="white--text ml-3">
            Made by <a class="white--text" href="https://github.com/matheus510" target="_blank">Matheus Fonseca</a>
            with <a class="white--text" href="https://vuetifyjs.com" target="_blank">Vuetify</a>
          </div>
        </v-flex>
      </v-layout>
    </v-footer>
  </v-app>
</template>

<script>
import appExperiences from './components/appExperiences.vue'
import appProfile from './components/appProfile.vue'

export default {
  name: 'App',
  data () {
    return {
      title: 'Your Logo',
      posts: [
        {
          title: 'Fusce ullamcorper tellus',
          content: 'Fusce ullamcorper tellus sed maximus rutrum. Donec imperdiet ultrices maximus. Donec non tellus non neque pellentesque fermentum. Aenean in pellentesque urna.',
          imgUrl: 'https://raw.githubusercontent.com/vuetifyjs/docs/dev/static/doc-images/cards/drop.jpg'
        },
        {
          title: 'Donec vitae suscipit lectus, a luctus diam.',
          content: 'Donec vitae suscipit lectus, a luctus diam. Proin vitae felis gravida, lobortis massa sit amet, efficitur erat. Morbi vel ultrices nisi.',
          imgUrl: 'https://raw.githubusercontent.com/vuetifyjs/docs/dev/static/doc-images/cards/docks.jpg'
        },
        {
          title: 'Vestibulum condimentum quam',
          content: 'At sagittis sapien vulputate. Vivamus laoreet lacus id magna rutrum dapibus. Donec vel pellentesque arcu. Maecenas mollis odio tempus felis elementum commodo.',
          imgUrl: 'https://raw.githubusercontent.com/vuetifyjs/docs/dev/static/doc-images/cards/plane.jpg'
        }
      ]
    }
  },
  components: {
    appExperiences,
    appProfile
  }
}
</script>
