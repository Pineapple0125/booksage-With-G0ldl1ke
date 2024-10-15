<!-- BookItem.vue -->

<template>
  <div :data-category="book.category" class="book-item col-xs-12 col-sm-6 col-md-4">
    <div class="pro-text text-center">
      <div class="pro-img">
        <img :src="book.imageSrc" :alt="book.title" style="height: 280px; width: 220px; padding: 10px;">
        <div class="hover-icon">
          <router-link :to="{ name: 'ShopDetail', query: { index: book.id, bookname: book.title } }" target="_blank"><span class="icon icon-Search"></span></router-link>
        </div>
      </div>
      <div class="pro-text-outer">
        <span>{{ book.category }}</span>
        <router-link :to="{ name: 'ShopDetail', query: { index: book.id, bookname: book.title } }" target="_blank">
          <h4>{{ truncateTitle(book.title) }}</h4>
        </router-link>
        <p class="wk-price">{{ book.price }}</p>
		<p>Sales: {{book.sale}}</p>
        <a href="#" class="add-btn">Add to cart</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['book'],
  methods:{
	  truncateTitle(title) {
	        if (title.length > 20) {
	          return title.substring(0, 20) + '...';
	        }
	        return title;
	  }
  }
};
</script>

<style scoped>
/* Add your component-specific styles here */
</style>
