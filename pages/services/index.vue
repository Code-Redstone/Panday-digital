<template>
    <v-app>
        <main class="MTM-150px">
            <v-sheet color="deep-purple darken-1">
                <v-container>
                    <v-row>
                        <v-col class=""  cols="12" sm="12" md="6" lg="6" xl="6" color="white">
                            <v-img
                            class="ma-auto"
                            max-width="600px"
                            max-height="600px"
                            :src="require(`~/assets/resources/SEO-Audit.png`)"
                            />
                        </v-col>
                        <v-col cols="12" sm="12" md="6" lg="6" xl="6" class="d-flex">
                            <div class="d-block ">
                                <h1 class="white--text darken-4   font-weight-bold py-5 text-xl-h2 text-lg-h3 text-md-h5 text-sm-h2">SEO Audit Services</h1>
                                <h1 class="white--text darken-4 font-weight-thin py-5 text-xl-h2 text-lg-h3 text-md-h5 text-sm-h2">Get a Full Audit With a Detailed Action Plan</h1>
                                <p class="white--text darken-4 font-weight-light text-xl-h5 text-lg-h5 text-md-subtitle-1 text-sm-h5">Our audit services are carefully evaluated for each component and include significant recommendations that are tailored to your business.</p><br>
                            </div>
                        </v-col>
                    </v-row>
                </v-container>
            </v-sheet>
        </main>
        <svg id="arched" style="background:#5E35B1; fill:#fff;transform: scale(-1); height:52px; scale:;" preserveAspectRatio="none" viewBox="0 0 1442 144" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="" d="M1442,14.287108 L682.266,129.122 C621.756612,138.267588 517.026832,143.977138 423.629338,144 L422.504016,144 C396.685569,143.99367 371.751899,143.551232 348.88,142.625 L0,128.495459 L0,0 L1442,0 L1442,14.287108 Z" id="Combined-Shape"></path> </svg>
        <main>
            <v-sheet class="" height="100%" width="100%">
                <BeOnTop/>
            </v-sheet>
        </main>
        <svg id="arched" style="background:#5E35B1; fill:#fff; height:52px; scale:;" preserveAspectRatio="none" viewBox="0 0 1442 144" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="" d="M1442,14.287108 L682.266,129.122 C621.756612,138.267588 517.026832,143.977138 423.629338,144 L422.504016,144 C396.685569,143.99367 371.751899,143.551232 348.88,142.625 L0,128.495459 L0,0 L1442,0 L1442,14.287108 Z" id="Combined-Shape"></path> </svg>
        <main >
            <v-sheet class="pb-16 pt-16" color="#5E35B1" height="100%" width="100%">
                <SearchEngine/>
            </v-sheet>
        </main>
        <svg id="arched" style="background:#5E35B1; fill:#fff; height:52px;transform: scaleY(-1)scaleX(1);" preserveAspectRatio="none" viewBox="0 0 1442 144" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="" d="M1442,14.287108 L682.266,129.122 C621.756612,138.267588 517.026832,143.977138 423.629338,144 L422.504016,144 C396.685569,143.99367 371.751899,143.551232 348.88,142.625 L0,128.495459 L0,0 L1442,0 L1442,14.287108 Z" id="Combined-Shape"></path> </svg>
        <v-main class="my-15">
            <div class="container">
                <v-row>
                    <v-col
                    cols="12"
                    >
                    <div class="Faq-title">
                        <h1 class="deep-purple--text darken-1 font-weight-regular text-xl-h2 text-lg-h3 text-md-h4 text-sm-h4">Frequently Asked Questions</h1>
                    </div>
                    </v-col>
                    <v-col cols="12">
                    <v-expansion-panels >
                        <v-expansion-panel
                        v-for="faq in faqs"
                        :key="faq.id"
                        >
                        <v-expansion-panel-header>
                            <h3 class="deep-purple--text darken-1 font-weight-regular text-xl-h4 text-lg-h5 text-md-h6 text-sm-h4">{{faq.question}}</h3>
                        </v-expansion-panel-header>
                        <v-expansion-panel-content>
                            <p class="deep-purple--text darken-1 text-xl-h5 text-lg-h6 text-md-h6 text-sm-h4 font-weight-light">{{faq.answer}}</p>
                        </v-expansion-panel-content>
                        </v-expansion-panel>
                    </v-expansion-panels>
                    </v-col>
                </v-row>
            </div>
        </v-main>
    </v-app>
</template>

<script>
export default {
  head: {
    titleTemplate: 'Panday Digital - %s',
    title: 'Services',
    htmlAttrs: {
      lang: 'en'
    },
  },
    layout: 'dashboard',
    auth: false,
    methods: {
      test() {
        this.router.push('/dashboard');
      }
    },
//    mounted() {
//     this.$store.dispatch('themecolor/setThemeColor', "background-color: #eee !important")
//    },
    data() {
      return {
        faqs:[
          {
            id:1,
            question:'Why Panday Digital?',
            answer:'We offer you A to Z services to materialize your digital marketing strategy and help you reap the best results of your online presence. We listen to your thoughts and ideas, we help innovate and improvise those and implement them in the final product, which we create with a combination of fruitful SEO techniques, unique designs, appealing content, and effective and compatible coding.',
          },
          {
            id:2,
            question:'Why Panday Digital?',
            answer:'We offer you A to Z services to materialize your digital marketing strategy and help you reap the best results of your online presence. We listen to your thoughts and ideas, we help innovate and improvise those and implement them in the final product, which we create with a combination of fruitful SEO techniques, unique designs, appealing content, and effective and compatible coding.',
          },
          {
            id:3,
            question:'Why Panday Digital?',
            answer:'We offer you A to Z services to materialize your digital marketing strategy and help you reap the best results of your online presence. We listen to your thoughts and ideas, we help innovate and improvise those and implement them in the final product, which we create with a combination of fruitful SEO techniques, unique designs, appealing content, and effective and compatible coding.',
          },
          {
            id:4,
            question:'Why Panday Digital?',
            answer:'We offer you A to Z services to materialize your digital marketing strategy and help you reap the best results of your online presence. We listen to your thoughts and ideas, we help innovate and improvise those and implement them in the final product, which we create with a combination of fruitful SEO techniques, unique designs, appealing content, and effective and compatible coding.',
          },
        ],
        colors:[
          {
            color:'#1b75bb',
            id:1,
            discription:'"It was a pleasure working with Merlina and her team. They are extremely knowledgeable about Local SEO."',
            img:'/_nuxt/assets/resources/yeoman.png',
            name:'Yeoman',
            position:'CEO/artist/model',

          },
          {
            color:'#1b75bb',
            id:2,
            discription:' "Great working with Digital Marketing Manila. If more SEO projects come again in the future, I will definitely use them again."',
            img:'/_nuxt/assets/resources/ubunto.png',
            name:'Pinguin',
            position:'First Pinguin that can`t swim',      
          },
                    {
            color:'#1b75bb',
            id:3,
            discription:' "Great working with Digital Marketing Manila. If more SEO projects come again in the future, I will definitely use them again."',
            img:'/_nuxt/assets/resources/dog.png',
            name:'Ahmjigh',
            position:'Head',
          },
        ],
    }
  }
}
</script>

<style>

</style>