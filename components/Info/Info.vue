<template>
  <div class="info-container">
    <h2>{{title}}</h2>
    <h3>{{subtitle}}</h3>
    <p class="line"></p>
    <p style="text-align: center">{{text}}</p>
  </div>
</template>
<script>
export default {
  name: 'info',
  props: {
    title: {
      type: String,
    },
    subtitle: {
      type: String,
    },
    text: {
      type: String,
    }
  }
}
</script>
<style scoped>
.info-container {
  margin-top: 45px;
}
.line {
  border: 1px solid black;
  width: 35%;
  margin: 0px auto 20px auto;
}
h2 {
    text-transform: uppercase;
    color: #ffc000;
    font-size: 2rem;
    margin-bottom: 0;
    text-align: center;
}
h3 {
  font-size: 2rem;
  line-height: 1.4;
  text-transform: uppercase;
  text-align: center;
}
</style>
