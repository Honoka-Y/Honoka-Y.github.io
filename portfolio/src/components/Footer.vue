<template>
<!-- footer -->
<footer class="footer">
  <div class="copyright">&copy;{{name}}</div>
</footer>
<!-- /footer -->
</template>

<script>
export default {
  name: 'Footer',
  data () {
    return {
      name: 'H.Y'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/*--------------------------------
footer
---------------------------------*/
.footer {
padding: 30px;
background-color: #3a5b52;
}
.copyright {
font-size: 10px;
text-align: center;
color: #fff;
}
/*media Queries 767
--------------------------------------*/
@media screen and (max-width: 767px) {
  /* Footer */
  .footer {
    padding: 20px;
  }
}
</style>
