<template>
  <div>
    <Header @open="openMenu" @close="closeMenu" />
    <div class="full" ref="full">
      <Nuxt />
    </div>
    <Footer />
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
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;

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
</style>
