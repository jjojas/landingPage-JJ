<template>
<div class="content">
  <div class="title_container">
        <button @click="lightMode()"><i class="fi fi-br-bulb"></i></button>
        <h1>Justin Dermawan Ikhsan</h1>
  </div>
  <div class="main-cont">
   <div id="nav">
      <router-link to="/">About</router-link>
      <router-link to="/skills">Skills</router-link>
      <router-link to="/portfolio">Portfolio</router-link>
      <router-link to="/thoughts">Thoughts</router-link>
    </div>
    <router-view/>
  </div>
</div>  
</template>

<script>

export default ({
  setup() {
    
  },
  methods: {
    lightMode(){
      var element = document.body;
      element.classList.toggle("dark-mode");
  }
}
})
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700;800;900&display=swap');
@import url('https://cdn-uicons.flaticon.com/uicons-bold-rounded/css/uicons-bold-rounded.css');

body{
  background: #2f2f2f;
  color: #fcfcfc;
}
#app {
  font-family: Montserrat, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: inherit;
  background: inherit;
  padding: 2em 4em;
}

.dark-mode{
  color: #2f2f2f;
  background: #fcfcfc;
}

.main-cont{
  padding: 30px;
  display: flex;
  flex-direction: row;
  align-items: flex-start;
}

#nav {
  padding: 2em;
  width: 10%;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
}

router-view{
  display: flex;
}

.title_container{
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: flex-start;
}

.title_container button i{
  font-size:24px;
}

.title_container h1 {
    font-size: 24px;
    font-weight: 600;
    letter-spacing: 0em;
    transition: 0.3s;
}

.title_container h1:hover {
    letter-spacing: 0.2em;
}

.title_container button{
    background:none;
    border-style: none;
    color: inherit;
}

.title_container button i{
    color: inherit;
}

#nav a {
  font-weight: 600;
  text-decoration: none;
  color: inherit;
  padding: 1em 0em;
}

#nav a.router-link-exact-active {
  font-weight: 800;
}

h1 {
  font-size: 36px;
  font-weight: bold;
  margin-bottom: 1em;
}

p {
  font-size: 24px;
  font-weight: 400;
}


@media only screen and (max-width: 768px) {

  
.title_container button i{
  font-size:14px;
}

.title_container h1 {
    font-size: 14px;
}

  .title_container{
    font-size: 24px;
  }
  
  #app{
    padding: 1em 0em;
  }

  .main-cont{
    padding: 1em;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }

  #nav {
    padding: 0em;
    display: flex;
    flex-direction: row;
    align-items: center;
}

#nav a {
  font-weight: 600;
  text-decoration: none;
  color: inherit;
  padding: 0em .25em;
  }
  
  h1 {
    font-size: 24px;
    font-weight: bold;
    margin-bottom: 1em;
  }

  h2 {
    font-size: 20px;
    font-weight: bold;
  }

  p {
    font-size: 18px;
    font-weight: 400;
  }

}
</style>
