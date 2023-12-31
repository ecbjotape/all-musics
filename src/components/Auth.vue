<template>
  <v-container class="fill-height">
    <v-responsive class="align-center text-center fill-height">
      <h1>AUTH</h1>
    </v-responsive>
  </v-container>
</template>

<script lang="ts">
//

export default {
  created() {
    // Captura o código de autorização da URL
    const authorizationCode = new URLSearchParams(window.location.search).get(
      "code"
    );
    // TODO persistir autenticação no vuex
    console.log(authorizationCode);
  },
};
</script>
