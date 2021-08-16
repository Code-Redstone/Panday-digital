<template>
    <v-app>
        <v-main class="MTM-150px">
            <div id="hero-offer-section" class=" pt-16 cyan">
                <v-container>
                    <v-row>
                        <v-col cols="12"  lg="6">
                            <div class="first-image text-center">
                                <v-img
                                id="offersheroimage"
                                class="ma-auto"
                                width="600px"
                                max-width="800px"
                                max-height="600px"
                                :src="require(`~/assets/resources/pricing.png`)"
                                />
                            </div>
                        </v-col>
                        <v-col class=" center "  cols="12"  lg="6" color="white">
                            <RegestrationForm/>
                        </v-col>
                    </v-row>
                </v-container>
            </div>
            <svg id="peak-center-soft" style="fill:#ffffff;transform:rotateX(180deg);height:100px;width:100%;background: #00BCD4;transform: scaleY(-1.5);" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="divider-color" d="M1437.37922,100.277057 L823.4576,26.0907362 C785.104953,21.2174623 750.835079,18.7808253 720.647978,18.7808253 C690.460878,18.7808253 657.029922,21.1301388 620.355113,25.8287658 L4.0317179,100.277057 L0,100.277057 L0,0.277057299 L1442,0.277057299 L1442,100.277057 L1437.37922,100.277057 Z"></path> </svg>
            <svg id="peak-center-soft" style="position: relative;z-index: 1;background: #ffffff;fill:#ffffff; height:20px;width:100%;" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="divider-color" d="M1437.37922,100.277057 L823.4576,26.0907362 C785.104953,21.2174623 750.835079,18.7808253 720.647978,18.7808253 C690.460878,18.7808253 657.029922,21.1301388 620.355113,25.8287658 L4.0317179,100.277057 L0,100.277057 L0,0.277057299 L1442,0.277057299 L1442,100.277057 L1437.37922,100.277057 Z"></path> </svg>
            <div id="firstoffers-Section" class="pt-12">
                <v-container>
                    <v-row>
                        <v-col cols="12">
                            <div class="Title">
                                <h1 class="deep-purple--text lighten-4 text-center font-weight-bold py-5 text-xl-h2 text-lg-h3 text-md-h5 text-sm-h2">CMS Development Pricing</h1>
                            </div>
                        </v-col>
                        <v-col v-for="(price) in pricing" :key="price.id" cols="12" lg="4" md="6">
                            <div >
                                <v-card
                                    class="mx-auto "
                                    max-width="540"
                                    :color="price.bodycolor"
                                >
                                    <v-sheet
                                    height="100px"
                                    :color="price.titlecolor"
                                    class="d-flex "
                                    >
                                        <h1 class="font-weight-thin text-h6 white--text text-center ma-auto">{{price.title}}</h1>
                                    </v-sheet>
                                    <v-sheet
                                    height="300px"
                                    :color="price.bodycolor"
                                    class=""
                                    >
                                        <div class="d-block">
                                            <h1 class="ma-auto white--text text-center font-weight-thin py-5 text-xl-subtitle-1 text-lg-h4 text-md-h4 text-sm-h4">
                                                ₱{{price.basicprice}} - ₱{{price.proprice}}   
                                            </h1>
                                            <h1 class="ma-auto white--text text-center font-weight-thin py-5 text-xl-h2 text-lg-h3 text-md-h5 text-sm-h2">
                                                Save {{price.save}}% today
                                            </h1>
                                            <p class="ma-auto font-weight-thin text-center white--text px-16 pt-0 mx-10">{{price.description}}</p>
                                        </div>
                                    </v-sheet>
                                    <v-card-actions class="d-block text-center pb-16">
                                        <v-btn
                                            color="#ffffff52"
                                            class="text-center title font-weight-light white--text px-10 py-8 rounded-lg mb-5"
                                            x-large
                                        >
                                            Buy Basic
                                        </v-btn>
                                        <br>
                                        <v-btn
                                            color="#ffffff52"
                                            class="text-center title font-weight-light white--text px-10 py-8 rounded-lg "
                                            x-large 
                                        >
                                            Buy Pro
                                        </v-btn>                                    
                                    </v-card-actions>
                                </v-card>
                            </div>
                        </v-col>
                    </v-row>
                </v-container>  
            </div>    
            <svg id="" style="fill:#fff;width:100%;height:100px;background:#00bcd4;position:relative;top:7px;" class=" positionR-bottom3 flip Dn700" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <polygon class=" pink lighten-2" points="0 0 3000 0 0 100"></polygon> </svg>
            <div id="second-section" class="cyan">
                    <v-container class="d-flex ">
                        <v-row>
                            <v-col cols="12 d-flex" lg="6"  > 
                                <div class="text-center">
                                    <h1 class="white--text text-center font-weight-bold py-5 text-xl-h3 text-lg-h4 text-md-h5 text-sm-h2">Custom Web Development Pricing</h1>
                                    <p class="white--text font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">Pricing for custom web development is difficult to anticipate, as each job is unique. After we've established the requirements and broken them down into User Stories, we'll be able to provide you a price. This enables us to construct tasks based on the user story requirements and assign time to each job.</p>             
                                    <p class="white--text  font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">The TOTAL price is then calculated by multiplying the number of hours each work by our hourly rate ($1,200). However, we define an MVP (minimum viable product) and great to have features in our Agile strategy. Payments are made only after the milestones that we set jointly are met. Unless otherwise specified, these are usually two-week work sprints. In this process, we are quite adaptable! </p>   
                                    <p class="white--text  font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">We do it this way to deliver full transparency to our clients, no surprises and you know what expect beforehand! Many times during the development of a custom project the client comes up with new ideas. Without this method, it`s hard to plan in the new changes, but with this method, we can add it easily to the next sprint of work and tell you the costs beforehand.</p>   
                                </div>
                            </v-col>
                            <v-col cols="12" lg="6" class="d-flex">
                                    <v-img
                                    class="ma-auto"

                                    max-width="700px"
                                    max-height="700px"
                                    :src="require(`~/assets/resources/CWD.png`)"
                                    />
                            </v-col>
                        </v-row>
                    </v-container>
            </div>
            <svg id="skewed" style="fill:#00BCD4;width:100%;height:100px;background:#fff;" class="positionR-bottom3 flip Dn700 " preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <polygon  points="0 0 3000 0 0 100"></polygon> </svg>
            <div id="third-section" class="">
                <v-container>  
                    <v-row>
                        <v-col cols="12">
                            <div class="Title">
                                <h1 class="deep-purple--text lighten-4 text-center font-weight-bold py-5 text-xl-h2 text-lg-h3 text-md-h5 text-sm-h2"> Maintenance Packages</h1>
                            </div>
                        </v-col>
                        <v-col v-for="(cmsprice) in CMSpricing" :key="cmsprice.id" cols="12" lg="4" md="6">
                            <div >
                                <v-card
                                    class="mx-auto "
                                    max-width="540"
                                    :color="cmsprice.bodycolor"
                                >
                                    <v-sheet
                                    height="100px"
                                    :color="cmsprice.titlecolor"
                                    class="d-flex "
                                    >
                                        <h1 class="font-weight-thin text-h6 white--text text-center ma-auto">{{cmsprice.title}}</h1>
                                    </v-sheet>
                                    <v-sheet
                                    height="300px"
                                    :color="cmsprice.bodycolor"
                                    class=""
                                    >
                                        <div class="d-block">
                                            <h1 class="ma-auto white--text text-center font-weight-thin py-5 text-xl-subtitle-1 text-lg-h4 text-md-h4 text-sm-h4">
                                                ₱{{cmsprice.basicprice}} - ₱{{cmsprice.proprice}}   
                                            </h1>
                                            <h1 class="ma-auto white--text text-center font-weight-thin py-5 text-xl-h2 text-lg-h3 text-md-h5 text-sm-h2">
                                                Save {{cmsprice.save}}% today
                                            </h1>
                                            <p id="px400-adjust" class="ma-auto font-weight-thin text-center white--text px-16 pt-0 mx-10">{{cmsprice.description}}</p>
                                        </div>
                                    </v-sheet>
                                    <v-card-actions class="d-block text-center pb-16">
                                        <v-btn
                                            color="#ffffff52"
                                            class="text-center title font-weight-light white--text px-10 py-8 rounded-lg mb-5"
                                            x-large
                                        >
                                            Avail
                                        </v-btn>                                
                                    </v-card-actions>
                                </v-card>
                            </div>
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
        title: 'Offers',
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
//        this.$store.dispatch('themecolor/setThemeColor',  "background-color: #000 !important")
//    },
    data() {
      return {
        colors:[
          {
            color:'#1b4cbb',
            id:1,
            discription:'"It was a pleasure working with Merlina and her team. They are extremely knowledgeable about Local SEO."',
            img:'/resources/yeoman.png',
            name:'Yeoman',
            position:'CEO/artist/model',

          },
          {
            color:'#1b4cbb',
            id:2,
            discription:' "Great working with Digital Marketing Manila. If more SEO projects come again in the future, I will definitely use them again."',
            img:'/resources/ubunto.png',
            name:'Pinguin',
            position:'First Pinguin that can`t swim',
          },
          {
            color:'#1b4cbb',
            id:3,
            discription:' "Great working with Digital Marketing Manila. If more SEO projects come again in the future, I will definitely use them again."',
            img:'/resources/dog.png',
            name:'Ahmjigh',
            position:'Head',
          },
        ],
        pricing:[
            {
            id:1,
            titlecolor:'#E53935',
            title:'WordPress Website',
            bodycolor:'#EF5350',
            basicprice:'24,000',
            proprice:'95,000',
            save:'12',
            description:'Ideal for Small Business to know their website Performance',
            },
            {
            id:2,
            titlecolor:'#D81B60',
            title:'Live chat & Chat Bot implementation (per month)',
            bodycolor:'#EC407A',
            basicprice:'1,500',
            proprice:'2,500',
            save:'12',
            description:'Ideal for Local Start-Ups/Small Businesses ',
            },
            {
            id:3,
            titlecolor:'#8E24AA',
            title:'Landing Page',
            bodycolor:'#AB47BC',
            basicprice:'5,000',
            proprice:'8,500',
            save:'12',
            description:'Ideal for ecommerce companies with the goal to reach massive audiences.',
            },    
            {
            id:4,
            titlecolor:'#5E35B1',
            title:'Heatmap Implementation/ Visitor recordings (per month)',
            bodycolor:'#7E57C2',
            basicprice:'2,300',
            proprice:'5,400',
            save:'12',
            description:'Ideal for ecommerce companies with the goal to reach massive audiences.',
            }, 
            {
            id:5,
            titlecolor:'#3949AB',
            title:'Email List Management',
            bodycolor:'#5C6BC0',
            basicprice:'6,200',
            proprice:'10,800',
            save:'12',
            description:'Ideal for ecommerce companies with the goal to reach massive audiences.',
            }, 
            {
            id:6,
            titlecolor:'#1E88E5',
            title:'Custom Payment Gateway Implementation',
            bodycolor:'#42A5F5',
            basicprice:'15,400',
            proprice:'3,070',
            save:'12',
            description:'Ideal for ecommerce companies with the goal to reach massive audiences.',
            },
            {
            id:7,
            titlecolor:'#039BE5',
            title:'Domainname +Setup (1yr)',
            bodycolor:'#29B6F6',
            basicprice:'2,300',
            proprice:'2,300',
            save:'12',
            description:'Ideal for ecommerce companies with the goal to reach massive audiences.',
            },
            {
            id:8,
            titlecolor:'#00ACC1',
            title:'Domainname (.com) yearly',
            bodycolor:'#26C6DA',
            basicprice:'750',
            proprice:'750',
            save:'12',
            description:'Ideal for ecommerce companies with the goal to reach massive .',
            }, 
            {
            id:9,
            titlecolor:'#00897B',
            title:'Backup restore website (per time)',
            bodycolor:'#26A69A',
            basicprice:'1,500',
            proprice:'2,300',
            save:'12',
            description:'Ideal for ecommerce companies with the goal to reach  audiences.',
            },                                                                                     
        ],
         CMSpricing:[
            {
            id:1,
            titlecolor:'#43A047',
            title:'SEO Maintenance',
            bodycolor:'#66BB6A',
            basicprice:'24,000',
            proprice:'95,000',
            save:'12',
            description:'On-Page optimization, Internal linking and Image optimization,  (10 hours per month)',
            },
            {
            id:2,
            titlecolor:'#7CB342',
            title:'SEO Maintenance',
            bodycolor:'#9CCC65',
            basicprice:'1,500',
            proprice:'2,500',
            save:'12',
            description:'On-Page optimization, Internal linking and Image optimization,  (5 hours per month)',
            },
            {
            id:3,
            titlecolor:'#FB8C00',
            title:'WordPress ',
            bodycolor:'#FFA726',
            basicprice:'5,000',
            proprice:'8,500',
            save:'12',
            description:'WP Core, Plugins, Daily Backups, Error Reporting, Security, SMALL content changes',
            },  
            {
            id:4,
            titlecolor:'#757575',
            title:'Website Speed Optimization ',
            bodycolor:'#BDBDBD',
            basicprice:'5,000',
            proprice:'8,500',
            save:'12',
            description:'* One Time Cost *',
            },                                                                                    
        ],
    }
  }
}

</script>

<style>

</style>