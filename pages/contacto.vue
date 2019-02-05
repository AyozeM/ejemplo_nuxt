<template>
  <b-container>
    <b-form>
      <b-form-group label="Datos personales">
        <b-form-input
          v-model="data.email"
          type="email"
          required
          placeholder="Ejemplo: suso@mail.com"
          label="Email"
        />
      </b-form-group>
    </b-form>
  </b-container>
</template>

<script>
export default {
  data() {
    return {
      data: {
        email: null
      }
    }
  }
}
</script>

<style>
</style>
