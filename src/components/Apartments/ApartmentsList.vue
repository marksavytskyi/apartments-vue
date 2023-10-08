<template>
  <div class="apartments-list">
    <ApartmentsItem
      v-for="{id, imgUrl, descr, rating, price} in items"
      :key="id"
      :descr="descr"
      imgSrc="/public/img/apartment-1.jpg"
      :rating="rating"
      :price="price"
    />
  </div>
</template>

<script>
import ApartmentsItem from "./ApartmentsItem.vue";
export default {
  name: "ApartmentsList",
  components: {ApartmentsItem},
  props: {
    items: Array,
    default: () => [],
  },
};
</script>

<style lang="scss" scoped>
.apartments-list {
  display: flex;
  flex-wrap: wrap;
  margin-left: -15px;
  margin-right: -15px;
}
</style>
