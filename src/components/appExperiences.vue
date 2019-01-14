<template>
  <v-flex xs12 md5 offset-md2>
    <div v-for="experience in experiences" :key="experience.id">
      <v-card class="my-3" hover>
          <v-container fill-height fluid>
            <v-layout>
              <v-flex xs5>
                  <v-img
                    :src="require(`../assets/places/${experience.logo}`)"
                    height="125px"
                    width="125px"
                    contain
                  ></v-img>
              </v-flex>
              <v-flex xs12 align-end d-flex>
                <span class="headline">{{ experience.at }}</span><br />
                <span class="title">{{ experience.position }}</span>
              </v-flex>
            </v-layout>
          </v-container>
        <v-card-text>
          {{ experience.description }}
        </v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn flat class="blue--text">Read More</v-btn>
        </v-card-actions>
      </v-card>
    </div>
  </v-flex>
</template>

<script>
export default {
  data: () => ({
    experiences: [
      {
        id: 0,
        at: 'Gerenciarme',
        position: 'Front-end Developer',
        start: '2016-01-09T02:00:00.000Z',
        end: '2017-01-03T02:00:00.000Z',
        description: 'My first experience as a developer. Learned a lot with my mentor (and boss), Davi Arimatéia. Worked with a lot of Javascript, HTML and CSS. It was the first time I had to make API calls, learn about data-flows and good code practices.',
        logo: 'gerenciarme.png',
        technologies: [
          'knockout',
          'html',
          'css'
        ]
      },
      {
        id: 1,
        at: 'IBM - Marketing Services Group',
        position: 'Fullstack',
        start: '2017-01-03T02:00:00.000Z',
        end: '2017-01-11T02:00:00.000Z',
        description: 'On my brief passage through IBM, I learned a lot. I was responsible for the maintanence of IBM pages world-wide (mainly in Latin America). IBM was my chance to really learn to code. In there I made friends that taught me unvaluable concepts, testing, design patterns, project management and agile culture. I was very lucky to work on IBM on that especific period of time, because IBM was transforming itself, applying agile culture and encouraging all teams to adopt. As a result, I had tons of courses, free and quality material for study, needless to say, also experience.',
        logo: 'ibm.png',
        technologies: [
          'vue',
          'html',
          'css',
          'node',
          'mongo',
          'mithril'
        ]
      },
      {
        id: 2,
        at: 'Boxnet',
        position: 'Fullstack',
        start: '2017-01-11T02:00:00.000Z',
        end: '2018-01-09T02:00:00.000Z',
        description: 'Boxnet was a mid-sized midia monitoring bussines. When I entered there, all of their systems were build with AngularJS(1.6), and... we had technologies like React, Vue, Angular (2+) that were blowing, so I suggested to update all systems to Vue. And I did it. It was a very hard time, but it was very rewarding. After sometime in there, they asked for a nodejs microservice, for a URL generation (and invalidation, to secure the data we sent to our clients). It was VERY hard, coming from a full front-end background, I learned a lot and even used technologies like docker, running clusters on Amazons ECS and storaging data with S3',
        logo: 'boxnet.jpeg',
        technologies: [
          'angularjs',
          'vue',
          'node',
          'sqlserver',
          'aws',
          'docker'
        ]
      },
      {
        id: 3,
        at: 'Loopix',
        position: 'Back-end Developer',
        start: '2017-01-11T02:00:00.000Z',
        end: false,
        description: "On my current job, I'm the responsible for the development of Loopix's new app Back-end. I'm very glad to work on this project and having contact with various APIs, Push notification, SMS, e-mail, recurrent and single payments... Its been a very fun ride. Hope to see what is the next thing I'll have to grasp to bring it into the app. Currently I'm using EC2 machines in Amazon, but I plan to move it to docker containers in the future :)",
        logo: 'loopix.png',
        technologies: [
          'node',
          'mongo',
          'aws'
        ]
      }
    ]
  })
}
</script>

<style>

</style>
