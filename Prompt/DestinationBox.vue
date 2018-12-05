<template>

  <text-input
    v-model="text"
    :placeholder="placeholderText"
    class="destination-box"
  />

</template>

<script>

export default {

  props: ['placeholderText'],
  
  data: function() {
    return {
      text:null
    }
  }

}

</script>

<style>
.destination-box{
  margin-top:10px;
  padding:15px;

  font-size:17px;
  height: 50px;
  background-color:rgba(255, 255, 255, 0.2);
}
</style>
