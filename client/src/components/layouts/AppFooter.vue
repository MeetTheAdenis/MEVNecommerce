<template>
  <footer class="page-footer orange">
    <div class="container">
      <div class="row">
        <div class="col l6 s12">
          <h5 class="white-text">Company Bio</h5>
          <p class="grey-text text-lighten-4">Apple Store eshte projekt i krijuar nga Adenis Shala per lenden Zhvillimi i Web.</p>


        </div>
        <div class="col l3 s12">
          <h5 class="white-text">Settings</h5>
          <ul>
            <li><a class="white-text" href="/">Home</a></li>
            <li><a class="white-text" href="/about">About Me</a></li>
            <li><a class="white-text" href="/premium">Premium Orders</a></li>
            <li><a class="white-text" href="/cart">Cart</a></li>
          </ul>
        </div>
        <div class="col l3 s12">
          <h5 class="white-text">Connect</h5>
          <ul>
            <li><a class="white-text">Facebook</a></li>
            <li><a class="white-text">Instagram</a></li>
            <li><a class="white-text">Twitter</a></li>
            <li><a class="white-text">LinkedIn</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="footer-copyright">
      <div class="container">
        Made by <a class="orange-text text-lighten-3" href="https://www.facebook.com/adonis.shala.9003">Adenis Shala</a>
      </div>
    </div>
  </footer>
</template>

<script>

  import axios from "axios"
  import swal from "sweetalert2"
  import store from "../../vuex/store"

  export default {
    name: "AppFooter",

    data() {
      return {
        page: 0,
      }
    },

    computed: {

      user: function () {
        return store.getters.getUser
      },

      login: function () {
        return store.getters.getLogin
      }
    },
  }
</script>