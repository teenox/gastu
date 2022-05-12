<template>
  <div>
    <div class="mini-spacer">
      <v-container>
        <!-- -----------------------------------------------
            Start Contact Form
        ----------------------------------------------- -->
        <v-row justify="center">
          <v-col cols="12" sm="10" md="12" lg="12">
            <div class="scan-body">
              <h4 class="font-weight-medium contact-title mt-0">
                Do the house search for free advice
              </h4>
              <form>
                <v-row class="mt-15">
                  <v-col cols="12" class="py-0">
                    <v-text-field
                      name="address"
                      outlined
                      label="Address"
                    ></v-text-field>
                  </v-col>
                  <v-col cols="12" md="6" class="py-0">
                    <v-text-field
                      label="Name"
                      outlined
                      v-model="name"
                      placeholder="Name"
                    ></v-text-field>
                  </v-col>
                  <v-col cols="12" md="6" class="py-0">
                    <v-text-field
                      label="Email"
                      outlined
                      type="email"
                      v-model="email"
                      placeholder="Email"
                    ></v-text-field>
                  </v-col>
                </v-row>
                <v-btn
                  nuxt
                  to="/"
                  class="btn-custom-md btn-danger-gradient mt-12"
                  outlined
                  color="white"
                  elevation="0"
                >
                  Start the search
                </v-btn>
              </form>
            </div>
          </v-col>
        </v-row>
        <!-- -----------------------------------------------
            End Contact Form
        ----------------------------------------------- -->
      </v-container>
    </div>
  </div>
</template>
<script>
export default {
  name: "Search",
  data() {
    return {
      name: "",
      email: "",
    };
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
.scan-body {
  background-color: #fff;
  padding: 30px;
  border-radius: 16px;
  box-shadow: 0 2px 20px 0 rgb(0 0 0 / 15%);
  margin-top: 239px;
  position: absolute;
}
</style>