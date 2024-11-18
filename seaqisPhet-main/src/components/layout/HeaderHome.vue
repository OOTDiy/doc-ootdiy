<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
 <header>
    <img alt="SEAQIS Logo" class="logo" src="@/assets/logo.svg" />

    
      

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/simulation">Simulation</RouterLink>
        <RouterLink to="/teaching">Teaching</RouterLink>
        <RouterLink to="/research">Research</RouterLink>
      </nav>
      <input
			
			id="search-input"
			type="text"
			name=""
			placeholder="Search..."
		/>
    
  </header>

</template>

<style scoped>
header {
  position: sticky; 
  top: 0; 
  width: 100%; 
  height: 20px;
  background-color: #ffffff31; 
  color: white; 
  text-align: center; 
  padding: 1rem; 
  z-index: 1000;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
  text-align: center;
  margin-top: 2rem;
  top : 0;
 
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 555px) {
  header {
    display: flex;
    place-items: center;
    /* padding-right: calc(var(--section-gap) / 2); */
    z-index: 1000;
  }

  .logo {
    margin: 0 2rem 0 0;
    text-align: center;
    margin-top: 1rem;
    width: 125px;
    height: 125px; 
  /* kash */
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
@media (max-width: 555px) {
  header {
  position: sticky; 
  top: 0; 
  width: 100%; 
  height: 5px;
  background-color: #ffffff; 
  color: white; 
  text-align: center; 
  padding: 1rem; 
  z-index: 1000;
}
.logo {
 
 
  width: 100px;
  height: 100px;
}
.nav{
  display: none;
}

}
</style>