<template>
<v-container>
    <v-row>
        <v-col class="Text-center"  cols="12" >
            <div class="div text-center">
              <h3 class="black--text text--secondary font-weight-light text-xl-h4 text-lg-h5 text-md-h6 text-sm-h4 ">INCREASE TRAFFIC AND REVENUE</h3>
              <h2  class="black--text text--secondary text-xl-h2 text-lg-h4 text-md-h5 text-sm-h3 font-weight-bold py-5"> Be On the Top & Get More Traffic to Your Website</h2>
              <p class="black--text text--secondary text-h6 font-weight-light text-xl-h4 text-lg-h5 text-md-subtitle-1 text-sm-h5">We are thrilled to illuminate your thoughts when it comes to leading your digital journey forward as the Philippines' top digital marketing agency. Here are our top-rated services that attest to our legacy for you.</p>
            </div>
        </v-col>            
        <v-col class="text-center" cols="4" sm="12" md="4" lg="4" xl="4" v-for="seo in seos " :key="seo.id" >
            <v-card 
            class="pa-8 Services-hover Services-Font rounded-xl"
            outlined
            >
                <v-img
                class="ma-auto"
                max-width="200"
                max-height="200"
                :src="require(`~/assets/resources/`+seo.img)"
                >
                </v-img>
                <h3 class="mb-5 font-weight-bold text-center Services-Font text-xl-h4 text-lg-h5 text-md-h6 text-sm-h4">{{seo.title}}</h3>
                <p class="text-justify text-xl-h5 text-lg-h5 text-md-subtitle-1 text-sm-h5">{{seo.discription}}</p>
            </v-card>
        </v-col>
    </v-row>
</v-container>
</template>

<script>
export default {
    name:'BeOnTop',
    data() {
        return{
            seos: [
          {
            id:1,
            img:'seoseo.png',
            title:'Search Engine Optimization (SEO)',
            discription:'Establish your website as the first location when people search for items or services online. As the most reputable brand in your business, this is your ticket to securing leads.',
          },
          {
            id:2  ,
            img:'smm.png',
            title:'Marketing on Social Media',
            discription:`Utilize these game-changing platforms to capture the world with your every move. Your brand will be unstoppable once you've mastered how to engage your audience on social media.`,
          },
          {
            id:3  ,
            img:'lseo.png',
            title:'Local Search Engine Optimization',
            discription:`Consumers prioritize brands that provide complete convenience through closeness and accessibility. Ensure that your local customers find you first to influence their purchasing decisions effectively.`,
          },
          {
            id:4  ,
            img:'wdd.png',
            title:'Web Development and Design',
            discription:`Your website's aesthetics and user-friendliness will undoubtedly increase your online relevance. Leave your customers speechless with the way you welcome them to your company's headquarters`,
          },
          {
            id:5  ,
            img:'rm.png',
            title:'Management of Reputation',
            discription:`Take charge of the online dialogue that will help your company grow. Work with us to develop strategies that can help you change the odds and boost your business with every audience engagement.`,
          },
          {
            id:6  ,
            img:'Ads.png',
            title:'Management of Pay Per Click Campaigns',
            discription:'Directly diverting your resources to your target consumers will drive constant traffic to your website. Flourish in the areas that count.',
          },
          {
            id:7  ,
            img:'cdg.png',
            title:'Graphic Design for Creatives',
            discription:`Nothing is more appealing than photographs that demonstrate your company's capabilities. Invest in captivating them with innovative ideas and outstanding visual creativity`,
          },
          {
            id:8  ,
            img:'cwm.png',
            title:'Marketing and Content Writing',
            discription:`Create material that turns visitors into followers. Turn curiosity into a long-term commitment. It's crucial to be seen and heard, and we're here to help you find the right vocabulary that transforms.`,
          },
          {
            id:9  ,
            img:'em.png',
            title: 'Email Marketing',
            discription:'Establish personal connections with your customers outside of their inboxes. With a cost-effective plan and exceptional conversions, you can build your credibility through email marketing',
          },
        ],
        }
    }
}
</script>

<style>

</style>