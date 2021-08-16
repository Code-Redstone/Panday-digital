<template>
  <v-app>
      <v-main class="MTM-150px testing">
        <div id="hero-section" class="indigo darken-1">
            <v-container class="d-flex 5" >
                <v-row>
                    <v-col cols="12 d-flex" lg="6"  > 
                        <div class="" id="Hero-Description">
                            <h3 class="white--text font-weight-bold text-xl-h3 text-lg-h4 text-md-h4 text-sm-h4 text-h5 mb-5">Best SEO Company in the Philippines</h3>
                            <p class="white--text font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">With our exceptional, structured SEO services in the Philippines, you can gain search engine dominance and long-term optimization of digital resources.</p>
                             <v-btn class="Rounded-botton px-10 py-8 text-lg-h5 text-md-subtitle-1 text-sm-h5 text-center"
                            elevation="1"
                            ><nuxt-link to="contact">Get a Quote</nuxt-link></v-btn>
                        </div>
                    </v-col>
                    <v-col cols="12" lg="6">
                            <v-img
                            class="ma-auto"
                            max-width="700px"
                            max-height="700px"
                            :src="require(`~/assets/resources/20945385.png`)"
                            />
                    </v-col>
                </v-row>
            </v-container>
        </div>
        <svg id="peak-center-soft" class="w-100 Ddn" style="background:#3949ab;fill:#ffffff; height:100px;" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="divider-color" d="M1437.37922,100.277057 L823.4576,26.0907362 C785.104953,21.2174623 750.835079,18.7808253 720.647978,18.7808253 C690.460878,18.7808253 657.029922,21.1301388 620.355113,25.8287658 L4.0317179,100.277057 L0,100.277057 L0,0.277057299 L1442,0.277057299 L1442,100.277057 L1437.37922,100.277057 Z"></path> </svg>
        <svg id="peak-center-soft" style="position: relative;z-index: 1;background: #ffffff;fill:#ffffff; height:20px;width:100%;bottom:10px;" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="divider-color" d="M1437.37922,100.277057 L823.4576,26.0907362 C785.104953,21.2174623 750.835079,18.7808253 720.647978,18.7808253 C690.460878,18.7808253 657.029922,21.1301388 620.355113,25.8287658 L4.0317179,100.277057 L0,100.277057 L0,0.277057299 L1442,0.277057299 L1442,100.277057 L1437.37922,100.277057 Z"></path> </svg>
        <div id="First-section" class="">
            <v-container class="d-flex">
                <v-row>
                    <v-col cols="12 d-flex" lg="6"> 
                        <div class="test">
                            <h5 class="font-weight-bold text-xl-h4 text-lg-h5 text-md-h4 text-sm-h4 text-h4 mb-5">Why Choose SEO Agency in the Philippines</h5>
                            <p class="font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">The digital business world is growing and evolving by the second, but Search Engine Optimization remains the goose that lays the golden eggs – you don't want to kill it at any cost due to a lack of effective strategy and execution.</p>
                            <p class="font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">Digital Marketing Manila is an end-to-end SEO agency in Philippines providing dynamic search engine optimization services, complete with all its necessary dimensions. We take pride in our utter commitment towards customers and their businesses, and our reputation of yielding excellent results precedes our name. Along with other digital solutions like web designing, web development, content marketing, PPC management, social media marketing, and online reputation management, SEO is among the front line services that we extend to make your company’s digital crusade a victorious one.</p>              
                        </div>
                    </v-col>
                    <v-col cols="12" lg="6" id="webdevregestration">
                        <RegestrationForm/>
                    </v-col>
                </v-row>
            </v-container>
        </div>
        <div id="Second-section" class="indigo darken-1">
            <svg id="skewed" style="fill:#fff; height:100px;" class="w-100 positionR-bottom3 flip Ddn" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <polygon class="divider-color" points="0 0 1442 0 0 100"></polygon> </svg>
            <v-container class="d-flex">
                <v-row>
                    <v-col cols="12 d-flex" lg="6"  > 
                        <div class="">
                            <h5 class="white--text font-weight-bold text-xl-h4 text-lg-h5 text-md-h4 text-sm-h4 text-h4 mb-5">What Is SEO?</h5>
                            <p class="white--text font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">In a summary, Search Engine Optimization (SEO) is the foundation upon which the success of your company's online campaign is determined. A strong, effective, and carefully implemented SEO strategy is critical for staying ahead of the competition and consistently turning the needle in your favor.</p>             
                            <p class="white--text font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">SEO is the process of optimizing the content, design, and appearance of your website so that web crawlers on search engines such as Google, Yahoo, and Bing find your websites and blog sites before your competitors. When combined with the right organic tools and techniques, the right SEO practices will propel your company through the highly competitive market crowded with numerous businesses vying for the top few spots and place you right there.</p>         
                            <p class="white--text font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">With more and more people entrusting the internet to find out about global and local businesses, a successful SEO campaign is not just a necessity, it can very much be the ace up your sleeve that wins you the game. At our digital marketing and SEO Company in Manila, we provide all the core aspects of SEO solutions to help our clients take their business a notch higher.</p>         
                        </div>
                    </v-col>
                    <v-col cols="12" lg="6">
                            <v-img
                            class="ma-auto"
                            max-width="400px"
                            max-height="400px"
                            :src="require(`~/assets/resources/programminglang.png`)"
                            />
                    </v-col>
                </v-row>
            </v-container>
        </div>
        <svg id="skewed" style="fill:#3949ab; height:100px;background:#fff;" class="w-100 positionR-bottom3 flip Ddn" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <polygon class="divider-color" points="0 0 1442 0 0 100"></polygon> </svg>
        <svg id="peak-center-soft" style="position: relative;z-index: 1;background: #ffffff;fill:#ffffff; height:20px;width:100%;" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="divider-color" d="M1437.37922,100.277057 L823.4576,26.0907362 C785.104953,21.2174623 750.835079,18.7808253 720.647978,18.7808253 C690.460878,18.7808253 657.029922,21.1301388 620.355113,25.8287658 L4.0317179,100.277057 L0,100.277057 L0,0.277057299 L1442,0.277057299 L1442,100.277057 L1437.37922,100.277057 Z"></path> </svg>
        <div id="Third-section" class="">
            <v-container class="d-flex">
                <v-row>
                    <v-col cols="12 d-flex" lg="6"  > 
                        <div class="">
                            <h5 class="font-weight-bold text-xl-h4 text-lg-h5 text-md-h4 text-sm-h4 text-h4 mb-5">Does Your Business Really Need SEO?</h5>
                            <p class="font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">Many entrepreneurs and business owners make the mistake of taking an SEO agency in the Philippines with a grain of salt, only to come to regret their decision. SEO has managed to age like fine wine in this age of limitless technological advancement at light speed. Since it first became a digital sensation in the early 1990s, the importance of SEO has only grown and expanded at an exponential rate. It is also intricately linked to many other digital solutions that your company requires, such as content curation and management, advertising services, local listings, and web development.</p>          
                        </div>
                    </v-col>
                    <v-col cols="12" lg="6">
                            <v-img
                            class="ma-auto"
                            max-width="550px"
                            max-height="550px"
                            :src="require(`~/assets/resources/marketing_copywriting_102.png`)"
                            />
                    </v-col>
                </v-row>
            </v-container>
        </div>
      </v-main>
  </v-app>
</template>

<script>
export default {
  head: {
    titleTemplate: 'Panday Digital - %s',
    title: 'Web Development',
    htmlAttrs: {
      lang: 'en'
    },
  },
}
</script>

<style>
#webdevregestration .Web-Dev {
    background: #fff !important;
}
@media screen and (min-width:1265px) {
    #Fourth-section {
        height: 550px;
        margin-bottom: 68px;
    }
}
@media screen and (max-width:1264px) {
    #First-section,
    #Second-section,
    #Third-section,
    #Fourth-section,
    #Fifth-section,
    #Sixth-section {
        padding-bottom: 100px;
        padding-top: 100px;
    }
    #hero-sectionheight{
        height: 21.1%;
    } 
}
.flip{
    transform: scaleX(-1);
}
.pt-100{
    padding-top: 100px !important;
}
.pagoda{
    background-color: #14828e;
}
.w-100{
    width:100%;
}
#peak-center-soft {
    transform: scaleY(-1.1);
}

</style>