<template>
  <v-app>
      <v-main class="MTM-150px testing">
        <div id="hero-section" class="indigo lighten-1">
            <v-container class="d-flex 5" >
                <v-row>
                    <v-col cols="12 d-flex" lg="6"  > 
                        <div class="" id="Hero-Description">
                            <h3 class="white--text font-weight-bold text-xl-h3 text-lg-h4 text-md-h4 text-sm-h4 text-h5 mb-5 TAC">Local SEO Expert In The Philippines</h3>
                            <p class="white--text font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5 TAC">Take control of the local market with a vibrant online presence created with dedication and diligence by a local SEO expert for you.</p>
                             <v-btn class="Rounded-botton px-10 py-8 text-lg-h5 text-md-subtitle-1 text-sm-h5 text-center TAC"
                            elevation="1"
                            ><nuxt-link to="contact">Get a Quote</nuxt-link></v-btn>
                        </div>
                    </v-col>
                    <v-col cols="12" lg="6">
                            <v-img
                            class="ma-auto"
                            max-width="700px"
                            max-height="700px"
                            :src="require(`~/assets/resources/Seopage.png`)"
                            />
                    </v-col>
                </v-row>
            </v-container>
        </div>
        <svg id="peak-center-soft" class="w-100 Ddn" style="background:#5C6BC0;fill:#ffffff; height:100px;" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="divider-color" d="M1437.37922,100.277057 L823.4576,26.0907362 C785.104953,21.2174623 750.835079,18.7808253 720.647978,18.7808253 C690.460878,18.7808253 657.029922,21.1301388 620.355113,25.8287658 L4.0317179,100.277057 L0,100.277057 L0,0.277057299 L1442,0.277057299 L1442,100.277057 L1437.37922,100.277057 Z"></path> </svg>
        <svg id="peak-center-soft" style="position: relative;z-index: 1;background: #ffffff;fill:#ffffff; height:20px;width:100%;bottom:10px;" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="divider-color" d="M1437.37922,100.277057 L823.4576,26.0907362 C785.104953,21.2174623 750.835079,18.7808253 720.647978,18.7808253 C690.460878,18.7808253 657.029922,21.1301388 620.355113,25.8287658 L4.0317179,100.277057 L0,100.277057 L0,0.277057299 L1442,0.277057299 L1442,100.277057 L1437.37922,100.277057 Z"></path> </svg>
        <div id="First-section" class="">
            <v-container class="d-flex">
                <v-row>
                    <v-col cols="12 d-flex" lg="6"> 
                        <div class="test">
                            <h5 class="font-weight-bold text-xl-h4 text-lg-h5 text-md-h4 text-sm-h4 text-h4 mb-5"> Why Choose Local SEO Agency In The Philippines</h5>
                            <p class="font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">Because it is now well established, simply having a business will not suffice. It is nearly impossible to beat the competition and achieve success without a strong online presence. Both buyers and sellers are now using the internet. Whatever business sector your company is in, chances are that more than 40% of the industry's customers look up potential service providers online. Your company will fall behind in this race if it does not have a good local SEO. Digital Marketing Manila is a leading local SEO company in the Philippines, and we ensure that your company receives the exposure and recognition it deserves.</p>
                            <h5 class="font-weight-bold text-xl-h4 text-lg-h5 text-md-h4 text-sm-h4 text-h4 mb-5"> What is Local SEO?</h5>
                            <p class="font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">Local SEO is a set of organic techniques used to optimize your online presence for highly targeted, location-specific business searches. It enables you to connect with the local market and cultivate a loyal customer base closer to home. It entails using the same old methods of traditional search engine optimization processes, but with an emphasis on emphasizing its geographical location in order to attract customers within a certain radius. Traditional SEO tools like link building, on-page optimization, and content management can help you gain traction in a broader, more general sense. However, if you want to dominate your neighbors, you'll need something extra. Our local SEO services in the Philipines</p>              
                        </div>
                    </v-col>
                    <v-col cols="12" lg="6" id="webdevregestration">
                        <RegestrationForm/>
                    </v-col>
                </v-row>
            </v-container>
        </div>
        <v-container class="pb-10">
                <v-row>
                    <v-col cols="12" sm="12" md="6" class="ma-auto" v-for="work in works" :key="work.id" >
                        <v-card
                        class="pa-10 Services-hover Services-Font"
                        outlined
                        shaped
                        >
                            <h3 class="mb-5 lighten-1 indigo--text text-center font-weight-bold text-xl-h4 text-lg-h5 text-md-h4 text-sm-h4 text-h4 mb-5">{{work.title}}</h3>
                            <p class=" font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">{{work.discription}}</p>
                            <ul v-for="listing in work.listing" :key="listing.id">
                                <li class="font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">{{listing.list}}</li>
                            </ul>
                        </v-card>
                    </v-col>
                </v-row>
            </v-container>
        <div id="" class="indigo lighten-1">
            <v-container class="d-flex">
                <v-row>
                    <v-col cols="12 d-flex"> 
                        <div class="">
                            <h1 class="white--text font-weight-bold text-xl-h3 text-lg-h4 text-md-h4 text-sm-h4 text-h5 mb-5 text-center mt-10">Our Local SEO Services</h1>
                            <h1 class="mb-5 lighten-1 white--text font-weight-light text-center text-xl-h5 text-lg-h5 text-md-h4 text-sm-h4 text-h4 mb-5">What are you signing up for – find out!</h1>
                            <h1 class="mb-5 lighten-1 white--text font-weight-bold text-xl-h4 text-lg-h5 text-md-h4 text-sm-h4 text-h4 mb-5">Local SEO Audit</h1>                            
                            <p class="white--text font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">A Local SEO expert or an SEO consultant from Digital Marketing Manila would go through your entire online persona and analyze every piece of information available on the internet about you or your business to create a meticulously researched audit result. The evaluation process is exhaustive and done with meticulous attention to detail so that you can make an informed decision on how to avoid risks and capitalize on opportunities. Our Local SEO expert team typically conducts the audit over five extensive steps. The steps are as follows:</p>         
                            <p v-for="step in steps" :key="step.id" class="white--text font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5 py-1"><b class="font-weight-bold">Step {{step.id}}:</b> {{step.discription}}</p>
                        </div>
                    </v-col>
                </v-row>
            </v-container>
        </div>
        <svg id="skewed" style="fill:#5C6BC0; height:100px;background:#fff;" class="w-100 positionR-bottom3 flip Ddn" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <polygon class="divider-color" points="0 0 1442 0 0 100"></polygon> </svg>
        <svg id="peak-center-soft" style="position: relative;z-index: 1;background: #ffffff;fill:#ffffff; height:20px;width:100%;" preserveAspectRatio="none" viewBox="0 0 1442 100" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="divider-color" d="M1437.37922,100.277057 L823.4576,26.0907362 C785.104953,21.2174623 750.835079,18.7808253 720.647978,18.7808253 C690.460878,18.7808253 657.029922,21.1301388 620.355113,25.8287658 L4.0317179,100.277057 L0,100.277057 L0,0.277057299 L1442,0.277057299 L1442,100.277057 L1437.37922,100.277057 Z"></path> </svg>
        <div class="fifth-section">
            <v-container class="pt-10">
                <v-row>
                    <v-col cols="12" sm="12" md="6" class="ma-auto" v-for="Offer in Offers" :key="Offer.id" >
                        <v-card
                        class="pa-10 Services-hover Services-Font"
                        outlined
                        shaped
                        >
                            <h3 class="mb-5 lighten-1 indigo--text text-center font-weight-bold text-xl-h4 text-lg-h5 text-md-h4 text-sm-h4 text-h4 mb-5">{{Offer.title}}</h3>
                            <p class="text-center font-weight-light text-xl-h6 text-lg-h6 text-md-h6 text-sm-h5">{{Offer.discription}}</p>
                        </v-card>
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
    data() {
        return{
            steps:[
                {
                    id:1,
                    discription:`Collecting your company's information – objectives, website URLs, social media profile credentials, and previous digital marketing efforts.`,
                },
                {
                    id:2,
                    discription:`Perform an end-to-end inspection of all provided data using a combination of manual and SEO tools.`,
                },   
                {
                    id:3,
                    discription:`Sort and organize the audit results before reviewing them to draw relevant conclusions. This step generates recommendations for further improving the online presence, which aids in the next step.`,
                }, 
                {
                    id:4,
                    discription:`A local SEO audit report is created for the customer and other parties involved to read through and understand the shortcomings of their online marketing efforts. Our knowledgeable consultants will be available to you to discuss the report and clear up any confusion you may have about it.`,
                },   
                {
                    id:5,
                    discription:`Once the client is satisfied with the local SEO audit report, an action plan is developed based on a brainstorming session to arrive at specific local SEO strategies that will help improve your area-specific rankings and integrate the same in all online locations where you have a presence.`,
                },        
            ],
            works: [
                {
                    id: 1,
                    title: 'How Does Local SEO Work?',
                    discription:`Local SEO practices ensure that your website and online directory listings are visible to people in your area. It optimizes all of your online profiles and information and integrates them with your local information so that it appears on the first page of Google for area-specific searches. It accomplishes this through the following express optimization activities:`,
                    listing:[
                        {
                            id:1,
                            list:`A thorough local SEO audit`,
                        },
                        {
                            id:2,
                            list:`Search and analysis for locality-based keywords`,
                        },
                        {
                            id:3,
                            list:`Optimization of website content for regional locations, maps and terms`,
                        },
                        {
                            id:4,
                            list:`Verification of business and authentication of NAP – name, address and phone number`,
                        },
                        {
                            id:5,
                            list:`Registration to local business directories and listings of major search engines`,
                        },
                        {
                            id:6,
                            list:`Manage positive reviews and feedback’s on the website, social media platforms and business listings`,
                        },
                        {
                            id:7,
                            list:`Covering a social media marketing campaign focusing on the specific area`,
                        },
                    ],
                },
                {
                    id: 2,
                    title: `Why Does Your Business Need Local SEO?`,
                    discription:`Your company has already undergone a fairly detailed SEO strategy, and you are confident that it is sufficiently updated from the ground up to attract all types of audience attention. Local SEO activities, on the other hand, are critical to achieving more area-specific success. For example, if you own a new pizzeria in UP Village or run a construction company out of one of Makati's commercial buildings, you will need to use local SEO services in Philippines to beat the competition and stay on top.`,
                    listing:[
                        {
                            id:1,
                            list:`With local SEO integration, your business information will reach interested clients far more easily and quickly, and you will be able to make a sale before your competitors in the same area.`,
                        },
                        {
                            id:2,
                            list:`With location-specific searches, there is a high likelihood that the customer is genuinely interested in the service and has not stumbled upon your company by chance, resulting in a guaranteed lead conversion.`,
                        },
                        {
                            id:3,
                            list:`With localized optimization, you will be filtering out the rest of the world and competing only with the local brands, therefore diluting the concentration of rivalry.`,
                        },
                    ],
                },
            ],
            Offers: [
                
                {
                    id: 1,
                    title: `Google My Business Optimization`,
                    discription: `Google is by far the most popular search engine on the planet, accounting for more than 70% of all search hits at any given time. It is critical that your company is optimized in accordance with Google guidelines. The search engine giant provides a free service through its listing platform, Google My Business, for local businesses to post their NAP information, business description, and exact location on a Google Map. We assist you in optimizing your GMB listing by ensuring that all information provided is accurate and aligns with positive lead generation.`
                },
                {
                    id: 2,
                    title:`Titles and Metadata Optimization` ,
                    discription:`In a nutshell, your website's title and metadata are important elements that reflect the nature of your business. These are the behind-the-scenes aspects of SEO that communicate with search engine crawlers and provide relevant information in response to a search request. We pay close attention to including location-based keywords in these elements and making them catchy and interesting, so your business can cut through the ocean of search results generated by Google, Yahoo, or Bing.`
                },
                {
                    id: 3,
                    title: `Social Media Management`,
                    discription:`Nowadays, social media is essential in almost all types of digital marketing solutions, including local SEO. Indeed, because of the community building and mutual sharing features, it is strongly associated with localized searches. Digital Marketing Manila manages your social media platforms in order to integrate them with your local SEO campaign.`
                },
                {
                    id: 4,
                    title:`NAP Consistency`,
                    discription:`It is critical for the success of your local SEO strategy to have authentic and consistent NAP information. NAP stands for Name, Address, and Phone Number, which are the three main pillars of optimizing your business locally. We ensure that your NAP information is up to date and that it appears on all relevant pages of your website, blog, and social media platforms.`
                },
                {
                    id: 5,
                    title:`Backlink Building`,
                    discription:`Digital Marketing Manila will secure your business site with effective backlink opportunities from renowned and reputed high authority websites, directories, and blog posts, thereby increasing your credibility with local customers.`
                },
                {
                    id: 6,
                    title:`Local Citations`,
                    discription:`To appear higher in search results, your company's name must be prominent in local directories and business listings. Our local SEO services include searching for all relevant citation sites and getting your business listed on them.`
                }                                                                             
            ],
        }
    },
}
</script>

<style>
#webdevregestration .local-seo {
    background: #fff !important;
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