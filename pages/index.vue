<template>
<div>
  <Header/>
  <div class="container">
  <Slide/>
  </div>
</div>
</template>

<script>
import Header from '~/components/Header/Header'
import Slide from '~/components/SlideShow/Slide'


export default {
  components: {
    Header,
    Slide
  }
}
</script>