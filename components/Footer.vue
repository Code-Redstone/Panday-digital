<template>
    <v-main >
        <v-container>
            <v-row>
                <v-col cols="12 py-15">
                    <v-row>
                        <v-col 
                        cols="12"
                        md="4"
                        >
                        <p class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-light text-center"><strong>Panday Digital</strong><br>
                            Purok Jasmin, <br>
                            Barangay Acmac,<br>
                            Iligan City,<br>
                            Lanao del Norte,<br>
                            Mindanao, 9200 Philippines</p>
                        </v-col>
                        <v-col 
                        cols="12 text-center"
                        md="4"
                        >
                            <p class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-light">
                                <b>Business Hours</b><br>
                                Monday – Saturday<br>
                                8:00AM – 8:00PM<br><br>

                                +63 (977) 366-8544<br>
                                info@pandaydigital.xyz
                            </p>
                        </v-col>
                        <v-col cols="12" md="4">
                            <p class="white--text text-center text-lg-h5 text-md-h6 text-sm-h4 font-weight-light"><b>Connect to Us!</b></p>
                                <v-row id="socialmediaicons">
                                    <v-col cols="12 d-flex">
                                        <v-img
                                        class="mr-4 footerIMG"
                                        :src="require(`~/assets/resources/fb.png`)"
                                        max-height="50px"
                                        max-width="50px"
                                        >
                                        </v-img>      
                                        <v-img
                                        class="mr-2 footerIMG"
                                        :src="require(`~/assets/resources/twitter.png`)"
                                        max-height="50px"
                                        max-width="50px"
                                        >

                                        </v-img>   
                                            <svg fill="#000000" xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 50 50" width="50px" height="50px"><path d="M 25 3 C 12.861562 3 3 12.861562 3 25 C 3 36.019135 11.127533 45.138355 21.712891 46.728516 L 22.861328 46.902344 L 22.861328 29.566406 L 17.664062 29.566406 L 17.664062 26.046875 L 22.861328 26.046875 L 22.861328 21.373047 C 22.861328 18.494965 23.551973 16.599417 24.695312 15.410156 C 25.838652 14.220896 27.528004 13.621094 29.878906 13.621094 C 31.758714 13.621094 32.490022 13.734993 33.185547 13.820312 L 33.185547 16.701172 L 30.738281 16.701172 C 29.349697 16.701172 28.210449 17.475903 27.619141 18.507812 C 27.027832 19.539724 26.84375 20.771816 26.84375 22.027344 L 26.84375 26.044922 L 32.966797 26.044922 L 32.421875 29.564453 L 26.84375 29.564453 L 26.84375 46.929688 L 27.978516 46.775391 C 38.71434 45.319366 47 36.126845 47 25 C 47 12.861562 37.138438 3 25 3 z M 25 5 C 36.057562 5 45 13.942438 45 25 C 45 34.729791 38.035799 42.731796 28.84375 44.533203 L 28.84375 31.564453 L 34.136719 31.564453 L 35.298828 24.044922 L 28.84375 24.044922 L 28.84375 22.027344 C 28.84375 20.989871 29.033574 20.060293 29.353516 19.501953 C 29.673457 18.943614 29.981865 18.701172 30.738281 18.701172 L 35.185547 18.701172 L 35.185547 12.009766 L 34.318359 11.892578 C 33.718567 11.811418 32.349197 11.621094 29.878906 11.621094 C 27.175808 11.621094 24.855567 12.357448 23.253906 14.023438 C 21.652246 15.689426 20.861328 18.170128 20.861328 21.373047 L 20.861328 24.046875 L 15.664062 24.046875 L 15.664062 31.566406 L 20.861328 31.566406 L 20.861328 44.470703 C 11.816995 42.554813 5 34.624447 5 25 C 5 13.942438 13.942438 5 25 5 z"/></svg>                                                                                                                     
                                    </v-col>
                                </v-row>
                        </v-col>
                    </v-row>
                </v-col>
                <v-col cols="12  pt-10">
                    <v-row>
                        <v-col cols="12" md="4"  class="px-0 center justify-center"> 
                            <p class="text-subtitle-2 white--text font-weight-light text-lg-h5 text-md-h6 text-sm-h4">©2021 Panday Digital. All Rights Reserved.</p>
                        </v-col>
                        <v-col cols="12" md="4" class="text-center"> 
                            <div class="d-block text-center mx-auto" id="Footer-logo">
                                <h1>PANDAY DIGITAL</h1>
                                <p class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-light">we build you digital pressence
                                </p>
                            </div>
                        </v-col>
                        <v-col cols="12" md="4"  class="center justify-center">  
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