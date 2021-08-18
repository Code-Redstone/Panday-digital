<template>
    <v-container class="regestrationForm" :class="$route.path.replace(/\\|\//g,'')">
        <v-row>
            <v-col cols="12" class="custom-height">
                <h3 class="font-weight-bold text-xl-h4 text-lg-h5 text-md-h6 text-sm-h4 pt-5">Digital Marketing Proposal</h3>
            </v-col>
            <v-col cols="12 " class="py-0">
                <p class="ma-0 font-weight-light text-xl-h4 text-lg-h5 text-md-h5 text-sm-h5">Fields with an asterisk (*) are compulsory.</p>
            </v-col>              
            <v-col cols="12" lg="6" class="custom-width">
                <v-text-field label="Full name" auto-grow outlined rows="2" row-height="15">
                </v-text-field>
            </v-col>
            <v-col cols="12" lg="6" class="custom-width">
                <v-text-field label="Name of Business" auto-grow outlined rows="2" row-height="15">
                </v-text-field>
            </v-col>
            <v-col cols="12" lg="6"  class="custom-width">
                <v-text-field label="E-mail address" auto-grow outlined rows="2" row-height="15">
                </v-text-field>
            </v-col>
            <v-col cols="12" lg="6" class="custom-width">
                <v-text-field
                label="Phone number" 
                auto-grow outlined 
                rows="2" 
                row-height="15">
                </v-text-field>
            </v-col>
            <v-col cols="12 " class="pb-0">
                <p class="font-weight-medium mb-0 mt-5 text-xl-h4 text-lg-h5 text-md-subtitle-1 text-sm-h5">What Services Can We Help You With?</p>
            </v-col>
            <v-col cols="12 " class="">
                <v-container>
                    <v-row>
                        <v-col cols="12" lg="6" class="py-0">
                            <v-checkbox
                            label="Search Engine Optimization"
                            color="blue "
                            value="optimization"
                            hide-details
                            ></v-checkbox>
                        </v-col>
                        <v-col cols="12" lg="6" class="py-0">
                            <v-checkbox
                            label="Online Reputation Management"
                            color="blue "
                            value="reputation_management"
                            hide-details
                            ></v-checkbox>
                        </v-col>
                        <v-col cols="12" lg="6"  class="py-0">
                            <v-checkbox
                            label="Web Design & Development"
                            color="blue "
                            value="web_development"
                            hide-details
                            ></v-checkbox>
                        </v-col>
                        <v-col cols="12" lg="6"  class="py-0">
                            <v-checkbox
                            label="Social Media Management"
                            color="blue "
                            value="media_management"
                            hide-details
                            ></v-checkbox>
                        </v-col>
                        <v-col cols="12" lg="6"  class="py-0">
                            <v-checkbox 
                            label="Search Engine Marketing"
                            color="blue "
                            value="marketing"
                            hide-details
                            ></v-checkbox>
                        </v-col>
                        <v-col cols="12" lg="6"  class="py-0">
                            <v-checkbox
                            label="Content Writing Management"
                            color="blue "
                            value="content_writing"
                            hide-details
                            ></v-checkbox> 
                        </v-col>
                        <v-col cols="12" class="custom-width">
                            <v-text-field
                            label="E-mail"
                            auto-grow 
                            outlined 
                            rows="2" 
                            row-height="15">
                            </v-text-field>
                        </v-col>                         
                    </v-row>
                </v-container>
            </v-col>
            <v-col cols="12">
                <v-btn id="Regestrationbutton" color="blue" 
                class="px-lg-15 py-lg-10 px-md-15 py-md-10 px-sm-15 py-sm-10 px-0 py-10 Responsivebutton" :class="$route.path.replace(/\\|\//g,'')"
                elevation="1"
                ><span class="white--text font-weight-light text-justify text-xl-h6 text-lg-h6 text-md-subtitle-2 text-sm-h5">LET THE EXPERTS ASSIST YOU</span>
                </v-btn>             
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
     name:'RegestrationForm',
}
</script>

<style>
#webdevregestration button.SEO{
    background-color: #5c6bc0 !important;
}
#webdevregestration button.Web-Dev{
    background-color: #3949ab !important;
}
#webdevregestration button.offers{
    background-color: #00bcd4 !important;
}
#webdevregestration button.SEO{
    background-color: #5c6bc0 !important;
}
#webdevregestration button.SEO{
    background-color: #5c6bc0 !important;
}
#webdevregestration button.SEO{
    background-color: #5c6bc0 !important;
}
#webdevregestration button.SEO{
    background-color: #5c6bc0 !important;
}
.regestrationForm.offers,
.regestrationForm.offers input,
.regestrationForm.offers fieldset,
.regestrationForm.offers label,
.regestrationForm.offers i,
.regestrationForm.offers li::before{
    color: white !important;
}
</style>