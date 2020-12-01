<template>
    <div class="Login" style="display:flex">
        <form class="signin" style="padding:10% 2% 10% 2%">
            <h3 class="text-center">Sign In</h3>
            <div class="form-group">
                <input type="email" placeholder="Email" class="form-control form-control-lg" />
            </div>
            <div class="form-group">
                <input type="password" placeholder="Password" class="form-control form-control-lg" />
            </div>
            <p class="forgot-password text-center mt-2 mb-4">Forgot password? <a href="#">Click here</a></p>
            <nuxt-link to="/"><button type="submit" class="btn btn-dark btn-lg btn-block">Sign In</button></nuxt-link>
        </form>
        <form class="signUp" style="padding:10% 2% 10% 2%">
            <h3 class="text-center">Here is EduOne</h3>
            <p>Lorem ipsum dolor sit amet consectetur.</p>
            <p>Lorem ipsum dolor sit amet consectetur.</p>
            <nuxt-link to="/"><button type="submit" style="background-color:white; color:black;" class="btn btn-dark btn-lg btn-block">Sign up</button></nuxt-link>
        </form>
    </div>
</template>

<script>
    export default {
        data() {
            return {}
        }
    }
</script>

<style>

body{
  background: #ffffff!important;
  min-height: 100vh;
  display: flex;
  font-weight: 400;
}

.Login {
  width: 100%;
  height: 100%;
  margin: auto;
  box-shadow: 0px 14px 80px rgba(34, 35, 58, 0.2);
  padding: 40px 55px 45px 55px;
  border-radius: 15px;
  margin: 50%;
}
.signUp{
  background-color: #213E3B;
  color: #ffffff;
}
.signin{
  border: 1px solid;
  padding: 10px;
  box-shadow: 5px 10px 18px #888888;
  }

</style>