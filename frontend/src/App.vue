<template>
  <div>
    <router-view />
    <footer>
      <p>Copyright © 2021 Tous droits réservés | un étudiant d'Openclasrooms</p>
    </footer>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: black;
  background-color: #f1f1f1	;
  background-image: url("assets/backmess.jpg");

}

#nav {
  background-image: url("assets/head.jpg");
  background-size: cover;
  width: 100%;
  height: 100px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  color: white;
  border-bottom: 6px solid #d44c5c;
  font-size: 1.25em;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}
#nav a{
  text-decoration: none;
  color: white;
  margin: auto;
}
#nav img {
  width: 22%;
  margin: auto;
}
  p {
    color: rgb(189, 89, 89);
  }
  .links {
    display: flex;
    flex-wrap: wrap;
    // justify-content: space-between;
    list-style: none;
    // width: 30%;
  }
  li {
    margin-right: 20px;
  }
  a {
    font-weight: bold;
    color: white;
    text-decoration: none;

    &.router-link-exact-active {
      color: #c46e78;
    }
  }
  a:hover {
    border-bottom: 2px solid white;
  
  }
footer {
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #192a48;
  background-image: url("assets/head.jpg");
  border-top: 6px solid #d44c5c;
  color: white;
  height: 60px;
  padding: 20px;
  margin-top: 50px;
}

@media screen and (max-width: 768px) {
  #nav img {
    width: 35%;
  }
}
@media screen and (max-width: 450px) {
  #nav img {
    width: 50%;
  }
}
</style>
