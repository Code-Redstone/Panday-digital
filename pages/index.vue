<template>
  <v-app > 
    <v-main style="margin-top:50px;" class="desktop-main">
      <v-sheet class="radius" color="#1b75bb" height="100%" width="100%" style="padding-top: 100px;">
        <v-container>
          <v-row>
            <v-col cols="12" sm="12" md="6" lg="6" xl="6">
              <div class="first-image text-center">
                <v-img
                class="ma-auto"
                max-width="600px"
                max-height="600px"
                :src="require(`~/assets/resources/home.png`)"
                />
              </div>
            </v-col>
            <v-col class=" center"  cols="12" sm="12" md="6" lg="6" xl="6" color="white">
              <div class="d-block ">
                <h3 class="white--text font-weight-regular text-xl-h4 text-lg-h5 text-md-h6 text-sm-h4">WORLD-CLASS DIGITAL BUILDER</h3>
                <h1 class="white--text font-weight-bold py-5 text-xl-h2 text-lg-h3 text-md-h5 text-sm-h2">PANDAY DIGITAL Setting Outstanding Digital Standards</h1>
                <p class="white--text font-weight-light text-xl-h5 text-lg-h5 text-md-subtitle-1 text-sm-h5">The leading digital marketing agency in the Philippines can only match the digital brilliance your audience expects from you with globally tested digital creativity. Don't settle for anything less than the unexpected when it comes to your brand.</p><br>
                <v-btn class="Rounded-botton px-10 py-8 text-lg-h6 text-md-subtitle-1 text-sm-h5"
                  elevation="1"
                ><nuxt-link to="contact">Get a Quote</nuxt-link>
                </v-btn>
              </div>
            </v-col>
          </v-row>
        </v-container>
      </v-sheet>
    </v-main>
    <v-sheet 
    class="desktop-main"
    max-height="100px"
    max-width="100%"
    >
      <svg id="hill-side-round" style=" margin-bottom:10px;fill: white;height: 100%;width: 100%;transform: scaleY(-1)scaleX(-1);background: rgb(27, 117, 187)" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="divider-color" d="M1442,34.6187945 C1315.02765,14.2772114 1160.84924,2.89696087 977.282647,2.89696087 C645.766901,2.89696087 281.275997,40.0139604 0,100 L0,0 L1442,0 L1442,34.6187945 Z"></path> </svg>
    </v-sheet>
    <v-main class="desktop-main">
      <v-sheet 
      max-width="100%" 
      max-height="100%"
      >
        <v-container>
          <v-row>
            <v-col cols="6" sm="12" md="6" lg="6" xl="6">
              <RegestrationForm/>
            </v-col>
            <v-col cols="6" sm="12" md="6" lg="6" xl="6" >
              <div class="d-block ">
                <h3 class="blue--text font-weight-regular text-xl-h4 text-lg-h5 text-md-h6 text-sm-h4 pt-5">WORLD-CLASS DIGITAL BUILDER</h3>
                <h1 class="blue--text font-weight-bold text-xl-h2 text-lg-h3 text-md-h5 text-sm-h2 py-8">PANDAY DIGITAL Driving Outstanding Digital Specifications</h1>
                <p class="black--text font-weight-light text-justify text-xl-h5 text-lg-h5 text-md-subtitle-1 text-sm-h5 text-justify">By now, we've all figured it out. When it comes to spotting genuine and reputable products online, Filipinos are always one step ahead. Panday Digital provides simple, data-backed strategies for measurable results that ideally target their admiration.<br><br> We recognize how carefully planned digital strategies have resulted in increased traffic, revenue, and recognition. Today is your last chance to claim the top spot in your target audience's digital universe. Are you up for it?
                </p><br><br>
                <v-btn x-large color="blue"
                  elevation="1"
                  class="px-15 py-10 "
                ><span class="white--text font-weight-light text-justify text-xl-h6 text-lg-h6 text-md-subtitle-2 text-sm-h5">SEE WHAT WE OFFER</span>
                </v-btn> 
              </div>
            </v-col>
          </v-row>
        </v-container>
      </v-sheet>
    </v-main>
    <v-main class="desktop-main">
      <svg id="hill-side-round" style="fill: rgb(27, 117, 187);height: 100px; width: 100%; transform: scaleY(-1) scaleX(-1); position: relative;top: 10px;" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="divider-color" d="M1442,34.6187945 C1315.02765,14.2772114 1160.84924,2.89696087 977.282647,2.89696087 C645.766901,2.89696087 281.275997,40.0139604 0,100 L0,0 L1442,0 L1442,34.6187945 Z"></path> </svg>    
      <v-sheet class="" color="#1b75bb" height="101%" width="100%">
        <FullService/>
      </v-sheet>
    </v-main>
    <v-main class="desktop-main">
      <v-sheet max-width="100%" max-height="100%">
        <svg id="hill-side-round" style="fill:  rgb(27, 117, 187);height: 100px;width: 100%;transform: scaleY(1)scaleX(1);" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="divider-color" d="M1442,34.6187945 C1315.02765,14.2772114 1160.84924,2.89696087 977.282647,2.89696087 C645.766901,2.89696087 281.275997,40.0139604 0,100 L0,0 L1442,0 L1442,34.6187945 Z"></path> </svg>
      </v-sheet>
    </v-main>
    <v-main class="desktop-main">
      <v-sheet class="" height="100%" width="100%">
        <BeOnTop/>
      </v-sheet>
    </v-main>
    <v-main class="desktop-main">
      <v-sheet class="" height="100%" width="100%">
        <v-container>
          <v-row>
            <v-col class="Text-center"  cols="12" >
              <h3  class="blue--text text-center text-xl-h3 text-lg-h4 text-md-h5 text-sm-h3 font-weight-bold py-5"> Why Panday Digital Should be Partner in Digital Marketing</h3>
            </v-col>            
            <v-col class="d-flex"  sm="12" md="6" lg="6" xl="6" >
              <div class="div">
                <p class="font-weight-light text-xl-h5 text-lg-h5 text-md-h6 text-sm-h3">
                  1. Knowledgeable and Highly Experienced.
                  <br><br>
                  2. Particular with Deadlines.
                  <br><br>
                  3. Outstanding Track Records
                  <br><br>
                  4. Budget-Friendly Pricing
                  <br><br>
                  5. Conscientious Marketing
                  </p><br>
              </div>
            </v-col>
            <v-col class=""  sm="12" md="6" lg="6" xl="6" >
              <div class="div">
                <p class="font-weight-light text-xl-h5 text-lg-h5 text-md-h6 text-sm-h3">Why would you select us over all the other digital marketing firms in town?  Is it just due to the diverse services we provide, or is there more to us?<br><br>There is, indeed, more to us. The result of your digital marketing plan, how it appears to the consumers' eyes, and the outcomes it produces, are evidence of our experience and competence in the field. Plus, how we go about the entire approach is a wholesome exhibition of our service.</p><br>
              </div>
            </v-col>
          </v-row>
        </v-container>
      </v-sheet>
    </v-main>
    <!--
    <v-main class="desktop-main">
      <svg id="deepening-off" style="fill: rgb(27, 117, 187); height:60px; width:100%; transform: scaleY(-1) scaleX(-1);     position: relative; top: 7px;" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="divider-color" d="M394.85237,100 L-1,100 L-1,0 L-1,1.07456559 C157.650655,93.379895 352.733938,121.089042 584.249849,84.2020074 C913.749958,31.7033176 1199.33335,4.31314693 1441.00001,2.03149535 L1441.00001,0 L-0.999987893,0 L1441,0 L-0.999987893,0 L1441,0 L1441,100 L-1,100 L-1,0 L-1,1.07456559 C112.35263,67.0248254 244.303421,99.9999702 394.85237,100 Z" id="deepening-off" transform="translate(720.000006, 50.000000) scale(1, -1) translate(-720.000006, -50.000000) "></path> </svg>
      <v-sheet class="" height="400px" width="100%" color="#1b75bb">
        <div class="container">
          <div class="testimonial">
            <h1 class="white--text font-weight-regular text-xl-h2 text-lg-h3 text-md-h4 text-sm-h4">What Did Our Clients Say</h1>
          </div>
        </div>
        <div class="container">
          <v-carousel 
          height="250px"
          class="center"
          >
            <v-carousel-item
              v-for="(color) in colors"
              :key="color.id"
              reverse-transition="fade-transition"
              transition="fade-transition"
              height="100%"
              class="px-10 pa-4"
            >
              <v-sheet
                :color="color.color"
                tile
                height="100%"
              >
                <v-row
                  class="fill-height"
                  align="center"
                  justify="center"
                >
                  <v-row>
                    <v-col cols="8" class="center">
                      <div class="display-3 text-center">
                        <p class="white--text font-weight-light px-10 font-weight-light text-xl-h5 text-lg-h5 text-md-h6 text-sm-h3">{{color.discription}}</p>
                      </div>
                    </v-col>
                    <v-col cols="4 " class="center">
                      <div class=" display-3 center text-center">
                        <v-avatar
                          size="130px"
                          color="red"
                        >       
                          <v-img
                          :src="require(`~/assets/resources/`+color.img)"
                          max-width="120px"
                          max-height="120px"
                          ></v-img>
                        </v-avatar>
                        <div class="persons d-block text-left ml-5">
                          <h6 class="">{{color.name}}</h6>
                          <p class="white--text text-subtitle-1 text-h6 font-weight-light text-xl-h4 text-lg-h5 text-md-h6 text-sm-h3"> {{color.position}}</p>
                        </div>
                      </div>
                    </v-col>                    
                  </v-row>
                </v-row>
              </v-sheet>
            </v-carousel-item>
          </v-carousel>
        </div>
      </v-sheet>
    </v-main>
    -->
    <v-main class="desktop-main">
      <div class="container">
        <v-row>
          <v-col
            cols="12"
          >
            <div class="Faq-title">
              <h1 class="blue--text font-weight-regular text-xl-h2 text-lg-h3 text-md-h4 text-sm-h4">Frequently Asked Questions</h1>
            </div>
          </v-col>
          <v-col cols="12">
            <v-expansion-panels >
              <v-expansion-panel
                v-for="faq in faqs"
                :key="faq.id"
              >
                <v-expansion-panel-header>
                  <h3 class="font-weight-regular text-xl-h4 text-lg-h5 text-md-h6 text-sm-h4">{{faq.question}}</h3>
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                  <p class="text-xl-h5 text-lg-h6 text-md-h6 text-sm-h4 font-weight-light">{{faq.answer}}</p>
                </v-expansion-panel-content>
              </v-expansion-panel>
            </v-expansion-panels>
          </v-col>
        </v-row>
      </div>
    </v-main >
    <v-main class="desktop-main">
      <div class="testing101">
        <h1 v-bind:jr="jr"></h1>
      </div>
    </v-main>
  </v-app>
</template>

<script >
export default {
    layout: 'dashboard',
    auth: false,
    methods: {
      test() {
        this.router.push('/dashboard');
      }
    },
    data() {
      return {
         jr:'Click me',
        faqs:[
          {
            id:1,
            question:'1. Why Choose Panday Digital?',
            answer:'We offer various services to help you put your digital marketing strategy into action and get the most out of your online presence. We listen to your ideas and suggestions, then assist you to innovate and improve them before incorporating them into the final result, which we create using a combination of successful SEO strategies, distinctive designs, compelling content, and efficient and compatible coding.',
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
            img:'yeoman.png',
            name:'Yeoman',
            position:'CEO/artist/model',

          },
          {
            color:'#1b75bb',
            id:2,
            discription:' "Great working with Digital Marketing Manila. If more SEO projects come again in the future, I will definitely use them again."',
            img:'ubunto.png',
            name:'Pinguin',
            position:'First Pinguin that can`t swim',
          },
                    {
            color:'#1b75bb',
            id:3,
            discription:' "Great working with Digital Marketing Manila. If more SEO projects come again in the future, I will definitely use them again."',
            img:'dog.png',
            name:'Ahmjigh',
            position:'Head',
          },
        ],
    }
  }
}
</script>

<style>
.pt-100{
  padding-top: 100px;
}
.center {
    display: flex;
    align-items: center;
}
.first-image img {
    width: 100%;
}
.Services-hover {
    box-shadow: 0px 3px 64px 0px rgb(41 54 69 / 10%);
    border-color:white !important;
}
.Digital-Services:hover{
    box-shadow: 0px 3px 60px 3px rgb(255 255 255 / 22%);
}
.Services-hover:hover{
  box-shadow: 0px 3px 40px 1px rgb(62 87 100 / 29%);
}
.Services-Font h1{
  font-size: 47px !important;
}
.Services-Font h1{
  font-size: 47px !important;
}
.Services-Font h3{
  font-size: 23px !important;
}
.Services-Font p{
  font-size: 15px !important;
}
.v-expansion-panel::before {
  box-shadow: 0px !important;
}

</style>
 