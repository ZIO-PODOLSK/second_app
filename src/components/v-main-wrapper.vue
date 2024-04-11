<template>
  <vCatalog />
  <div class="v-main-wrapper"></div>
  <vCart />
</template>

<script>
import vCatalog from "./v-catalog.vue";
import vCart from "./v-cart.vue";

export default {
  name: "v-main-wrapper",
  components: { vCatalog, vCart },
  props: {},
  data() {
    return {
      title: "hello all",
    };
  },
  computed: {},
  methods: {},
  watch: {},
  mounted() {
    console.log("Я смонтировался");
  },
};
</script>

<style lang="scss">
.v-main-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  max-width: 900px;
  margin: 0 auto;
}
</style>