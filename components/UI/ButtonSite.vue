<template>
  <button type="submit" class="wrapper-res__btn btn" @click="btnClick">
    {{ textBtn }}
  </button>
</template>

<script>
export default {
  props: {
    textBtn: {
      required: true,
      type: String,
    },
  },
  methods: {
    btnClick() {
      this.$emit("btnClick", "Нажатие");
    },
  },
};
</script>

<style>
</style>