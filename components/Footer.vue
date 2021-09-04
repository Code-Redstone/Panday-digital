<template>
    <v-main >
        <v-container>
            <v-row>
                <v-col cols="12 py-15">
                    <v-row>
                        <v-col cols="12 " md="4" lg="2" sm="6">
                            <h2 class="white--text font-weight-thin">About us</h2><br>
                            <p class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-light">
                                We create the fastest websites you've ever seen. And we design and develop custom business applications ranging from simple point-of-sale systems to enterprise resource planning, logistics, and human resources.
                            </p>
                        </v-col>                                                                     
                        <v-col cols="12 " md="4" lg="2" sm="6">
                            <h2 class="white--text font-weight-thin">Panday Digital</h2><br>
                            <p class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-light ">
                                Purok Jasmin, <br>
                                Barangay Acmac,<br>
                                Iligan City,<br>
                                Lanao del Norte,<br>
                                Mindanao, 9200 Philippines
                            </p>
                        </v-col>
                        <v-col cols="12 " md="4" lg="2" sm="6">
                            <h2 class="white--text font-weight-thin">Business Hours</h2><br>
                            <p class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-light">
                                Monday – Saturday<br>
                                8:00AM – 8:00PM<br><br>

                                info@pandaydigital.xyz
                            </p>
                        </v-col>         
                        <v-col cols="12 " md="4" lg="2" sm="6">
                            <h2 class="white--text font-weight-thin">Trusted by</h2><br>
                                <img @click="$router.push('/')" :src="require(`~/assets/resources/reseta-logo.png`)" alt="" width="50%" style="width: 50%;mar" >
                        </v-col>                                    
                        <v-col cols="12 text-right" md="4" lg="2" sm="6" >
                            <h2 class="pb-10 white--text font-weight-thin">Connect to Us!</h2><br>
                            <v-row id="">
                                <v-col cols="12 d-flex">
                                    <v-row>
                                        <v-col cols="3">
                                            <svg fill="#fff" xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 50 50" width="50px" height="50px"><path d="M 25 2 C 12.309295 2 2 12.309295 2 25 C 2 37.690705 12.309295 48 25 48 C 37.690705 48 48 37.690705 48 25 C 48 12.309295 37.690705 2 25 2 z M 25 4 C 36.609824 4 46 13.390176 46 25 C 46 36.609824 36.609824 46 25 46 C 13.390176 46 4 36.609824 4 25 C 4 13.390176 13.390176 4 25 4 z M 16 12 C 14.35499 12 13 13.35499 13 15 C 13 16.64501 14.35499 18 16 18 C 17.64501 18 19 16.64501 19 15 C 19 13.35499 17.64501 12 16 12 z M 16 14 C 16.564129 14 17 14.435871 17 15 C 17 15.564129 16.564129 16 16 16 C 15.435871 16 15 15.564129 15 15 C 15 14.435871 15.435871 14 16 14 z M 14 19 A 1.0001 1.0001 0 0 0 13 20 L 13 35 A 1.0001 1.0001 0 0 0 14 36 L 18 36 A 1.0001 1.0001 0 0 0 19 35 L 19 20 A 1.0001 1.0001 0 0 0 18 19 L 14 19 z M 22 19 A 1.0001 1.0001 0 0 0 21 20 L 21 35 A 1.0001 1.0001 0 0 0 22 36 L 26 36 A 1.0001 1.0001 0 0 0 27 35 L 27 27.5 C 27 26.120455 28.120455 25 29.5 25 C 30.879545 25 32 26.120455 32 27.5 L 32 30 L 32 35 A 1.0001 1.0001 0 0 0 33 36 L 37 36 A 1.0001 1.0001 0 0 0 38 35 L 38 26.5 C 38 22.36961 34.63039 19 30.5 19 C 29.213528 19 28.059744 19.41615 27 19.990234 A 1.0001 1.0001 0 0 0 26 19 L 22 19 z M 15 21 L 17 21 L 17 34 L 15 34 L 15 21 z M 23 21 L 25 21 L 25 21.816406 A 1.0001 1.0001 0 0 0 26.693359 22.537109 C 27.684186 21.585305 29.016683 21 30.5 21 C 33.54961 21 36 23.45039 36 26.5 L 36 34 L 34 34 L 34 30 L 34 27.5 C 34 25.029545 31.970455 23 29.5 23 C 27.029545 23 25 25.029545 25 27.5 L 25 34 L 23 34 L 23 21 z"/></svg>                                              
                                        </v-col>
                                        <v-col cols="3">
                                            <svg fill="#fff" xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 50 50" width="50px" height="50px"><path d="M 25 2 C 12.309295 2 2 12.309295 2 25 C 2 37.690705 12.309295 48 25 48 C 37.690705 48 48 37.690705 48 25 C 48 12.309295 37.690705 2 25 2 z M 25 4 C 36.609824 4 46 13.390176 46 25 C 46 36.609824 36.609824 46 25 46 C 13.390176 46 4 36.609824 4 25 C 4 13.390176 13.390176 4 25 4 z M 30.693359 14.058594 C 27.093054 14.058594 24.152344 16.998175 24.152344 20.597656 C 24.152344 20.622956 24.159856 20.646615 24.160156 20.671875 C 20.346071 20.164308 16.972078 18.281343 14.654297 15.439453 A 1.0001 1.0001 0 0 0 13.015625 15.568359 C 12.452734 16.536013 12.130859 17.663768 12.130859 18.857422 C 12.130859 19.919597 12.426761 20.906321 12.878906 21.796875 A 1.0001 1.0001 0 0 0 12.085938 22.773438 L 12.085938 22.84375 C 12.085938 24.777783 12.990963 26.452789 14.332031 27.652344 A 1.0001 1.0001 0 0 0 14.072266 28.677734 C 14.630704 30.41466 15.93241 31.774479 17.5625 32.541016 C 16.258408 33.150994 14.861087 33.587891 13.320312 33.587891 C 12.909515 33.587891 12.510187 33.564538 12.119141 33.517578 A 1.0001 1.0001 0 0 0 11.460938 35.353516 C 14.065405 37.024617 17.166795 38 20.490234 38 C 25.860882 38 30.105907 35.743874 32.943359 32.525391 C 35.780812 29.306907 37.253906 25.153083 37.253906 21.240234 C 37.253906 21.122724 37.248494 21.01029 37.246094 20.894531 C 38.219933 20.11274 39.135827 19.250444 39.830078 18.210938 A 1.0001 1.0001 0 0 0 38.705078 16.699219 C 38.866705 16.38464 39.095491 16.111528 39.205078 15.769531 A 1.0001 1.0001 0 0 0 37.744141 14.603516 C 36.869551 15.121731 35.886845 15.463383 34.869141 15.701172 C 33.725772 14.727018 32.30529 14.058594 30.693359 14.058594 z M 30.693359 16.058594 C 32.005547 16.058594 33.178321 16.606981 34.005859 17.490234 A 1.0001 1.0001 0 0 0 34.927734 17.789062 C 35.079649 17.759183 35.201682 17.662443 35.351562 17.626953 C 35.332963 17.638463 35.321514 17.658672 35.302734 17.669922 A 1.0001 1.0001 0 0 0 35.832031 19.527344 C 35.763341 19.579724 35.722335 19.662323 35.652344 19.712891 A 1.0001 1.0001 0 0 0 35.238281 20.566406 C 35.247781 20.79066 35.253906 21.015832 35.253906 21.240234 C 35.253906 24.645385 33.939657 28.371609 31.443359 31.203125 C 28.947059 34.03464 25.308587 36 20.490234 36 C 18.837046 36 17.2817 35.669687 15.800781 35.167969 C 17.643043 34.77762 19.387244 34.125203 20.816406 33.003906 A 1.0001 1.0001 0 0 0 20.21875 31.21875 C 18.803099 31.19304 17.712807 30.392345 16.898438 29.359375 C 17.197615 29.320665 17.507049 29.319275 17.792969 29.240234 A 1.0001 1.0001 0 0 0 17.724609 27.294922 C 16.073199 26.96164 14.784996 25.723029 14.3125 24.121094 C 14.7378 24.223448 15.110445 24.452375 15.5625 24.466797 A 1.0001 1.0001 0 0 0 16.150391 22.636719 C 14.930654 21.821102 14.130859 20.439709 14.130859 18.857422 C 14.130859 18.530423 14.306329 18.270522 14.371094 17.964844 C 17.211591 20.776703 20.99183 22.6429 25.248047 22.857422 A 1.0001 1.0001 0 0 0 26.271484 21.628906 C 26.193654 21.29976 26.152344 20.956387 26.152344 20.597656 C 26.152344 18.079138 28.173664 16.058594 30.693359 16.058594 z"/></svg>
                                        </v-col>
                                        <v-col cols="3">
                                            <svg fill="#fff" xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 50 50" width="50px" height="50px"><path d="M 25 3 C 12.861562 3 3 12.861562 3 25 C 3 36.019135 11.127533 45.138355 21.712891 46.728516 L 22.861328 46.902344 L 22.861328 29.566406 L 17.664062 29.566406 L 17.664062 26.046875 L 22.861328 26.046875 L 22.861328 21.373047 C 22.861328 18.494965 23.551973 16.599417 24.695312 15.410156 C 25.838652 14.220896 27.528004 13.621094 29.878906 13.621094 C 31.758714 13.621094 32.490022 13.734993 33.185547 13.820312 L 33.185547 16.701172 L 30.738281 16.701172 C 29.349697 16.701172 28.210449 17.475903 27.619141 18.507812 C 27.027832 19.539724 26.84375 20.771816 26.84375 22.027344 L 26.84375 26.044922 L 32.966797 26.044922 L 32.421875 29.564453 L 26.84375 29.564453 L 26.84375 46.929688 L 27.978516 46.775391 C 38.71434 45.319366 47 36.126845 47 25 C 47 12.861562 37.138438 3 25 3 z M 25 5 C 36.057562 5 45 13.942438 45 25 C 45 34.729791 38.035799 42.731796 28.84375 44.533203 L 28.84375 31.564453 L 34.136719 31.564453 L 35.298828 24.044922 L 28.84375 24.044922 L 28.84375 22.027344 C 28.84375 20.989871 29.033574 20.060293 29.353516 19.501953 C 29.673457 18.943614 29.981865 18.701172 30.738281 18.701172 L 35.185547 18.701172 L 35.185547 12.009766 L 34.318359 11.892578 C 33.718567 11.811418 32.349197 11.621094 29.878906 11.621094 C 27.175808 11.621094 24.855567 12.357448 23.253906 14.023438 C 21.652246 15.689426 20.861328 18.170128 20.861328 21.373047 L 20.861328 24.046875 L 15.664062 24.046875 L 15.664062 31.566406 L 20.861328 31.566406 L 20.861328 44.470703 C 11.816995 42.554813 5 34.624447 5 25 C 5 13.942438 13.942438 5 25 5 z"/></svg>                                               
                                        </v-col>  
                                    </v-row>                                                                                                                
                                </v-col>
                            </v-row>
                        </v-col>
                        <v-col cols="12" sm="6" md="4" lg="2">
                            <h2 class="pb-10 white--text font-weight-thin">Quick links</h2><br>
                            <nuxt-link to="/"><p class="font-weight-regular black--text text-xl-h2 text-lg-h3 text-md-h5 text-sm-h2 footer-custom-css">HOME</p></nuxt-link>
                            <nuxt-link to="offers"><p class="font-weight-regular black--text text-xl-h1 text-lg-h1 text-md-h5 text-sm-h2 ">OFFERS</p></nuxt-link>
                            <!--<nuxt-link to="article"> <h1 class="font-weight-regular black--text text-xl-h1 text-lg-h1 text-md-h5 text-sm-h2">ARTICLE</h1></nuxt-link>-->
                            <v-expansion-panels class="elevation-0">
                                <v-expansion-panel class="elevation-0 background-transparent">
                                    <v-expansion-panel-header class="footer-services">
                                            <nuxt-link  class="text-left" to="services"><p class="text-left font-weight-regular black--text text-xl-h1 text-lg-h1 text-md-h5 text-sm-h2">SERVICES</p></nuxt-link>  
                                    </v-expansion-panel-header>
                                    <v-expansion-panel-content class="custom-css">
                                            <nuxt-link to="Web-Dev"><p class="font-weight-regular black--text text-xl-h2 text-lg-h2">WEB DEV</p></nuxt-link><br>
                                            <nuxt-link to="SEO"><p class="font-weight-regular black--text text-xl-h2 text-lg-h2">SEO</p></nuxt-link><br>
                                            <nuxt-link to="local-seo"><p class="font-weight-regular black--text text-xl-h2 text-lg-h2">Local SEO</p></nuxt-link>
                                    </v-expansion-panel-content>
                                </v-expansion-panel>
                            </v-expansion-panels>               
                            <nuxt-link to="contact"><p class="font-weight-regular black--text text-xl-h1 text-lg-h1 text-md-h5 text-sm-h2 footer-custom-css">CONTACT US</p></nuxt-link>
                        </v-col>                             
                    </v-row>
                </v-col>                 
                <v-col cols="12  pt-10">
                    <v-row>
                        <v-col cols="12" md="4"  class="px-0 center justify-center text-center"> 
                            <p class="text-subtitle-2 white--text font-weight-light text-lg-h5 text-md-h6 text-sm-h4">©2021 Panday Digital. All Rights Reserved.</p>
                        </v-col>
                        <v-col cols="12" md="4" class="text-center"> 
                            <div class="d-block text-center mx-auto" id="Footer-logo">
                                <h1>PANDAY DIGITAL</h1>
                                <p class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-light">we build you digital presence
                                </p>
                            </div>
                        </v-col>
                        <v-col cols="12 justify-center" md="4"  class="center ">  
                                <span class="white--text"><NuxtLink to="/" class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-regular">Privacy Policy</NuxtLink ></span>
                                <span class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-regular">&nbsp; | &nbsp;</span>
                                <span class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-regular"><NuxtLink to="/" class="white--text"
                                >Terms & Conditions</NuxtLink ></span>
                        </v-col>                                        
                    </v-row>
                </v-col>
            </v-row>
        </v-container>
    </v-main>
</template>

<script>
//:style="themecolor"
import { mapState } from 'vuex'
export default {
    data() {
        return {
           //
        }
    },
//    computed: {
//        ...mapState({
//            themecolor: (state) => state.themecolor
//        })
//    },
//    mounted() {
//        console.log(this.themecolor)
//    }
}
</script>

<style>
.footer-services i {
    color: white !important;
}
.footer-services {
    padding: 0px;
    text-align: inherit;
    width: 120px;
}
.footer-custom-css {
    margin-bottom: 10px !important;
}
.background-transparent {
    background: transparent !important;
}
.font-weight-thin{
    font-weight: 300 ;
}
.justify-center{
    justify-content: center;
}
@keyframes rotate {
    from {transform: rotate(0deg);}
    to {transform: rotate(360deg);}
}
.svg {
    transition-property: transform;
    transition-duration: 2s;
}
.svg:hover {
    animation-name: rotate; 
    animation-duration: 2s; 
    animation-iteration-count: infinite;
    animation-timing-function: linear;
}
.white--text{
    color: #fff !important;
}
#Footer-logo h1{
    color: #fff !important;
}
#Footer-logo{
    margin: auto;
}
.mb-10{
    margin-bottom: 10px !important;
}
.my-1{
    margin:0 1% !important;
}
.Footer-color.v-sheet {
    background:transparent;
}

#app .v-application--wrap{
    min-height: 100% !important;
    
}
</style>