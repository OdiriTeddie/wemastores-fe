<template>
  <section class="container">
    <h2>Popular Categories</h2>
    <div class="flex justify-between">
      <div v-for="category in categoriesData" v-bind:key="category.id">
        <div class="popular-category-img">IMG</div>
        <div>
          <h4>{{ category.name }}</h4>
          <span>{{ category.product_count }} products</span>
        </div>
      </div>
    </div>
  </section>
</template>
<script lang="ts" setup>
import axios from 'axios'
import { onMounted, ref } from 'vue'

interface Category {
  id: number
  name: string
  slug: string
  product_count: number
}

const categoriesData = ref<Category[]>([])

const fetchCategories = async () => {
  try {
    const response = await axios.get('http://wemastores.test/api/categories')
    categoriesData.value = response.data.data
  } catch (error) {
    console.error(error)
  }
}

// watch(
//   () => categoriesData,
//   () => {
//     console.log(categoriesData.value)
//   },
//   { immediate: true, deep: true },
// )

onMounted(async () => {
  await fetchCategories()
})
</script>
<style></style>
