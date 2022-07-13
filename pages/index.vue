<template>
  <v-app>
    <v-main class="d-flex align-center">
      <v-container class="d-flex justify-center">
        <div class="d-flex justify-center">
          <v-card
            class="d-flex justify-center rounded-xl cartao"
            elevation="3"
            height="auto"
            width="82%"
          >
            <v-col>
              <v-row class="d-flex justify-center">
                <v-img
                  class="ma-5 mt-2"
                  max-height="20%"
                  max-width="20%"
                  src="https://usefintech.com/wp-content/uploads/2020/09/sample-logo-600x600.png"
                >
                </v-img>
              </v-row>
              <v-row>
                <v-text-field class="ml-15 mr-15 login" outlined label="Login">
                </v-text-field>
              </v-row>
              <v-row>
                <v-text-field
                  class="ml-15 mr-15 mb-3 senha"
                  outlined
                  label="Senha"
                >
                </v-text-field>
              </v-row>
              <v-action-button class="d-flex justify-center">
                <v-btn
                  class="rounded-xl"
                  :loading="loading"
                  :disabled="loading"
                  @click="login()"
                  
                >
                  Entrar
                  <v-icon class="ml-2 rounded-xl botao">
                    mdi-arrow-right-bold
                  </v-icon>
                </v-btn>
              </v-action-button>
            </v-col>
          </v-card>
        </div>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      loader: null,
      loading: false,
    };
  },
  methods: {
    async login() {
      this.loader = "loading";
      this.$router.push('/conta');
    },
  },
  watch: {
    loader() {
      const l = this.loader;
      this[l] = !this[l];

      setTimeout(() => (this[l] = false), 2000);

      this.loader = null;
    },
  },
};
</script>

<style scoped>
.senha {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
}
.login {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
}

.botao {
  background-color: #ffc107;
}
</style>