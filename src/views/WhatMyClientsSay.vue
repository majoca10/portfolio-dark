<template>
  <core-section id="what-my-clients-say">
    <core-heading>Formas de Pago.</core-heading>
    <v-row>
      <div class="pt-3 font-italic">
        <template>
          <v-data-table
            :headers="headers"
            :items="desserts"
            item-key="name"
            sort-by="name"
            group-by="category"
            class="elevation-1"
            show-group-by
          ></v-data-table>
        </template>
      </div>
    </v-row>
  </core-section>
</template>
<script>
  export default {
    name: 'WhatMyClientsSay',
    components: {
    },
    data: () => ({

          quote: 'Aliquam sit amet eros id lorem posuere lobortis ut id enim. Proin ullamcorper fringilla risus et lacinia.Aliquam eget lacus a libero.',
          name: 'J. Williams',
          company: 'Motion',

          headers: [
          {
            text: 'Dessert (100g serving)',
            align: 'start',
            value: 'name',
            groupable: false,
          },
          { text: 'Category', value: 'category', align: 'right' },
          { text: 'Dairy', value: 'dairy', align: 'right' },
        ],
        desserts: [
          {
            name: 'Frozen Yogurt',
            category: 'Ice cream',
            dairy: 'Yes',
          },
          {
            name: 'Ice cream sandwich',
            category: 'Ice cream',
            dairy: 'Yes',
          },
          {
            name: 'Eclair',
            category: 'Cookie',
            dairy: 'Yes',
          },
          {
            name: 'Cupcake',
            category: 'Pastry',
            dairy: 'Yes',
          },
          {
            name: 'Gingerbread',
            category: 'Cookie',
            dairy: 'No',
          },
          {
            name: 'Jelly bean',
            category: 'Candy',
            dairy: 'No',
          },
          {
            name: 'Lollipop',
            category: 'Candy',
            dairy: 'No',
          },
          {
            name: 'Honeycomb',
            category: 'Toffee',
            dairy: 'No',
          },
          {
            name: 'Donut',
            category: 'Pastry',
            dairy: 'Yes',
          },
          {
            name: 'KitKat',
            category: 'Candy',
            dairy: 'Yes',
          },
        ],
      
    }),
  }
</script>
