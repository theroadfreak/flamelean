<template>
  <nav class="bg-primary navbar navbar-expand-lg">
    <div class="container d-flex align-items-center py-2">
      <nuxt-link to="/" class="navbar-brand">
        <img
          src="../../assets/images/layouts/custom-navbar/logo.svg"
          alt="Flamelean's Logo"
          width="150"
          height="34"
        />
      </nuxt-link>
      <button
        class="navbar-toggler border-0 p-0"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbar"
        aria-controls="navbar"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <i class="fa fa-bars fs-1 fw-light text-white"></i>
      </button>
      <div
        id="navbar"
        class="collapse navbar-collapse d-lg-flex justify-content-lg-end py-2 py-lg-0"
      >
        <ul
          class="navbar-nav d-flex flex-column flex-lg-row align-items-center justify-content-center mx-auto"
        >
          <li v-for="(link, i) in links" :key="i" class="nav-item mx-3">
            <nuxt-link
              v-if="link.to"
              class="nav-link text-decoration-none text-white fw-light"
              :to="link.to"
            >{{ link.name }}
            </nuxt-link>
          </li>
        </ul>
        <div class="d-flex justify-content-center text-center">
          <button
            class="nav-item btn btn-light text-primary rounded rounded-3 px-3 mt-2 mt-lg-0"
          >
            Order Now
          </button>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "CustomNavbar",
  data() {
    return {
      links: [
        {
          name: "About Flamelean",
          to: "/",
        },
        {
          name: "Ingredients",
          to: "/",
        },
        {
          name: "FAQ",
          to: "/",
        },
      ],
    };
  },
}
</script>

<style scoped>
.navbar-toggler:focus {
  box-shadow: none !important;
}
</style>
