<template>
<div v-bind:class="[{ leftClass: direction === 'left', rightClass: direction === 'right' }, 'directionClass']"></div>
</template>

<script>

export default {
  name: 'ArrowButton',
  props: {
    direction: String
  }
};

</script>

<style>
.directionClass {
  width: 0;
  height: 0;
  border-style: solid;
  margin: 15px;
}
.rightClass{
  border-width: 15px 0 15px 31px;
  border-color: transparent transparent transparent #c6d18f;
}
.leftClass{
  border-width: 15px 31px 15px 0;
  border-color: transparent #c6d18f transparent transparent;
}
</style>
  