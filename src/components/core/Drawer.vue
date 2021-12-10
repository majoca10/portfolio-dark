<template>
  <v-navigation-drawer
    v-if="$vuetify.breakpoint.mdAndUp"
    app
    class="text-center"
    color="#181818"
    permanent
  >
    <v-row
      align="center"
      class="flex-column fill-height py-5 mx-0"
      justify="center"
    >
    <div style="height: 300px; width: -webkit-fill-available;">
    <v-img
      :src="require('@/assets/logo2.png')"
    ></v-img>
    </div>
      <div
        v-for="(item, i) in items"
        :key="i"
      >
        <v-btn
          class="text-capitalize subheading font-weight-light mb-3"
          text
          @click="$vuetify.goTo(item.to)"
        >
          <span v-text="item.text" />
        </v-btn>
      </div>
      <div class="mt-auto">
        <social-contacts />
      </div>
    </v-row>
  </v-navigation-drawer>
</template>

<script>
  // Utilities
  import {
    mapState,
  } from 'vuex'

  export default {
    name: 'Drawer',

    components: {
      SocialContacts: () => import('@/components/SocialContacts'),
    },

    data: vm => ({
      items: [
        {
          text: 'Quienes Somos?',
          to: '#who-i-am',
        },
        {
          text: 'Como nos ayudas?',
    <template>
  <v-navigation-drawer
    v-if="$vuetify.breakpoint.mdAndUp"
    app
    class="text-center"
    color="#181818"
    permanent
  >
    <v-row
      align="center"
      class="flex-column fill-height py-5 mx-0"
      justify="center"
    >
    <div style="height: 300px; width: -webkit-fill-available;">
    <v-img
      :src="require('@/assets/logo2.png')"
    ></v-img>
    </div>
      <div
        v-for="(item, i) in items"
        :key="i"
      >
        <v-btn
          class="text-capitalize subheading font-weight-light mb-3"
          text
          @click="$vuetify.goTo(item.to)"
        >
          <span v-text="item.text" />
        </v-btn>
      </div>
      <div class="mt-auto">
        <social-contacts />
      </div>
    </v-row>
  </v-navigation-drawer>
</template>

<script>
  // Utilities
  import {
    mapState,
  } from 'vuex'

  export default {
    name: 'Drawer',

    components: {
      SocialContacts: () => import('@/components/SocialContacts'),
    },

    data: vm => ({
      items: [
        {
          text: 'Quienes Somos?',
          to: '#who-i-am',
        },
        {
          text: 'Como nos ayudas?',
          to: '#what-i-can-do-for-you',
        },
        {
          text: 'Recompensa',
          to: '#where-ive-been',
        },
        {
          text: 'Donaciones',
          to: '#what-my-clients-say',
        },
        {
          text: 'Contact',
          to: '#lets-talk',
        },
      ],
    }),

    computed: {
      ...mapState('app', ['initials', 'schema']),
    },
  }
</script>
