<template>
    <v-container class="regestrationForm" :class="$route.path.replace(/\\|\//g,'')">
        <v-row>
            <v-col cols="12" class="custom-height">
                <h3 class="font-weight-bold text-xl-h4 text-lg-h5 text-md-h6 text-sm-h4 pt-5">Digital Marketing Proposal</h3>
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
            <v-col cols="12 " class="pb-0" v-if="$route.name === 'index'">
                <p class="font-weight-medium mb-0 mt-5 text-xl-h4 text-lg-h5 text-md-subtitle-1 text-sm-h5">What Services Can We Help You With?</p>
            </v-col>
            <v-col cols="12 " id="home"  v-if="$route.name === 'index'">
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
                        <v-col cols="12" lg="6"  class="py-0" >
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
                    </v-row>
                </v-container>
            </v-col>
            <v-col cols="12" lg="6"  class="custom-width" id="seo-imputs" v-if="$route.name === 'Website-development'" >
                <h3>Website</h3>
                <v-text-field label="http://" auto-grow outlined rows="2" row-height="15">
                </v-text-field>
            </v-col>
            <v-col cols="12" lg="6"  class="custom-width" id="seo-imputs" v-if="$route.name === 'Website-development'">
                <h3>Your projected budget</h3>
                <v-select
                :items="Web"
                filled
                outlined
                label=""
                ></v-select>
            </v-col>
            <v-col cols="12 " class="pb-0" v-if="$route.name === 'Website-development'">
                <p class="font-weight-medium mb-0 mt-5 text-xl-h4 text-lg-h5 text-md-subtitle-1 text-sm-h5">Web development technologies ?</p>
            </v-col>
            <v-col cols="12 " id="Website-development"  v-if="$route.name === 'Website-development'">
                <v-container>
                    <v-row>
                        <v-col cols="12" lg="6" class="py-0">
                            <v-checkbox
                            label="PHP"
                            color="blue "
                            value="PHP"
                            hide-details
                            ></v-checkbox>
                        </v-col>
                        <v-col cols="12" lg="6" class="py-0">
                            <v-checkbox
                            label="Woocommerce"
                            color="blue "
                            value="Woocommerce"
                            hide-details
                            ></v-checkbox>
                        </v-col>
                        <v-col cols="12" lg="6"  class="py-0">
                            <v-checkbox
                            label="Laravel"
                            color="blue "
                            value="Laravel"
                            hide-details
                            ></v-checkbox>
                        </v-col>
                        <v-col cols="12" lg="6"  class="py-0">
                            <v-checkbox
                            label="Wordpress"
                            color="blue "
                            value="Wordpress"
                            hide-details
                            ></v-checkbox>
                        </v-col>
                        <v-col cols="12" lg="6"  class="py-0" >
                            <v-checkbox 
                            label="Shopify"
                            color="blue "
                            value="Shopify"
                            hide-details
                            ></v-checkbox>
                        </v-col>
                        <v-col cols="12" lg="6"  class="py-0">
                            <v-checkbox
                            label="Others"
                            color="blue "
                            value="Others"
                            hide-details
                            ></v-checkbox> 
                        </v-col>
                    </v-row>
                </v-container>
            </v-col>
            <v-col cols="12" lg="12"  class="" id="seo-imputs" v-if="$route.name === 'SEO'">
                <h3>What is your projected monthly SEO budget?</h3>
                <v-select
                class="custom-width"
                :items="Seo"
                filled
                outlined
                label=""
                ></v-select>
            </v-col>
            <v-col cols="12 py-0 pr-0" v-if="$route.name === 'SEO'">
                <h3>Did you hired any SEO agency/freelancer in the past? *</h3>
                <v-radio-group v-model="row" row >
                    <v-radio
                        class="Seo-radio"
                        label="Yes"
                        value="Yes"
                    ></v-radio>
                    <v-radio
                        class="Seo-radio"
                        label="No"
                        value="No"
                    ></v-radio>
                </v-radio-group>
            </v-col>
            <v-col cols="12 pt-4 pb-0 pr-0" v-if="$route.name === 'SEO'">
                <v-row class="pa-0">
                    <v-col cols="12 py-0 pr-0">
                        <h3 >What SEO services do you need? *</h3>
                    </v-col>
                    <v-col cols="4 py-0">
                        <v-checkbox
                        value="On-Page"
                        >   
                            <template 
                            v-slot:label
                            >On-Page SEO</template>
                        </v-checkbox>
                    </v-col>
                    <v-col cols="4 py-0">
                        <v-checkbox 
                        value="Off-Page"
                        >                    
                            <template 
                            v-slot:label
                            >Off-Page SEO</template>
                        </v-checkbox>
                    </v-col>
                    <v-col cols="4 py-0">
                        <v-checkbox 
                        value="Keywords Research"
                        >                    
                            <template 
                            v-slot:label
                            >Keywords Research</template>
                        </v-checkbox>
                    </v-col>
                </v-row>
            </v-col>
            <v-col cols="12 py-0 pr-0" v-if="$route.name === 'SEO'">
                <h3>How would you describe your business? *</h3>
                <v-radio-group v-model="row" row >
                    <v-radio
                        class="Seo-radio-business"
                        label="Local"
                        value="Local"
                    ></v-radio>
                    <v-radio
                        class="Seo-radio-business"
                        label="National"
                        value="National"
                    ></v-radio>
                    <v-radio
                        class="Seo-radio-business"
                        label="Global"
                        value="Global"
                    ></v-radio>
                </v-radio-group>
            </v-col>
            <v-col cols="12 pt-4 pb-0 pr-0" v-if="$route.name === 'local-seo'">
                <h3>Did you hired any SEO agency/freelancer in the past? *</h3>
                <v-radio-group v-model="row" row >
                    <v-radio
                        class="Seo-radio"
                        label="Yes"
                        value="Yes"
                    ></v-radio>
                    <v-radio
                        class="Seo-radio"
                        label="No"
                        value="No"
                    ></v-radio>
                </v-radio-group>
            </v-col>
             <v-col cols="12 py-0 pr-0" v-if="$route.name === 'local-seo'">
                <v-row class="pa-0">
                    <v-col cols="12 py-0 pr-0">
                        <h3 >What SEO services do you need? *</h3>
                    </v-col>
                    <v-col cols="6 py-0" md="4">
                        <v-checkbox
                        value="On-Page"
                        >   
                            <template 
                            v-slot:label
                            >On-Page SEO</template>
                        </v-checkbox>
                    </v-col>
                    <v-col cols="6 py-0" md="4">
                        <v-checkbox 
                        value="Off-Page"
                        >                    
                            <template 
                            v-slot:label
                            >Off-Page SEO</template>
                        </v-checkbox>
                    </v-col>
                    <v-col cols="6 py-0" md="4">
                        <v-checkbox 
                        value="Keywords Research"
                        >                    
                            <template 
                            v-slot:label
                            >Keywords Research</template>
                        </v-checkbox>
                    </v-col>
                    <v-col cols="6 py-0" md="4">
                        <v-checkbox
                        value="On-Page"
                        >   
                            <template 
                            v-slot:label
                            >Local SEO Audit</template>
                        </v-checkbox>
                    </v-col>
                    <v-col cols="6 py-0" md="4">
                        <v-checkbox 
                        value="Off-Page"
                        >                    
                            <template 
                            v-slot:label
                            >GMB Optimization</template>
                        </v-checkbox>
                    </v-col>
                    <v-col cols="6 py-0" md="4">
                        <v-checkbox 
                        value="Keywords Research"
                        >                    
                            <template 
                            v-slot:label
                            >Social Media Marketing</template>
                        </v-checkbox>
                    </v-col>
                </v-row>
            </v-col>
            <v-col cols="12" class="pb-0">
                <v-textarea
                label="Message"  
                auto-grow outlined  >
                </v-textarea>
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
    props: {
        page:{
            type:String,
            required:true
        }
    },
    methods: {
    send() {
        this.message = "Phone: " + this.phone;
        this.message += "n"
        this.$mail.send({
            from: this.email,
            subject: 'Contact form message',
            text: this.message,
        })
        }
    },
    data: () => ({
      Web: ['₱20,000 - ₱30,000', '₱40,000 - ₱50,000', '₱60,000 - ₱80,000', '₱100,000+'],
      Seo: ['₱20,000 - ₱33,000', '₱40,000 - ₱50,000', '₱60,000 - ₱80,000', '₱100,000+'],
    }),
    
}
</script>

<style>
.Seo-radio-business{
    width: 33.33% !important;
    margin: 0px !important;
}
.Seo-radio{
    width: 50% !important;
    margin: 0px !important;
}
#webdevregestration button.local-seo{
    background-color: #5c6bc0 !important;
}
#webdevregestration button.SEO{
    background-color: #5c6bc0 !important;
}
#webdevregestration button.Website-development{
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