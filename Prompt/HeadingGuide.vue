<template>

  <text class="title-text">
    {{headingText}}
  </text>

</template>

<script>

export default {
  props: ['headingText']
}

</script>

<style>

.title-text {
  color:white;
  font-size: 25px;
  font-weight: 600;
}

</style>
