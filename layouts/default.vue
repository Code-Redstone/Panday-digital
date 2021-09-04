<template>
  <div>
    <Header @open="openMenu" @close="closeMenu"/>
    <div class="full" ref="full">
      <Nuxt />
    </div>
    <div class="change-background" :class="$route.path.replace(/\\|\//g,'')" ref="footer">
      <Footer />
    </div>
  </div>
</template>
<script>
export default {
  methods: {
    openMenu() {
      this.$refs.full.style.transform = "translate3d(-300px, 0,0)"
    },
    closeMenu() {
      this.$refs.full.style.transform = "none"
    }
  }
}

</script>
<style>
.change-background p{
  color: #fff;
}
.change-background{
  background-color: #64B5F6;
}
.local-seo{
  background-color: #5c6bc0 !important;
}
.offers {
  background-color: #00BCD4  !important;
}
.contact {
  background-color: #009688 !important;
}
.Web-Dev {
  background-color: #3949ab !important;
}
.services {
  background-color:#5e35b1  !important;
}
.SEO {
  background-color:#5C6BC0  !important;
}
*{
  font-family: sans-serif;
}
.full {
  transition: transform .4s cubic-bezier(0.77, 0.2, 0.05, 1) ;
}
body{
  background: #EEE;
}
a{
  text-decoration: none;
}
p{
  margin-bottom: 15px;
}
p:last-of-type{
  margin-bottom: 0px;
}
.change-background {
    padding: 70px 0px;
}
.footerIMG{
  margin: 14px auto 0px;
}
.text-center{
  text-align: center;
}
#socialmediaicons{
  width: 70%;
  margin: auto;
}

</style>
