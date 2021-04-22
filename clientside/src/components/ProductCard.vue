<template>
  <div class="card">  
      
      <div class="image" v-bind:style="{ backgroundImage: 'url(' + photourl + ')' }" />
      <p href="" class="title">{{ title }}</p>
      <p><span class="oldprice">{{ oldprice }}</span> <span class="newprice">{{ price }}</span></p>
  </div>
</template>

<script>
import { Number } from "core-js";

export default {
  name: 'ProductCard',
  props: {
      title: String,
      price: Number,
      oldprice: Number,
      onsale: Boolean,
      photourl: String,
  }
}
</script>

<style scoped>
  .card:hover{
    cursor:pointer;
  }
  .card{
    display: flex;
    height:max-content;
    flex-direction: column;
    align-items: center;

    width: 10em;
    height:20em;
  }
  .title{
    font-family: Poppins;
    font-style: normal;
    font-weight: normal;
    font-size: 13px;
    line-height: 19px;
    align-self: center;
    overflow:hidden;
    text-overflow:ellipsis;
    display:-webkit-box;
    -webkit-box-orient:vertical;
    -webkit-line-clamp:2;
    margin: 10px 0px;
  }

  .image{
      height: 14vh;
      width:100%;
      background-position:center;
      background-repeat: no-repeat;
      background-size: 100%;
  }

  .oldprice{

    font-size: 13px;
    line-height: 140%;
    align-self:flex-end;

    /* or 20px */
    text-decoration-line: line-through;

    /* Color - 11 */
    color: #666666;
    margin: 10px 0px;
  }
.newprice{
    font-weight:bold;
    color:black;
    margin: 10px 20px;
}
</style>
