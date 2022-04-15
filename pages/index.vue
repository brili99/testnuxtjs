<template>
  <div>
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
  </div>
</template>

<script>
import MenuBarNav from "../components/MenuBarNav.vue";
import MenuSideBar from "../components/MenuSideBar.vue";
export default {
  name: "IndexPage",
  components: { MenuBarNav, MenuSideBar },
};
</script>
