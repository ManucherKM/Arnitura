<template>
  <div class="wrapper-form">
    <h2 class="wrapper-form__title">Добавить товар</h2>
    <div class="wrapper-form__form">
      <div class="wrapper-form__container">
        <div class="wrapper-form__wrapper-inpt">
          <p class="text name">Наименование</p>
          <input
            v-model="modelName"
            type="text"
            placeholder="Иван Иванов"
            class="wrapper-form__input"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      modelName: "",
      modelCategory: "",
      modelType: "",
      modelWidth: "",
      modelLength: "",
      modelHeight: "",
      file: "",
      modelMaterial: "",
      modelPrice: "",
      modelDecription: "",
      modelTime: "",
      StatsModeration: true,
      StatsVerify: false,
      Statsreject: false,
      Photo: {
        name: "Фото",
      },
    };
  },
  methods: {
    addFile(event) {
      this.file = event.target.files[0].name;
    },
  },
};
</script>

<style>
</style>