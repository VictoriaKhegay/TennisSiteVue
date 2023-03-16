<!-- <template>
  <div class="services">
    <SliderListComponent title="Услуги">
      <div
        class="about-slide-item"
        v-for="(photo, index) in services"
        :key="index"
      
      >
        <router-link tag="a" :to="photo.routeUrl">
          {{ photo.routeTitle }}
        </router-link>
      </div>
    </SliderListComponent>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import TitleComponent from "../Title.vue";
import SliderListComponent from "../slider/SliderList.vue";
import { ISliderItem } from "@/types/SliderItem";

@Component({
  components: {
    TitleComponent,
    SliderListComponent,
  },
  props: {
    items: {
      type: Array as () => ISliderItem[],
      required: false,
      default: [],
    },
  },
})
export default class SliderServicesComponent extends Vue {
  itemWidth = 636;
  offset = 0;

  services = [
    {
      image: require("@/assets/img/services.jpg"),
      title: "Уютное кафе",
    },
    {
      image: require("@/assets/img/services.jpg"),
      title: "Вкусный кофе",
    },
    {
      image: require("@/assets/img/services.jpg"),
      title: "Полезные завтраки",
    },
  ];
}
</script>

<style scoped lang="scss">
.services {
  width: 636px;
  &__slider {
    border: 1px solid #f7ece1;
    overflow: hidden;
    padding: 30px 0 30px 25px;
    &__line {
      transition: 0.5s;
      display: flex;
      gap: 50px;
    }
  }
}
</style> -->
