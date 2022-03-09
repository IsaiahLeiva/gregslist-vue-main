<template>
  <router-link :to="{ name: 'HouseDetails', params: { id: house.id } }">
    <div>
      <div class="col-12">
        <img class="img-fluid" :src="house.imgUrl" alt="" />
      </div>
      <h3 class="text-center col-12">
        Bedrooms: {{ house.bedrooms }} | Bathrooms: {{ house.bathrooms }}
      </h3>
      <div class="col-12"></div>
    </div>
  </router-link>
</template>


<script>
export default {
  props: {
    house: {
      type: Object,
      required: true,
    },
  },
  setup() {
    return {};
  },
};
</script>


<style lang="scss" scoped>
</style>