<template>
  <header ref="header" class="center" id="header"> 
	  <div class="container d-flex">
		<div class="mainmenu">
            <div class="Mdn">
                <v-row>
                    <v-col cols="9">
                       <img @click="$router.push('/')" :src="require(`~/assets/resources/Panday-digital-long2.png`)" alt="" width="100%" style="width: 55%;" >
                    </v-col>
                    <v-col cols="3 d-flex">
                        <nav class="float Mauto0AutoAuto">
                            <div id="menuToggle" class="Mauto0AutoAuto">
                                <!--
                                A fake / hidden checkbox is used as click reciever,
                                so you can use the :checked selector on it.
                                -->
                                <input type="checkbox" @click="burgerClick" v-model="inputBurger"/>
                                
                                <!--
                                Some spans to act as a hamburger.
                                
                                They are acting like a real hamburger,
                                not that McDonalds stuff.
                                --> 
                                <span></span>
                                <span></span>                             
                                <span></span>
                                
                                <!--
                                Too bad the menu has to be inside of the button
                                but hey, it's pure CSS magic.
                                -->
                                <ul id="menu">                                 
                                    <nuxt-link to="/"><h1 @click="onMenuClick" class="font-weight-regular black--text text-xl-h2 text-lg-h3 text-md-h5 text-sm-h2">HOME</h1></nuxt-link>
                                    <nuxt-link to="offers"><h1 @click="onMenuClick" class="font-weight-regular black--text text-xl-h1 text-lg-h1 text-md-h5 text-sm-h2">OFFERS</h1></nuxt-link>
                                    <!--<nuxt-link to="article"> <h1 class="font-weight-regular black--text text-xl-h1 text-lg-h1 text-md-h5 text-sm-h2">ARTICLE</h1></nuxt-link>-->
                                    <v-expansion-panels class="elevation-0 customcss">
                                        <v-expansion-panel class="elevation-0">
                                            <v-expansion-panel-header class="elevation-0" >
                                                    <nuxt-link  class="text-left" to="services"><h1 @click="onMenuClick" class=" font-weight-regular black--text text-xl-h1 text-lg-h1 text-md-h5 text-sm-h2">SERVICES</h1></nuxt-link>  
                                            </v-expansion-panel-header>
                                            <v-expansion-panel-content>
                                                    <nuxt-link to="Website-development"><h4 @click="onMenuClick" class="font-weight-regular black--text text-xl-h2 text-lg-h2">WEBSITE DEVELOPMENT</h4  ></nuxt-link><br>
                                                    <nuxt-link to="SEO"><h4 @click="onMenuClick" class="font-weight-regular black--text text-xl-h2 text-lg-h2">SEO</h4></nuxt-link>
                                                    <nuxt-link to="local-seo"><h4 @click="onMenuClick" class="font-weight-regular black--text text-xl-h2 text-lg-h2">Local SEO</h4></nuxt-link>
                                            </v-expansion-panel-content>
                                        </v-expansion-panel>
                                    </v-expansion-panels>               
                                    <nuxt-link to="contact"><h1 @click="onMenuClick" class="font-weight-regular black--text text-xl-h1 text-lg-h1 text-md-h5 text-sm-h2">CONTACT US</h1></nuxt-link>
                                </ul>
                            </div>
                        </nav> 
                    </v-col>
                </v-row>
            </div> 
            <div class="Ddn">
                <v-row>
                    <v-col cols="3 center">
                        <img  @click="$router.push('/')" :src="require(`~/assets/resources/Panday-digital-long2.png`)" alt="" width="90%">
                    </v-col>
                    <v-col cols="9" class="d-flex">
                        <nav class="float Ddn Mauto0AutoAuto">
                            <nuxt-link to="/"><h1 class="font-weight-regular black--text text-xl-h2 text-lg-h3 text-md-h6 text-sm-h2">HOME</h1></nuxt-link>
                            <nuxt-link to="offers"><h1 class="font-weight-regular black--text text-xl-h1 text-lg-h1 text-md-h5 text-sm-h2">OFFERS</h1></nuxt-link>
                            <div class="dropdown">
                                <button class="dropbtn">
                                    <nuxt-link to="services"><h1 class=" font-weight-regular black--text text-xl-h1 text-lg-h1 text-md-h5 text-sm-h2">SERVICES</h1></nuxt-link>
                                </button>
                                <div class="dropdown-content">
                                    <nuxt-link to="Website-development"><h4 class=" font-weight-regular black--text text-xl-h2 text-lg-h2">WEBSITE DEVELOPMENT</h4></nuxt-link>
                                    <nuxt-link to="SEO"><h4 class="font-weight-regular black--text text-xl-h2 text-lg-h2">SEO</h4></nuxt-link>
                                    <nuxt-link to="local-seo"><h4 @click="onMenuClick" class="font-weight-regular black--text text-xl-h2 text-lg-h2">Local SEO</h4></nuxt-link>
                                </div>
                            </div>
                            <!--<nuxt-link to="article"> <h1 class="font-weight-regular black--text text-xl-h1 text-lg-h1 text-md-h5 text-sm-h2">ARTICLE</h1></nuxt-link>-->
                            <nuxt-link to="contact"><h1  class="font-weight-regular black--text text-xl-h1 text-lg-h1 text-md-h5 text-sm-h2">CONTACT US</h1></nuxt-link>
                        </nav>
                    </v-col>
                </v-row>
            </div>
		</div>
	  </div>
  </header>
</template>

<script>
export default {
    data() {
        return {
            mobilemenu:true,
            inputBurger:false,
        }
    },
    methods: {
        burgerClick(e) {
            if(e.target.checked)
                this.$emit('open')
            else
                this.$emit('close')
        },
        handleScroll (event) {
            let bottomOfWindow = document.documentElement.scrollTop >= 100

            if (bottomOfWindow) {
                this.$refs.header.style="height: 100px;width: 100%;background-color: white;font-size: 14px;"
            }
            else {
                this.$refs.header.style="height: 150px;width: 100%;background-color: white;font-size: 16px;"
            }
            
        },
        onMenuClick (as) {
            this.inputBurger=!this.inputBurger
            this.burgerClick(as)
        } 
    },
    mounted () {
        window.addEventListener('scroll', this.handleScroll);
    },
    destroyed () {
        window.removeEventListener('scroll', this.handleScroll);
    },

}
</script>

<style lang="scss">
.v-expansion-panel.elevation-0::before {
    box-shadow: unset !important;
}
.customcss::after{
    border: unset !important;
}
.customcss a {
    margin: 0px !important;
}

.customcss {
    width: 40%;
}
.customcss button {
    padding: 0px !important;
    text-align: left;
}
.dropdown {
  float: left;
  overflow: hidden;
}

.dropdown .dropbtn {
  font-size: 16px;  
  border: none;
  outline: none;
  color: black;
  background-color: inherit;
  font-family: inherit;
  margin: 0;
}
.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 100px;
  z-index: 1;  
  padding: 10px 0;
}

.dropdown-content a {
  text-align: center;
  float: none;
  color: black;
  text-decoration: none;
  display: block;
  text-align: left;
}
.dropdown:hover .dropdown-content{
  display: block;
}
header{
    height: 150px;
    width: 100%;
    background-color: white;
    font-size: 16px;
}
header.center {
    box-shadow: 11px 10px 42px #6363632b;
}
header{
    transition: .5s
}
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

  $color-pack: false;

  @import '~vuetify/src/styles/main.sass';
    @media screen and (max-width:1264px) {
        header#header {
            height: 100px !important;
        }
        .MTM-150px{
            margin-top: 100px !important;
        }
    }
    @media screen and (max-width:700px) {
        #offersheroimage{
            width: 100% !important;
        }
        .Dn700{
            display: none !important;
        }
        header#header {
            height: 100px !important;
        }
    }
  @media screen and (max-width:400px) {
      .Responsivebutton {
        padding: 10px 10px 10px 10px !important;
        width: 100% !important;
    }
    #px400-adjust{
        padding: 10px !important;
    }

  }
  @media screen and (max-width:1264px) and (min-width:10px) {
    .desktop-main,
    .Ddn{
        display: none !important;
    }
    .mainmenu img {
        display: flex;
        align-self: center;
    }
    .M-textCenter{
        text-align: center;
    }
    #Hero-Description,
    #hero-homepage{
        text-align: center !important;
        padding-top: 50px;
    }
    .TAC{
        text-align: center !important;
    }
  }
    @media screen and (min-width:1265px) {
    .Mdn{
        display: none !important;
    }
    .MTM-150px{
        margin-top: 150px;
    }
  }

p{
    font-weight: 300;
}
.custom-width {
    height: 65px;
}
.Mauto0AutoAuto{
    margin: auto 0 auto auto;
}
h1,
h2,
h3,
h4,
h5,
h6,
p,
li,
a{
    font-family: 'Roboto', sans-serif;
}
nav.float {
    text-transform: uppercase;
}
.first-section h3, .first-section h1, .first-section p {
    color: white;
}
.mainmenu {
    width: 100%;
}
nav {
	display: flex;
	align-items: center;
}
nav a {
	display: block;
	color:#000;
}
.float-left{
	float: right !important;
}
header { 
    z-index: 9;
    position: fixed;
}
.title {
    font-weight: 900;
    font-size: 34px;
}
.radius {
    display: flex;
    align-items: center;
}
.Rounded-botton span {
    margin: 0px !important;
}
.first-section {
    position: relative;
    bottom: -20px;
}
.first-section h3 {
    font-weight: 300;
}
.first-section h1 {
    font-size: 38px;
}
.d-flex{
    align-items: center !important;
    display: flex;
}
#menuToggle span {
    display: block;
    width: 35px;
    height: 5px;
    margin-bottom: 3px;
    position: relative;
    background: #000000;
    border-radius: 3px;
    z-index: 1;
    transform-origin: 4px 0px;
    transition: transform 0.5s cubic-bezier(0.77, 0.2, 0.05, 1), background 0.5s cubic-bezier(0.77, 0.2, 0.05, 1), opacity 0.55s ease;
}
#menuToggle input {
    display: block;
    width: 58px;
    height: 39px;
    position: absolute;
    cursor: pointer;
    opacity: 0;
    z-index: 2;
    -webkit-touch-callout: none;
}
#menu {
    right: -200px;
    top: 56px;
    position: absolute;
    width: 500px;
    height: 1192px;
    padding: 33px;
    padding-top: 51px;
    background: #ffffff;
    list-style-type: none;
    -webkit-font-smoothing: antialiased;
    transform-origin: 0% 0%;
    transition: transform 0.5s cubic-bezier(0.77, 0.2, 0.05, 1);
    transform: translate(134%, 0);
}
#menuToggle {
    display: block;
    position: relative;
    z-index: 1;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
}
#menuToggle input:checked ~ span {
    opacity: 1;
    transform: rotate(45deg) translate(0px, -6px);
    background: #232323;
}
#menuToggle input:checked .testing{
    right: 300px;
}
#menuToggle input:checked ~ ul
{
  transform: none;
}

/*
 * But let's hide the middle one.
 */
#menuToggle input:checked ~ span:nth-last-child(3)
{
  opacity: 0;
  transform: rotate(0deg) scale(0.2, 0.2);
}

/*
 * Ohyeah and the last one should go the other direction
 */
#menuToggle input:checked ~ span:nth-last-child(2) {
    transform: rotate(-45deg) translate(0, -1px);
}
.v-responsive__content {
    width: 100% !important;
}
ul#menu a {
    margin-left: 0px !important;
    margin-top: 10px;
}
ul#menu a:last-child {
    margin-left: 0px !important;
    margin-bottom: 9px !important;
    margin-top: -3px !important;
}
div#third-section .container .row div:last-child {
    margin: auto;
}
nav.float.Ddn.Mauto0AutoAuto a:hover {
    background: #dedede;
    transition: .2s;
}
nav.float.Ddn.Mauto0AutoAuto a {
    padding: 9px 24px;
}
</style>