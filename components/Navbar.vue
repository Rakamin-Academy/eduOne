<template>
  <div>
    <header>
      <img id="eduone-logo" src="~/assets/eduone-logo.jpeg" />
      <nuxt-link id="nav" to="/Home">Home</nuxt-link>
      <nuxt-link id="nav" to=/forum>Forum</nuxt-link>
      <nuxt-link id="nav" to=/banksoal>BANK Soal</nuxt-link>
      <nuxt-link id="nav" to=/videos>Videos</nuxt-link>
      <nuxt-link id="nav" to=/tutorprofile>Tutor Profile</nuxt-link>
      <button class="button--green">Sign In</button>
    </header>
  </div>
</template>

<script>
export default {

}
</script>

<style>
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

.button--green {
  display: inline-block;
  border-radius: 4px;
  color: #fff;
  background-color: #41AEA9;
  text-decoration: none;
  width: 180px;
  height: 50px;
  border: 0;
  margin-left: 100px;
}

.button--green:hover {
  background: white;
  border: 1px solid #41AEA9;
  color: #41AEA9;
}
</style>
