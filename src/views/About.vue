<template>
  <div class="about">
    <AboutNav></AboutNav>
    <AboutContent></AboutContent>
  </div>
</template>
<script>
import AboutNav from '../components/AboutNav'
import AboutContent from '../components/AboutContent'
export default {
  components: {
    AboutContent,
    AboutNav
  }
}
</script>
