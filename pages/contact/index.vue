<template>
  <v-app>
    <v-main class="MTM-150px">
        <v-sheet class="radius pb-15 mb-15" color="teal" height="100%" width="100%" style="padding-top: 150px;">
            <v-container>
                <v-row>
                    <v-col class="text-center"  cols="12" color="white">
                        <div class="d-block ">
                            <h2  class="pl-sm-5 white--text text-xl-h2 text-lg-h4 text-md-h5 text-sm-h3 font-weight-bold py-sm-5"> Be On the Top & Get More Traffic to Your Website</h2>
                            <p class="text-left white--text text-h6 font-weight-light text-xl-h4 text-lg-h5 text-md-subtitle-1 text-sm-h5 TAC">As the top digital marketing agency in the Philippines, we are honored to illuminate your ideas when it comes to steering your digital journey forward. Here are our top-rated services that attest to our legacy for you.</p>
                        </div>
                    </v-col>
                </v-row>
            </v-container>
        </v-sheet>
    </v-main>
    <v-main>
    <svg id="arched" class="w-100" style="background:#009688; fill:#fff;transform: scale(-1); height:100px;width:100%; padding-bottom:30px;" preserveAspectRatio="none" viewBox="0 0 1442 144" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="" d="M1442,14.287108 L682.266,129.122 C621.756612,138.267588 517.026832,143.977138 423.629338,144 L422.504016,144 C396.685569,143.99367 371.751899,143.551232 348.88,142.625 L0,128.495459 L0,0 L1442,0 L1442,14.287108 Z" id="Combined-Shape"></path> </svg>
        <v-container>
            <v-row>
                <v-col class=" center"  cols="12" sm="12" md="6" lg="6" xl="6" color="white">
                    <ContactForm/>
                </v-col>
                <v-col class=""  cols="12" sm="12" md="6" lg="6" xl="6" color="white">
                    <v-img
                    class="ma-auto"
                    max-width="600px"
                    max-height="600px"
                    :src="require(`~/assets/resources/Metrics.png`)"
                    />
                </v-col>
            </v-row>
        </v-container>
    </v-main>
    <svg id="arched" class="w-100" style="background:#009688; fill:#fff; height:100px; padding-bottom:30px;" preserveAspectRatio="none" viewBox="0 0 1442 144" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"> <path class="" d="M1442,14.287108 L682.266,129.122 C621.756612,138.267588 517.026832,143.977138 423.629338,144 L422.504016,144 C396.685569,143.99367 371.751899,143.551232 348.88,142.625 L0,128.495459 L0,0 L1442,0 L1442,14.287108 Z" id="Combined-Shape"></path> </svg>
  </v-app>
</template>

<script>
export default {
    head: {
        titleTemplate: 'Panday Digital - %s',
        title: 'Contact',
        htmlAttrs: {
        lang: 'en'
        },
    },
}
</script>

<style>

</style>