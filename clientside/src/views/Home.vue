<template>
  <div class="home">
    <main class="mt-10 mx-auto max-w-7xl px-4 sm:mt-12 sm:px-6 md:mt-16 lg:mt-20 lg:px-8 xl:mt-28">

      <ProductCard title="Dell XPS 13, 8GB RAM 256GB NVME SSD With Intel i7 1185G7" price=2.3 oldprice=3 onsale=true photourl="https://www.notebookcheck.biz/fileadmin/Notebooks/News/_nc3/Dell_XPS_13_9310.jpg" />
    </main>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld  from '@/components/HelloWorld.vue'
import ProductCard from '@/components/ProductCard.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    ProductCard
  }
}
</script>
