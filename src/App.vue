<template>
<main>
  <nav>
    <ul>
      <li>Marché</li>
      <li>Panier</li>
      <li>S'abonner</li>
    </ul>
  </nav>
  <div class="container">
    <div class="top">
      <div class="name">
        <h1>Maket Place</h1>
        <p>Buy somethings</p>
      </div>
      <a href="./components/panier.vue"><i class="fas fa-shopping-basket"></i></a>
    </div>
    <div class="down">
      <div class="contents">
        <img src="./assets/pate.png" alt="Pate">
        <div class="price_button">
          <p>Pâtes</p>
          <p>2 balles</p>
          <button id="add"><i class="fas fa-plus"></i></button>
        </div>
      </div>
      <div class="contents">
        <img src="./assets/concombre.png" alt="Concombre">
        <div class="price_button">
          <p>Concombre</p>
          <p>2 balles</p>
          <button id="add"><i class="fas fa-plus"></i></button>
        </div>
      </div>
      <div class="contents">
        <img src="./assets/tomate.png" alt="Tomate">
        <div class="price_button">
          <p>Tomate</p>
          <p>2 balles</p>
          <button id="add"><i class="fas fa-plus"></i></button>
        </div>
      </div>
      <div class="contents">
        <img src="./assets/salade.png" alt="Salade">
        <div class="price_button">
          <p>Salade</p>
          <p>2 balles</p>
          <button id="add"><i class="fas fa-plus"></i></button>
        </div>
      </div>
      <div class="contents">
        <img src="./assets/poulet.png" alt="Poulet">
        <div class="price_button">
          <p>Poulet</p>
          <p>2 balles</p>
          <button id="add"><i class="fas fa-plus"></i></button>
        </div>
      </div>
      <div class="contents">
        <img src="./assets/oigon.png" alt="Oigon">
        <div class="price_button">
          <p>Oigons</p>
          <p>2 balles</p>
          <button id="add"><i class="fas fa-plus"></i></button>
        </div>
      </div>
      <div class="contents">
        <img src="./assets/patate.png" alt="Patate">
        <div class="price_button">
          <p>Patate</p>
          <p>2 balles</p>
          <button id="add"><i class="fas fa-plus"></i></button>
        </div>
      </div>
      <div class="contents">
        <img src="./assets/patate_douce.png" alt="Patate douce">
        <div class="price_button">
          <p>Patate douce</p>
          <p>2 balles</p>
          <button id="add"><i class="fas fa-plus"></i></button>
        </div>
      </div>
      <div class="contents">
        <img src="./assets/brocoli.png" alt="Brocoli">
        <div class="price_button">
          <p>Brocoli</p>
          <p>2 balles</p>
          <button id="add"><i class="fas fa-plus"></i></button>
        </div>
      </div>

    </div>
  </div>
</main>
</template>

<script>
// import panier from './components/panier.vue';

export default {
  name: 'App',
  components: {
    // panier,
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  list-style: none;
  text-decoration: none;
}

main {
  height: 100vh;
  display: flex;
  background: linear-gradient(to top right, #5DE7B0, white);
}

nav {
  width: 10%;
  display: flex;
  flex-direction: column;
  align-items: center;
  background: linear-gradient(#5DCFE7, white);
}

.container {
  width: 90%;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px 0;
}

/* TOP */
.top {
  width: 80%;
  height: 15vh;
  display: flex;
  justify-content: space-around;
  align-items: center;
  border-radius: 15px;
  background: linear-gradient(
 rgba(0, 0, 0, 0.45), 
 rgba(0, 0, 0, 0.45)
 ),url(./assets/supermarchet.jpg);
 background-size:cover;
 color: white;
 padding: 0 25px;
}

.top i {
  font-size: 25px;
  color: white;
}

.name {
  width: 20vw;
  text-align: center;
}

/* DOWN */
.down {
  width: 90%;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  border-radius: 15px;
  background-color: white;
  margin-top: 15px;
}

.contents {
  width: 20vw;
  height: 20vh;
  display: flex;
  justify-content: space-around;
  border: 1px solid black;
  border-radius: 5px;
  box-shadow: 5px 5px 10px gainsboro;
  margin: 20px;
}

img {
  width: 10vw;
}

.price_button {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
}

button {
  width: 2vw;
  height: 4vh;
}

#add:hover {
  color: green;
  cursor: pointer;
}

button i {
  font-size: 18px;
}
</style>