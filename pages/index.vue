<template>
  <!-- <div>
    <MenuBarNav />
    <MenuSideBar />
    <div>
      <b-jumbotron>
        <template #header>BootstrapVue</template>

        <template #lead>
          This is a simple hero unit, a simple jumbotron-style component for
          calling extra attention to featured content or information.
        </template>

        <hr class="my-4" />

        <p>
          It uses utility classes for typography and spacing to space content
          out within the larger container.
        </p>

        <b-button variant="primary" href="#">Do Something</b-button>
        <b-button variant="success" href="#">Do Something Else</b-button>
      </b-jumbotron>
    </div>
    <b-button v-b-toggle.sidebar-1>Toggle Sidebar</b-button>
  </div> -->
  <section style="width: 100%">
    <full-page>
      <section class="section" style="background: #f59e0b" id="page1">
        <MenuBarNav />
        <div>Page one</div>
      </section>
      <section class="section" style="background: #ef4444" id="page2">
        <div>Page Two</div>
      </section>
      <section class="section" style="background: #001122" id="page3">
        <div>Page Three</div>
      </section>
    </full-page>
  </section>
</template>

<script>
import MenuBarNav from "../components/MenuBarNav.vue";
import MenuSideBar from "../components/MenuSideBar.vue";
export default {
  name: "IndexPage",
  components: { MenuBarNav, MenuSideBar },
};
</script>

<style scoped>
.section {
  height: 100vh;
  width: 100%;
  /* display: flex;
  align-items: center;
  justify-content: center;
  font-size: 25px; */
}
</style>