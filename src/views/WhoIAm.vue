<template>
  <core-section id="who-i-am">
    <abstract-1 />

    <core-heading>Quienes Somos?.</core-heading>

    <v-col
      cols="12"
      md="7"
    >
      <v-row justify="space-between">
        <v-col
          cols="12"
          md="7"
        >
          <core-text class="mb-0">
            <p v-text="schema.basics.summary" />
          </core-text>
        </v-col>

        <v-col
          cols="12"
          md="4"
        >
          <v-row align="center">
            <v-col
              cols="6"
              class="text-uppercase primary--text font-weight-medium"
            >
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-col>

    <v-col
      class="hidden-sm-and-down text-right text-uppercase"
      cols="5"
    >

      <span
        class="primary--text font-weight-light"
      />

      <v-img
        :src="require('@/assets/john.png')"
        contain
        height="900"
        style="right: 0; position: absolute; top: 300px;"
      />
    </v-col>
  </core-section>
</template>

<script>
  // Utilities
  import {
    mapState,
  } from 'vuex'

  export default {
    name: 'WhoIAm',

    components: {
      Abstract1: () => import('@/components/Abstract1'),
    },

    computed: {
      ...mapState('app', ['schema']),
    },
  }
</script>

<style lang="sass">
  .v-expansion-panels > li
<template>
  <core-section id="who-i-am">
    <abstract-1 />

    <core-heading>Quienes Somos?.</core-heading>

    <v-col
      cols="12"
      md="7"
    >
      <v-row justify="space-between">
        <v-col
          cols="12"
          md="7"
        >
          <core-text class="mb-0">
            <p v-text="schema.basics.summary" />
          </core-text>
        </v-col>

        <v-col
          cols="12"
          md="4"
        >
          <v-row align="center">
            <v-col
              cols="6"
              class="text-uppercase primary--text font-weight-medium"
            >
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-col>

    <v-col
      class="hidden-sm-and-down text-right text-uppercase"
      cols="5"
    >

      <span
        class="primary--text font-weight-light"
      />

      <v-img
        :src="require('@/assets/john.png')"
        contain
        height="900"
        style="right: 0; position: absolute; top: 300px;"
      />
    </v-col>
  </core-section>
</template>

<script>
  // Utilities
  import {
    mapState,
  } from 'vuex'

  export default {
    name: 'WhoIAm',

    components: {
      Abstract1: () => import('@/components/Abstract1'),
    },

    computed: {
      ...mapState('app', ['schema']),
    },
  }
</script>

<style lang="sass">
  .v-expansion-panels > li
    border-top: 1px solid rgba(#fff, .12) !important
</style>
