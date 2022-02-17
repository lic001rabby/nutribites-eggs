<template>
  <div>
    <v-sheet id="hero">
      <v-container>
        <v-row>
          <v-col cols="12" md="8" lg="8" class="mt-8">
            <img
              width="70%"
              class="rounded-xl d-block mx-auto mb-8"
              src="~/static/eggs.avif"
              alt=""
            />
            <span
              class="text-h2 font-weight-black d-block mx-auto text-center accent--text"
              >Twin yolked eggs</span
            >
            <span
              class="text-h2 font-weight-black d-block mx-auto text-center accent--text"
              >Guranteed, Everytime</span
            >
          </v-col>
          <v-col cols="12" md="4" lg="4">
            <v-card flat rounded="xl">
              <v-card-text class="py-8">
                <span
                  class="text-h4 font-weight-black d-block mx-auto text-center accent--text mb-4"
                  >Box of 30 eggs, BDT450/= Only
                </span>
                <form name="Order" netlify data-netlify="true" data-netlify-honeypot="bot-field" method="POST">

                  <input type="hidden" name="form-name" value="Order" />

                <v-text-field
                  placeholder="Your full name"
                  label="Name"
                  outlined
                  rounded="xl"
                  name="Name"
                >
                </v-text-field>
                <v-text-field
                  label="Phone"
                  outlined
                  rounded="xl"
                  name="Phone"
                ></v-text-field>
                <v-text-field
                  name="Email"
                  type="email"
                  label="Email"
                  outlined
                  rounded="xl"
                ></v-text-field>

                <v-select
                  name="Frequency"
                  label="Send me eggs"
                  outlined
                  rounded="xl"
                  :items="['Weekly', 'Every 2 weeks', 'Monthly', 'Just one time']"
                >
                </v-select>
                <v-btn

                type="submit"
                  class="mx-auto d-block white--text"
                  color="accent"


                  href=""
                  large
                  rounded
                >
                  Send me eggs
                  <v-icon color="primary"
                    >mdi-egg</v-icon
                  ></v-btn
                >

                </form>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>
    <v-sheet color="accent" class="py-8">
      <v-container>
        <v-card color="transparent" flat>
          <v-card-text class="text-center"
            ><!-- <span class="text-h4 mt-6 pt-12 accent-text">Any queries</span> -->
            <span
              class="text-h3 font-weight-black d-block mx-auto mb-8 text-center primary--text"
              >Call Us Now!</span
            >
            <v-btn
              outlined
              x-large
              class="mx-auto rounded-xl"
              color="primary"
              href="tel:+8801708860395"
              >01708860395</v-btn
            >
          </v-card-text>
        </v-card>
      </v-container>
    </v-sheet>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>

<style scoped>
#hero {

  padding: 100px 0px;
  background-color: #f9f4d6;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
</style>
