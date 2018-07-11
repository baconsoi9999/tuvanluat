<template>
  <nav class="navbar is-fixed-top has-background-white">
      <div class="navbar-brand">
        <a class="navbar-item" href="https://bulma.io">
          <img src="http://eazymarketing.net/wp-content/uploads/2018/06/logo-340x45.png" alt="Bulma: a modern CSS framework based on Flexbox" width="250" height="50">
        </a>
      </div>

    <div id="navbar" class="navbar-end has-text-centered">
       <a  class="active" href=""> <b>TRANG CHỦ  </b></a>
       <a  href="">BÁO GIÁ</a>
       <a  href="">TIN TỨC</a>
      <a  href="">DỰ ÁN</a>
      <a  href="">DỊCH VỤ</a>
      <a  href="">VỀ CHÚNG TÔI</a>
      <a  href="">LIÊN HỆ</a>
    </div>
  </nav>

</template>

<script>
// When the user scrolls down 20px from the top of the document, slide down the navbar


export default {
  components: {
    
  }
}
</script>

<style>
.header {
  background-color: #f1f1f1;
  margin-bottom: 5px;
  text-align: center;
}

#navbar {
  margin-right: 50px;
  overflow: hidden;
}

#navbar a {
  float: right;
  display: block;
  color: black;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}
.navbar {
  padding-left: 20%;
  padding-right: 10%;
}
#navbar a:hover {
  border-top-style: solid;
  border-width: 5px;
  color: #ffc000;
}

#navbar a.active {
  border-top-style: solid;
  border-width: 5px;
  color: #ffc000;
}

</style>
