<template>
  <div>
    <header>
       <img id="eduone-logo" src="~/assets/eduone-logo.jpeg" />
      <nuxt-link id="nav" to=/home>Home</nuxt-link>
      <nuxt-link id="nav" to=/forum>Forum</nuxt-link>
      <nuxt-link id="nav" to=/banksoal>BANK Soal</nuxt-link>
      <nuxt-link id="nav" to=/videos>Videos</nuxt-link>
      <nuxt-link id="nav" to=/tutorprofile>Tutor Profile</nuxt-link>
      <Button />
    </header>
    <Nuxt />

    <footer>

    </footer>
  </div>
</template>

<script>
export default {
}
</script>

<style>
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

header{
  padding-top: 35px;
  display: flex;
  justify-content: center;
  align-items: center;
}

header, #nav , #navBtn{
  margin: 0 20px;
}

header #nav{
  color: black;
  font-weight: 500;
  text-decoration: none;
}

header #nav:hover{
  color: #41AEA9;
  text-decoration: none;
}

#eduone-logo{
  width: 100px;
  height: 100px;
  box-shadow: -3px 5px 4px rgba(0, 0, 0, 0.25);
  margin-right: 100px;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
