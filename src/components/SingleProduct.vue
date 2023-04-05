<template>
  <div class="single-product">
    <div class="img-container">
      <img src="@/assets/femProducts/p1.png" alt="" />
      <div v-if="product.sale" class="sale">-50%</div>
    </div>

    <div class="product-content">
      <h6 class="name">{{ product.name }}</h6>
      <div class="rating">
        <span class="price">{{ product.price }}</span>
        <span class="icon">
          <img src="@/assets/rating.png" alt="" />
        </span>
      </div>
    </div>
  </div>
</template>

<script setup>
  defineProps({
    product: {
      type: Object,
    },
  })
</script>

<style lang="scss" scoped>
.single-product {
  .img-container {
    position: relative;
    .sale {
      position: absolute;
      top: 0;
      left: 0;
      padding: 9px;
      background: #e91e63;
      right: auto;
      font-weight: 700;
      font-size: 12px;
      line-height: 13px;
      text-align: center;
      color: #ffffff;
    }
  }
  .product-content {
    padding: 10px 0px;

    h6 {
      font-weight: 400;
      font-size: 14px;
      line-height: 16px;
      opacity: 0.6;
    }
    .rating {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-top: 5px;
      .price {
        font-weight: 700;
        font-size: 14px;
        line-height: 16px;
      }
    }
  }
}
</style>
