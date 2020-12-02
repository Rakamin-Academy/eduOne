<template>
    <div style="margin:3%" >
  <b-row>
    <b-col cols="6" >
        <b-row>
        <b-row>
            <b-col cols="4" ><img src="~/assets/eduone-logo.jpeg" style="width:100%;height:100%;" /></b-col>
            <b-col  cols="8">
                <p style="text-align:left; font-size:36px">eduOne</p>
                <p style="text-align:left; font-size:20px">Your Elearning Answer</p>
            </b-col>
        </b-row>
        <b-col cols="12" ><p style="text-align:center; font-size:20px">Follow us On</p>
        <div>
    <font-awesome-icon style="font-size:400%;margin:5%" :icon="['fab', 'twitter']"/>
    <font-awesome-icon style="font-size:400%;margin:5%" :icon="['fab', 'instagram']"/>
    <font-awesome-icon style="font-size:400%;margin:5%" :icon="['fab', 'facebook']"/>
    <font-awesome-icon style="font-size:400%;margin:5%" :icon="['fab', 'youtube']"/>
  </div>
        </b-col>
    </b-row>
  </b-col >
    <b-col cols="6" >
        <p style="text-align:left;font-size:36px">Contact Us</p>
        <div>
        <div class="col-md-12">
         <input type="text" placeholder="Your Name" class="form-control">
        </div> 
        <div class="col-md-12">
         <input type="text" placeholder="Email" class="form-control">
        </div> 
        <div class="col-md-12">
          <textarea placeholder="Message" rows="4" class="form-control">
          </textarea>
        </div> 
        <div class="col-md-8">
          <b-button type="submit" value="Send" variant="info" class="form-control text-uppercase">Send</b-button>
        </div>
      </div>
    </b-col>
  </b-row>
</div>
</template>

<script>
export default {
    name: 'Footer',
}
</script>

<style>
</style>