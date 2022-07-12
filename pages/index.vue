<template>
  <v-container>
    <v-row>
      <v-spacer></v-spacer>
      <v-col cols="8">
        <!--Formulario-->
        <v-card height="550" rounded="false">
          <v-card-text>
            <v-form v-model="valid">
              <v-row>
                <v-spacer></v-spacer>
                <v-col cols="8" class="logo">
                  <v-img
                    height="100%"
                    width="50%"
                    src="https://blog.bancoafro.com.br/wp-content/themes/blogbancoafro/img/logo/logo.png"
                  >
                  </v-img>
                </v-col>
                <v-spacer></v-spacer>
              </v-row>

              <!--textfields-->
              <v-row>
                <v-col cols="12" md="4">
                  <v-text-field
                    outlined
                    v-model="nome"
                    :rules="nomeRules"
                    placeholder="Nome"
                    filled
                    required
                  ></v-text-field>
                </v-col>

                <v-col cols="12" md="4">
                  <v-text-field
                    outlined
                    v-model="sobrenome"
                    :rules="sobrenomeRules"
                    placeholder="Sobrenome"
                    filled
                    required
                  ></v-text-field>
                </v-col>

                <v-col cols="12" md="4">
                  <v-text-field
                    outlined
                    v-model="email"
                    :rules="emailRules"
                    placeholder="E-mail"
                    filled
                    required
                  ></v-text-field>
                </v-col>
              </v-row>
            </v-form>
          </v-card-text>
        </v-card>
      </v-col>
      <v-spacer></v-spacer>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    valid: false,
    nomeRules: [(v) => !!v || "Por favor colocar o Nome"],
    nome: "",
    sobrenome: "",
    sobrenomeRules: [(v) => !!v || "Por favor colocar o Sobrenome"],
    email: "",
    emailRules: [(v) => !!v || "Por favor colocar um E-mail valido"],
  }),
};
</script>

<style scoped>
.logo {
  padding-left: 22%;
}
</style>