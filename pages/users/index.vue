<template>
  <div class="container mt-5">
    <b-input-group size="sm" class="mb-3" prepend="Type user id">
      <b-form-input v-model="id"></b-form-input>
      <b-input-group-append>
        <b-button size="sm" text="Button" variant="success" @click="loadUser">Go</b-button>
      </b-input-group-append>
    </b-input-group>
  </div>
</template>

<script>
export default {
  data() {
    return {
      id: ""
    };
  },
  methods: {
    loadUser() {
      this.$router.push(`/users/${this.id}`);
    }
  }
};
</script>

<style lang="scss">
</style>