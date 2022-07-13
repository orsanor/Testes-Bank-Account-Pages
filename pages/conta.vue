<template>
  <v-app>
    <v-main class="page">
      <div>
        <v-card height="100px" width="auto%">
          <v-row>
            <v-col cols="6">
              <v-img
                class="ma-5 mt-2"
                max-height="auto"
                max-width="18%"
                src="https://blog.bancoafro.com.br/wp-content/themes/blogbancoafro/img/logo/logo.png"
              >
              </v-img>
            </v-col>
            <v-col cols="6" class="justify-center">
              <v-btn
                class="rounded-xl mt-6 float-right mr-3 pa-4"
                elavation="1"
                to="/"
              >
                Sair
              </v-btn>
            </v-col>
          </v-row>
        </v-card>

        <v-col cols="12">
          <v-row class="d-flex justify-center">
            <div>
              <v-card
                class="d-flex rounded-xl justify-center mt-16 card"
                elevation="3"
                height="350px"
                width="900px"
                outlined
              >
                <v-col cols="12">
                  <v-list-item-subtitle class="d-flex justify-center">
                    Bem-vindo(a)
                  </v-list-item-subtitle>
                  <v-list-item-title
                    class="d-flex justify-center font-weight-bold name"
                  >
                    Jonathan
                  </v-list-item-title>
                  <v-col cols="6">
                    <v-list-item-subtitle> Saldo </v-list-item-subtitle>
                    <v-list-item-title class="font-weight-bold display-1">
                      R$&nbsp;0,00
                    </v-list-item-title>
                    <v-col cols="12">
                      <v-btn
                        class="
                          d-flex
                          rounded-xl
                          mt-10
                          ml-4
                          justify-center
                          bottom
                        "
                        outlined
                        elevation="1"
                        height="110px"
                        width="350px"
                      >
                        <v-icon x-large color="#ffc107"> mdi-qrcode </v-icon>
                      </v-btn>
                    </v-col>
                  </v-col>
                </v-col>
              </v-card>
            </div>
          </v-row>
        </v-col>
      </div>
    </v-main>
  </v-app>
</template>

<style scoped>
.name {
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.page {
  background-color: #f2f2f2;
}
</style>


