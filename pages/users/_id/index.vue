<template>
  <div class="container mt-5">
    <div>This is user's id {{$route.params.id}}</div>
    <hr />
  </div>
</template>

<script>
export default {
  validate({ params }) {
    // validate(context) {
    return /^\d+$/.test(params.id);
    // return /^\d+$/.test(context.params.id);
  }
};
</script>

<style lang="scss">
</style>