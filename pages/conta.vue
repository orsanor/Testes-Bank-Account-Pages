<template>
  <v-app>
    <v-main>
      <div>
        <v-col>
          <v-row>
            <v-card class="d-flex card" elevation="0" height="100%" width="100%">
              <v-img
                class="ma-5 mt-2"
                max-height="9%"
                max-width="9%"
                src="https://blog.bancoafro.com.br/wp-content/themes/blogbancoafro/img/logo/logo.png"
              >
              </v-img>
              <v-action-button class="d-flex">
                <v-btn 
                class="rounded-xl ml-" 
                to="/index"
                >
                  Sair
                  <v-icon class="ml-1 rounded-xl botao"> mdi-close </v-icon>
                </v-btn>
              </v-action-button>
            </v-card>
          </v-row>
        </v-col>
        <v-col>
          <v-row class="d-flex justify-center">
             Seja Bem-vindo ao Banco Afro
          </v-row>
        </v-col>
        
      </div>
    </v-main>
  </v-app>
</template>
