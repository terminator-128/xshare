<template>
  <v-app>
    <!-- Navigation on the top of the Page -->
    <Navbar />

    <!-- Main content -->
    <v-main>
      <v-container fluid>
        <!-- <router-view ></router-view> -->
        <ScholarProfile />
      </v-container>
    </v-main>

    <!-- Footer -->
    <Footer />
  </v-app>
</template>

<script>
import Navbar from './components/NavBar';
import Footer from './components/Footer';
import ScholarProfile from './views/ScholarProfile';

export default {
  name: 'App',

  components: {
    Navbar,
    Footer,
    ScholarProfile,
  },

  data: () => ({
    //
  }),
};
</script>
