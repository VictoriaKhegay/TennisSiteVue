<template>
  <div class="rules-general">
    <h3>Основные определения</h3>
    <ul>
      <li>
        Площадь теннисного корта в квадратных метрах для одиночной игры
        рассчитывается от стандартной длины игровой площадки – 23,78 м (или 78
        футов) и ширины в 8,23 м (27 футов)
      </li>
      <li>
        Размер теннисного корта в квадратных метрах для парной игры также
        исходят от стандартной длины - 23,78 м (или 78 футов), но уже другой
        ширины - 10,97 м (36 футов)
      </li>
    </ul>
    <img src="../assets/img/cort-size.jpg" alt="" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component({
  name: "DefinitionsView",
})
export default class DefinitionsView extends Vue {}
</script>

<style scoped lang="scss">
.rules-general {
  max-width: 856px;
  margin: 0 auto;
  padding-left: 50px;
  color: #333333;
  font-size: 14px;
}
ul {
  list-style-type: square;
}
li {
  padding-bottom: 40px;
}
img {
  padding-top: 30px;
  align-items: center;
}
h3 {
  font-size: 18px;
  padding-bottom: 25px;
}
</style>
