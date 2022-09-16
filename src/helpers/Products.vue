<script setup>
import image01 from '../assets/images/image01.png'
import image02 from '../assets/images/image02.png'
import image03 from '../assets/images/image03.png'
import image04 from '../assets/images/image04.png'
import image05 from '../assets/images/image05.png'
import image06 from '../assets/images/image06.png'
import image07 from '../assets/images/image07.png'
import image08 from '../assets/images/image08.png'
import image09 from '../assets/images/image09.png'

const products = [
  { id: 1, image: image01, description: 'Lorem ipsum dolor sit', value: 50 },
  { id: 2, image: image02, description: 'Lorem ipsum dolor sit', value: 50 },
  { id: 3, image: image03, description: 'Lorem ipsum dolor sit', value: 50 },
  { id: 4, image: image04, description: 'Lorem ipsum dolor sit', value: 50 },
  { id: 5, image: image05, description: 'Lorem ipsum dolor sit', value: 50 },
  { id: 6, image: image06, description: 'Lorem ipsum dolor sit', value: 50 },
  { id: 7, image: image07, description: 'Lorem ipsum dolor sit', value: 50 },
  { id: 8, image: image08, description: 'Lorem ipsum dolor sit', value: 50 },
  { id: 9, image: image09, description: 'Lorem ipsum dolor sit', value: 50 }
]
</script>

<template>
  <ul>
    <li v-for="product in products" :key="product.id">
      <img :src="product.image" alt="product_image">
      <h3>{{ product.description }}</h3>
      <p>R$ <span>{{ product.value }},00</span></p>
    </li>
  </ul>
</template>