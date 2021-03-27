<template>
  <v-app-bar app color="#398860" flat>
    <v-container class="py-0 fill-height">
      <v-avatar class="mr-10" color="#398860" size="50">
        <img src="@/assets/images/easywon_logo_192x192.png" alt="logo" />
      </v-avatar>

      <v-btn v-for="link in links" :key="link.title" :to="link.to" text dark>
        {{ link.title }}
      </v-btn>

      <v-spacer></v-spacer>

      <v-responsive max-width="260">
        <v-text-field background-color="#ffffff" color="#398860" dense flat hide-details rounded solo label="Search"></v-text-field>
      </v-responsive>
    </v-container>
  </v-app-bar>
</template>

<script>
export default {
  name: "AppBar",
  component: {},
  data() {
    return {
      links: [
        { title: "Dashboard", to: "/" },
        { title: "Study", to: "/study" },
        { title: "Profile", to: "/profile" },
        { title: "Updates", to: "/updates" },
      ],
    };
  },
};
</script>
