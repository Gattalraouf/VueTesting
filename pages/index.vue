<template>
  <v-layout class=" justify-center align-center center">
    <v-card
      class="mx-auto my-12 d-flex pa-2 flex-wrap justify-center align-center"
      min-width="90%"
      outlined
    >
      <div id="avatar" class="text-center">
        <div>
          <div>
            <v-avatar size="150">
              <img src="https://cdn.vuetifyjs.com/images/john.jpg" alt="John" />
            </v-avatar>
          </div>
          <div>
            <v-btn class="ma-2" outlined rounded color="#FF2600">Modifier Profile</v-btn>
          </div>
        </div>
        <v-divider class="mx-4" id="divider" inset vertical></v-divider>
      </div>
      <div id="userInfo">
        <div class="userdata">
          <h1>Jhon Doe</h1>
          <div>
            <font-awesome-icon :icon="['fas', 'envelope']" />
            <p>contact@comapany.com</p>
          </div>
          <div>
            <font-awesome-icon :icon="['fas', 'phone-alt']" />
            <p>+001 2233 456</p>
          </div>
          <div>
            <font-awesome-icon :icon="['fas', 'map-marker-alt']" />
            <p>184 Main Rd E, St Albans VIC 3021, Australia</p>
          </div>
        </div>
      </div>
    </v-card>
  </v-layout>
</template>



<style scoped>
@import url("https://fonts.googleapis.com/css?family=Poppins&display=swap");
body {
  font-family: "Poppins", sans-serif !important;
}

.center {
  height: 100% !important;
}

#userInfo {
  width: 50%;
}
.userdata {
  margin: 15% 0% 15% 15%;
}

#avatar {
  margin: 5% 0%;
  font-size: 1rem;
  display: flex;
  align-items: center;
  flex-direction: row;
}
#avatar > div {
  margin: 0% 10% 0% 0%;
}

#userInfo > h1 {
  margin-bottom: 5%;
  font-size: 2rem;
  font-weight: bold;
  color: #f2f2f2;
}

#userInfo > div > div {
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-bottom: 1%;
  color: #7c7c7c;
  font-size: 0.66rem;
  font-weight: 200;
}

#userInfo > div > div > p {
  padding-left: 0.8rem;
  margin-bottom: 0%;
}

@media only screen and (max-width: 560px) {
  #divider {
    visibility: hidden;
  }
  #userInfo,
  .userdata {
    margin: 0%;
    width: 80%;
    text-align: center;
    align-items: center;
    justify-content: center;
    display: flex;
    flex-direction: column;
    margin-bottom: 5%;
  }
}
</style>
