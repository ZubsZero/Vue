<template>
  <nav class="NavBar">
    <ul class="navbar-bg">
      <li><router-link to="/" class="link">Home</router-link></li>
      <li><router-link to="/" class-="link">Products</router-link></li>
      <li><router-link to="/contact" class="link">Contact</router-link></li>
    </ul>
  </nav>
</template>
<script>
export default {

}
</script>
<style scoped>
.NavBar {
    background-color: black;
    margin: 0;
    padding: 1px;
}
li {
    list-style-type: none;
    display: flex;
    flex-direction: row;
    margin: 5px;
    align-items: center;
    justify-content: center;
    padding: 20px;
}
.navbar-bg {
    display: flex;
    align-items:center;
    justify-content: center;
}

.link {
    text-decoration: none;
    color: white;
    font-weight: 700;
}

li:hover{
    background-color: white ;
    color: black;
}

.link:hover {
    color:black
}

</style>
