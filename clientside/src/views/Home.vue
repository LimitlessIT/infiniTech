<template>
  <div class="home">
    <ProductCard title="Dell XPS 13, 8GB RAM 256GB NVME SSD With Intel i7 1185G7" price=2.3 oldprice=3 onsale=true photourl="https://www.notebookcheck.biz/fileadmin/Notebooks/News/_nc3/Dell_XPS_13_9310.jpg" />
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
