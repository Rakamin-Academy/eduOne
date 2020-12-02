<template>
  <div id="app">
  <Jumbotron/>
  <Video/>
  <Features/>
  </div>
</template>

<script>
export default {
}
</script>

<style>
.container {
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.sansserif {
  font-family: sans-serif;
  font-size: 28px;
  font-weight: bold;
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
</style>
