<template>
  <v-app id="inspire">
    <v-navigation-drawer
      color="green"
      dark
      absolute
      permanent
      right
      hide-overlay
      expand-on-hover
    >
      <v-list-item two-line class="px-2">
        <v-list-item-avatar>
          <img src="https://randomuser.me/api/portraits/women/81.jpg" />
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title>Jane Smith</v-list-item-title>
          <v-list-item-subtitle>Logged In</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-divider class="my-3"></v-divider>

      <v-list shaped nav dense>
        <v-list-item link to="/user/1">
          <v-list-item-icon>
            <v-icon>mdi-account</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>User 1</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link to="/user/2">
          <v-list-item-icon>
            <v-icon>mdi-home-city</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>User 2</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-main class="px-12 py-3" app>
      <v-container fluid>
        <router-view />
      </v-container>
    </v-main>
  </v-app>
</template>
