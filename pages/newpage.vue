<template>
  <v-app>
    <v-main class="d-flex align-center">
      <v-container class="d-flex justify-center">
        <div>
          <v-card class="d-flex justify-center rounded-xl" height="auto" width="500px">
            <v-col>
              <v-row class="d-flex justify-center">
                <v-img
                  class="ma-5"
                  max-height="20%"
                  max-width="20%"
                  src
                >
                </v-img>
              </v-row>
              <v-row>
                <v-text-field 
                  class="ml-15 mr-15 " 
                  outlined
                  label="Login"
                > 
                </v-text-field>
              </v-row>
              <v-row>
                <v-text-field 
                  class="ml-15 mr-15 mb-3" 
                  outlined
                  label="Senha"
                > 
                </v-text-field>
              </v-row>
              <v-action-button class="d-flex justify-center">
                <v-btn
                
              
                >
                    entrar
                    <v-icon
                      class="ml-2 amber accent-3 rounded-xl"
                    >
                      
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

