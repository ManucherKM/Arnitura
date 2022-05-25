<template>
  <div class="wrapper-product">
    <table class="wrapper-product__table">
      <tr class="wrapper-product__line">
        <td
          class="wrapper-product__column title-table wrapper-product__null"
        ></td>
        <td class="wrapper-product__column title-table wrapper-product__name">
          Наименование
        </td>
        <td
          class="wrapper-product__column title-table wrapper-product__category"
        >
          Категория
        </td>
        <td class="wrapper-product__column title-table wrapper-product__type">
          Тип
        </td>
        <td class="wrapper-product__column title-table wrapper-product__width">
          Ширина
        </td>
        <td class="wrapper-product__column title-table wrapper-product__length">
          Длина
        </td>
        <td class="wrapper-product__column title-table wrapper-product__height">
          Высота
        </td>
        <td
          class="wrapper-product__column title-table wrapper-product__file-3D"
        >
          Файл 3D модели
        </td>
        <td
          class="wrapper-product__column title-table wrapper-product__material"
        >
          Материал
        </td>
        <td class="wrapper-product__column title-table wrapper-product__price">
          Цена товара
        </td>
        <td class="wrapper-product__column title-table wrapper-product__desc">
          Описание
        </td>
        <td class="wrapper-product__column title-table wrapper-product__time">
          Дата и время публикации
        </td>
        <td class="wrapper-product__column title-table wrapper-product__stats">
          Статус
        </td>
        <td class="wrapper-product__column title-table wrapper-product__photo">
          Фото
        </td>
        <td
          class="wrapper-product__column title-table wrapper-product__null"
        ></td>
      </tr>
      <Table  v-for="item in massLine" :key="item.name" />
    </table>
  </div>
</template>

<script>
import Table from "../components/Table.vue";
export default {
  components: { Table },
  layout: "leftnav",
  data() {
    return {
      massLine: [
        {
          name: "Генрих 8",
          caregoty: "Для спальни",
          width: "Кресло",
          length: 65,
          height: 80,
          articl: 80,
          file3D: "уавфкиме.ew",
          material: {
            Кожа: "Кожа",
            Вельвет: "Вельвет",
          },
          price: "Генрих 8",
          description: "Описание",
          StatsModeration: true,
          StatsVerify: false,
          Statsreject: false,
          Photo: "Фото",
        },
        {
          name: "Генрих 10",
          caregoty: "Для спальни",
          width: "Кресло",
          length: 65,
          height: 80,
          articl: 80,
          file3D: "уавфкиме.ew",
          material: {
            Кожа: "Кожа",
            Вельвет: "Вельвет",
          },
          price: "Генрих 8",
          description: "Описание",
          StatsModeration: true,
          StatsVerify: false,
          Statsreject: false,
          Photo: "Фото",
        },
        {
          name: "Генрих 9",
          caregoty: "Для спальни",
          width: "Кресло",
          length: 65,
          height: 80,
          articl: 80,
          file3D: "уавфкиме.ew",
          material: {
            Кожа: "Кожа",
            Вельвет: "Вельвет",
          },
          price: "Генрих 8",
          description: "Описание",
          StatsModeration: true,
          StatsVerify: false,
          Statsreject: false,
          Photo: "Фото",
        },
      ],
    };
  },
};
</script> 

<style>
</style>