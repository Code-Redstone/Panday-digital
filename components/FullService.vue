<template>
    <v-container class="pb-10">
        <v-row>
            <v-col cols="12">
                <div class=" text-center Services-Font">
                <h1 class="white--text font-weight-bold text-xl-h2 text-lg-h2 text-md-h3 text-sm-h4 py-8">FULL-SERVICE DIGITAL MARKETING FIRM</h1>
                </div>
            </v-col>
            <v-col cols="12" sm="6" lg="4" class="ma-auto" v-for="service in services" :key="service.id" >
                <v-card
                class="pa-10 Services-hover Services-Font"
                outlined
                shaped
                >
                    <h3 class="mb-5 blue--text text-center Services-Font font-weight-bold text-xl-h3 text-lg-h5 text-md-h5 text-sm-h4 text-h5wa pt-5">{{service.title}}</h3>
                    <p class="text-center text-xl-h5 text-lg-h6 text-md-h6 text-sm-h5">{{service.discription}}</p>
                </v-card>
            </v-col>
        </v-row>
    </v-container>
</template>
<script>
export default {
    name:'FullService',
    data() {
        return{
            services: [
                
                {
                    id: 1,
                    title: 'Take a "No Filter" Image',
                    discription:'Panday Digital Marketing team is highly professional. They tell you what needs to be done and manage your expectations. She delivers on time and is always available to answer questions and explain her work. I’m glad I discovered the right team to work with on a long-term basis'
                },
                {
                    id: 2,
                    title: 'Reach Out to the Largest Audience',
                    discription:'Our focus is on executing well-thought-out campaigns based on our globally proven methodologies. Without a hyper-targeted market, even the most innovative product would fail. Rely on our expertise to spot trends and create strong audience connections for your company.'
                },
                {
                    id: 3,
                    title: 'Transform with Successes',
                    discription:' Dont waste time with trial and error. Lets concentrate on putting your efforts into action rather than merely making educated predictions. The secret to defeating substandard practices is to use analytics. You can learn about your market, predict your competitors moves, and calculate your next power move with us.'
                },
            ],
        }
    },
}
</script>
<style>
</style>