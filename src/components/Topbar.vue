<template>
  <div id="Topbar">
    <ContainerComponent>
      <div class="topbar">
        <div class="topbar__logo">
          <router-link to="/">
            <img src="../assets/logo.svg" alt="" />
          </router-link>
        </div>
        <div class="topbar-menu">
          <MenuComponent />
        </div>
        <div class="topbar-social">
          <a href="https://youtube.com">
            <img src="../assets/youtube.svg" alt="" />
          </a>
          <a href="https://vk.com">
            <img src="../assets/vk.svg" alt="" />
          </a>
        </div>
      </div>
    </ContainerComponent>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import ContainerComponent from "@/components/Container.vue";
import MenuComponent from "./Menu.vue";

@Component({
  components: {
    ContainerComponent,
    MenuComponent,
  },
})
export default class extends Vue {}
</script>

<style scoped lang="scss">
#Topbar {
  border-bottom: 1px solid #ccc;
  position: absolute;
  width: 100%;
  padding: 10px;
}
.topbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  &-menu {
    color: white;
    &__list {
      display: flex;
      align-items: center;
      gap: 20px;
      cursor: pointer;
    }
  }
  &-social {
    img {
      height: 15px;
    }
    a {
      margin-left: 10px;
    }
  }
}
</style>
