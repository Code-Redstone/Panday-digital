<template>
    <form action="">
        <v-container>
            <v-row class="pb-15">
                <v-col cols="12" class="custom-height">
                    <h1 class="font-weight-regular text-xl-h2 text-lg-h3 text-md-h6 text-sm-h4 pt-5">Write to us!</h1>
                </v-col>
                <v-col cols="6" class="custom-width ">
                    <v-text-field label="Name" auto-grow outlined rows="2" row-height="15" class="rounded-xl">
                    </v-text-field>
                </v-col>
                <v-col cols="6" class="custom-width">
                    <v-text-field label="Email" auto-grow outlined rows="2" row-height="15" class="rounded-xl">
                    </v-text-field>
                </v-col>
                <v-col cols="6" class="custom-width">
                    <v-text-field label="Company" auto-grow outlined rows="2" row-height="15" class="rounded-xl">
                    </v-text-field>
                </v-col>
                <v-col cols="6" class="custom-width">
                    <v-text-field
                    class="rounded-xl"
                    label="Phone" 
                    auto-grow outlined 
                    rows="2" 
                    row-height="15">
                    </v-text-field>
                </v-col>
                <v-col cols="12" class="pb-0">
                    <v-textarea
                    class="rounded-xl"
                    label="Message"  
                    auto-grow outlined  >
                    </v-textarea>
                </v-col>
                <v-col cols="12" class="py-0 pl-5">
                    <v-btn
                    type="submit"
                    class="teal px-10 py-5"
                    color="white"
                    auto-grow outlined  >
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
}
</script>

<style>

</style>