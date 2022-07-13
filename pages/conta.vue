<template>
  <v-app>
    <v-main>
      <div>
        <v-row>
          <v-col cols="6">
            <v-img
              class="ma-5 mt-2"
              max-height="100%"
              max-width="22%"
              src="https://blog.bancoafro.com.br/wp-content/themes/blogbancoafro/img/logo/logo.png"
            >
            </v-img>
          </v-col>
          <v-col cols="6" class="justify-center">
            <v-btn class="rounded-xl mt-10 float-right mr-2" to="/">
              Sair
              <v-icon class="ml-1 rounded-xl"> mdi-close </v-icon>
            </v-btn>
          </v-col>
        </v-row>

        <v-col>
          <v-row class="d-flex justify-center">
            <div class="h5 font-weight-bold gray--text"
            >
            Seja Bem-vindo ao Banco Afro
            </div>
          </v-row>
        </v-col>
      </div>
    </v-main>
  </v-app>
</template>

<style scoped>
</style>
