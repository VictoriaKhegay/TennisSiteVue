<!-- <template>
  <div class="block">
    <div class="accordeon">
      <h2 class="prices-block__title">Цены и абонементы</h2>

      <PriceButtonComponent
        v-for="(button, index) in buttons"
        :buttonContent="button.buttonContent"
        :key="index"
      />
    </div>
    <SliderServicesComponent :items="services" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import PriceButtonComponent from "@/components/Prise/PriceButton.vue";
import SliderServicesComponent from "@/components/Prise/SliderServises.vue";

@Component({
  components: {
    PriceButtonComponent,
    SliderServicesComponent,
  },
})
export default class PricesBlockComponent extends Vue {
  buttons = [
    {
      buttonContent: "Зимний сезон 2021-2022",
    },
    {
      buttonContent: "Абонементы",
    },
    {
      buttonContent: "Скидки",
    },
    {
      buttonContent: "Дополнительные услуги",
    },
  ];
}
</script>

<style scoped lang="scss">
.block {
  display: flex;
  justify-content: space-between;
  margin-top: 150px;
}
.accordeon {
  &__title {
    margin-bottom: 75px;
    font-weight: 700;
    font-size: 36px;
  }
}
</style> -->
