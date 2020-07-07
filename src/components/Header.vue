<template>
  <div class="header">
    <img src="assets/logo_bila.png" alt="Logo">
    <div class="site_description">Docházkový systém</div>
  </div>
</template>

<script>

export default {
  name: 'Header'

};

</script>

<style>
.header{
  display: flex;
  justify-content: space-around;
  color: #c6d18f;
  padding: 16px;
}
img{
  width: 40%;
  height: auto;
}
.site_description{
  align-self: flex-end;
  font-weight: bold;
  text-transform: uppercase;
  font-size: 14px;

}
</style>
