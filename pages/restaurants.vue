<template>
  <main class="container restaurant">
    <div class="restaurantheading">
      <h1>Restaurants</h1>

      <AppSelect @change="selectedRestaurant = $event" />
      <pre>{{ $data }}</pre>
    </div>
    <AppRestaurantInfo />
  </main>
</template>

<script>
import AppRestaurantInfo from "@/components/AppRestaurantInfo.vue";
import AppSelect from "@/components/AppSelect.vue";

export default {
  data() {
    return {
      selectedRestaurant: "",
    };
  },
  components: {
    AppRestaurantInfo,
    AppSelect,
  },
};
</script>

<style lang="scss" scoped>
</style>
