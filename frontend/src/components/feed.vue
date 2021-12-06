<template>
  <div>
    <nav id="nav">
      <img src="../assets/logo.png" alt="logo" />
      <ul class="links">
        <li><router-link to="/feed">Accueil</router-link></li>
        <li><router-link to="/profile"> Profil</router-link></li>
        <li><a to="/login" v-on:click="Logout()"> Déconnexion</a></li>
      </ul>
    </nav>
    <h2>Fil d'actualité</h2>
    <!--)àn <p id= 'p1'></p>-->
    <div>
      <newMessage />
    </div>
    <div>
      <loadMessages />
    </div>
  </div>
</template>


<script>
import loadMessages from "./loadMessages";
import newMessage from "./newMessage";
//let date1 =  Date();
//document.getElementById('p1').innerHTML = 'Date du jour : ' + date1;

export default {
  name: "feed",
  components: {
    loadMessages,
    newMessage,
  },
  data() {
    return {
      token: "",
      allMessages: [],
    };
  },
  methods: {
    Logout() {
      localStorage.clear();
      this.$router.push("/");
    },
  },
};
</script>

<style scoped>
</style>