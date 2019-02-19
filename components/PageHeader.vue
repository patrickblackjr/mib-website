<template>
  <div id="pageHeader">
    <b-row class="mt-5 mb-3">
      <b-col>
        <h2 class="text-center">{{ title }}</h2>
        <hr/>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  props: [
    'title'
  ]
}
</script>

<style lang="scss">
$purple: #8e44ad;
$primary: $purple;

hr {
  width: 30%;
  background-color: $primary;
  margin-top: 3em;
}
</style>