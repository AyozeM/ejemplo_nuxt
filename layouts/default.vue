<template>
  <div>
    <navbar/>
    <nuxt/>
    <Footer/>
  </div>
</template>

<script>
import navbar from '~/components/header'
import Footer from '~/components/footer'
export default {
  components: { navbar, Footer }
}
</script>
