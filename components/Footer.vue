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
                        <p class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-light"><strong>Panday Digital</strong><br>
                            One Global Place,<br>
                            Level 10-1,<br>
                            25th street & 5th Avenue,<br>
                            Bonifacio Global City,<br>
                            Taguig City, 1632 Philippines</p>
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
                                info@digitalmarketingmanila.com
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
                                        <v-img
                                        class="mr-2 footerIMG"
                                        :src="require(`~/assets/resources/in.png`)"
                                        max-height="50px"
                                        max-width="50px"
                                        >
                                            
                                        </v-img>                                                                                                                                   
                                    </v-col>
                                </v-row>
                        </v-col>
                    </v-row>
                </v-col>
                <v-col cols="12  pt-10">
                    <v-row>
                        <v-col cols="12" md="3"  class="center px-0 text-center"> 
                            <p class="text-subtitle-2 white--text font-weight-light text-lg-h5 text-md-h6 text-sm-h4">©2021 Panday Digital. All Rights Reserved.</p>
                        </v-col>
                        <v-col cols="12" md="6" class=" text-center "> 
                            <div class="d-block text-center mx-auto" id="Footer-logo">
                                <h1>PANDAY DIGITAL</h1>
                                <p class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-light">we build you digital pressence
                                </p>
                            </div>
                        </v-col>
                        <v-col cols="12" md="3"  class="center text-center"> 
                            <span class="white--text"><NuxtLink to="/" class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-regular">Privacy Policy</NuxtLink ></span>
                            <span class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-regular">&nbsp; | &nbsp;</span>
                            <span class="white--text text-lg-h5 text-md-h6 text-sm-h4 font-weight-regular"><NuxtLink to="/" class="white--text"
                            >Terms & Conditions</NuxtLink ></span>
                        </v-col>                                        
                    </v-row>
                </v-col>
            </v-row>
        </v-container>
        <v-container  class="Mdn">
            <v-row>
                <v-col sm="4" cols="12">
                    <p class="black--text font-weight-light">
                        <b>Business Hours</b><br>
                        Monday – Saturday<br>
                        8:00AM – 8:00PM<br><br>

                        +63 (977) 366-8544<br>
                        info@pandaydigital.com
                    </p>
                </v-col>
                <v-col sm="4" cols="12" >
                    <p class="black--text font-weight-light">
                        <strong>Panday Digital</strong><br>
                        One Global Place,<br>
                        Level 10-1,<br>
                        25th street & 5th Avenue,<br>
                        Bonifacio Global City,<br>
                        Taguig City, 1632 Philippines
                    </p>
                </v-col>
                <v-col sm="4" cols="12" class="">
                    <v-container>
                        <v-row>
                            <p class="white--text mb-10 text-sm-h4 font-weight-light"><b>Connect to Us!</b></p>
                        </v-row>
                        <v-row class="d-flex">
                        <v-img
                        class="my-1"
                        :src="require(`~/assets/resources/fb.png`)"
                        max-height="50px"
                        max-width="50px"
                        >
                        </v-img>
                        <v-img
                        class="my-1"
                        :src="require(`~/assets/resources/twitter.png`)"
                        max-height="50px"
                        max-width="50px"
                        >
                        </v-img>   
                        <v-img
                        class="my-1"
                        :src="require(`~/assets/resources/in.png`)"
                        max-height="50px"
                        max-width="50px"
                        >
                        </v-img>
                        </v-row>
                    </v-container>
                </v-col>
            </v-row>
            <v-row>
                <v-col sm="4" cols="12">
                    <p class="black--text text-sm-h1 font-weight-light">
                        ©2021 Panday Digital. All Rights Reserved.
                    </p>
                </v-col>
                <v-col sm="4" cols="12" >
                    <p class="black--text font-weight-light">
                        <strong>Panday Digital</strong><br>
                        One Global Place,<br>
                        Level 10-1,<br>
                        25th street & 5th Avenue,<br>
                        Bonifacio Global City,<br>
                        Taguig City, 1632 Philippines
                    </p>
                </v-col>
                <v-col sm="4" cols="12" class="">
                    <v-container>
                        <v-row>
                            <p class="white--text mb-10 text-sm-h4 font-weight-light"><b>Connect to Us!</b></p>
                        </v-row>
                        <v-row class="d-flex">
                        <v-img
                        class="my-1"
                        :src="require(`~/assets/resources/fb.png`)"
                        max-height="50px"
                        max-width="50px"
                        >
                        </v-img>
                        <v-img
                        class="my-1"
                        :src="require(`~/assets/resources/twitter.png`)"
                        max-height="50px"
                        max-width="50px"
                        >
                        </v-img>   
                        <v-img
                        class="my-1"
                        :src="require(`~/assets/resources/in.png`)"
                        max-height="50px"
                        max-width="50px"
                        >
                        </v-img>
                        </v-row>
                    </v-container>
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