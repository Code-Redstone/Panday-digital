<template>
    <form action="">
        <v-container>
            <v-row class="pb-15">
                <v-col cols="12" class="custom-height">
                    <h1 class="font-weight-regular text-xl-h2 text-lg-h3 text-md-h6 text-sm-h4 pt-5">Write to us!</h1>
                </v-col>
                <v-col cols="6" class="custom-width ">
                    <v-text-field v-model="name"  label="Name" auto-grow outlined rows="2" row-height="15" class="rounded-xl">
                    </v-text-field>
                </v-col>
                <v-col cols="6" class="custom-width">
                    <v-text-field v-model="email"  label="Email" auto-grow outlined rows="2" row-height="15" class="rounded-xl">
                    </v-text-field>
                </v-col>
                <v-col cols="6" class="custom-width">
                    <v-text-field v-model="company"  label="Company" auto-grow outlined rows="2" row-height="15" class="rounded-xl">
                    </v-text-field>
                </v-col>
                <v-col cols="6" class="custom-width">
                    <v-text-field v-model="phone"  label="Phone"  class="rounded-xl"  auto-grow outlined rows="2" row-height="15">
                    </v-text-field>
                </v-col>
                <v-col cols="12" class="pb-0">
                    <v-textarea v-model="message"  label="Message" class="rounded-xl"  auto-grow outlined  >
                    </v-textarea>
                </v-col>
                <v-col cols="12" class="py-0 pl-5">
                    <v-btn type="submit"  class="teal px-10 py-5" color="white" auto-grow outlined @click.prevent="send">
                         Submit
                    </v-btn>
                </v-col>
            </v-row>
        </v-container>
    </form>
</template>

<script>
export default {
     name:'ContactForm',
    data: () => ({
        name:'',
        email: '',
        company:'',
        phone: '',
        message:'',
        emailcontent:'',

    }),
    methods: {
        send() {
            this.emailcontent ="Contact Form" + '  ///'
            this.emailcontent += "Name: " + this.name + '  ///'
            this.emailcontent += "Email:" + this.email + '  ///'
            this.emailcontent += "Company:" + this.company + '  ///'
            this.emailcontent += "Phone:" + this.phone  + '  ///'
            this.emailcontent += "Message:" + this.message 
            this.$mail.send({
                from: this.email,
                subject: 'Contact form message',
                text: this.emailcontent,
            })
        }
    },
}
</script>

<style>

</style>