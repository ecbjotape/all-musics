<template>
  <v-container class="fill-height">
    <v-responsive class="align-center text-center fill-height">
      <h1 style="margin-bottom: 5em">Connect yours accounts</h1>
      <v-row class="d-flex align-center justify-center">
        <v-col cols="auto">
          <v-btn
            @click="integration('youtube')"
            color="red"
            min-width="228"
            rel="noopener noreferrer"
            size="x-large"
            target="_blank"
          >
            <!-- TODO caso já tenha o código token do youtube, sinalzar com um check -->
            <!-- TODO verificar no vuex -->
            <v-icon icon="mdi-speedometer" size="large" start />
            Youtube
          </v-btn>
        </v-col>

        <v-col cols="auto">
          <v-btn
            @click="integration('spotify')"
            color="green"
            min-width="228"
            rel="noopener noreferrer"
            size="x-large"
            target="_blank"
            variant="flat"
          >
            <v-icon icon="mdi-speedometer" size="large" start />

            Spotify
          </v-btn>
        </v-col>
      </v-row>
    </v-responsive>
  </v-container>
</template>

<script lang="ts">
// import credentials from "../plugins/integrations";

export default {
  methods: {
    integration(type: string) {
      switch (type) {
        case "youtube":
          // TODO adicionar credenciais no env
          const clientId =
            "44183124635-qregh42r6jdeescjgc9q63fb31hki62a.apps.googleusercontent.com";
          const redirectUri = "http://localhost:3000/autorization";
          const scope = "https://www.googleapis.com/auth/youtube.readonly";

          const authorizationUrl = `https://accounts.google.com/o/oauth2/auth?client_id=${clientId}&redirect_uri=${redirectUri}&scope=${scope}&response_type=code`;

          // Redirecione o usuário para a URL de autorização
          window.location.href = authorizationUrl;
          break;

        case "spotify":
          alert("Integração com api do spotify pendente...");
        default:
          break;
      }
    },
  },
};
</script>
