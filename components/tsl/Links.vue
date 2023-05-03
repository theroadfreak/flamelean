<template>
  <div class="container pb-5 d-flex flex-column align-items-center text-center">
    <a v-for="(link, i) in links" :key="i"
       :href="link"
       target="_blank"
       class="text-4D4D4D text-decoration-none font-size-12px"
    >
      {{ link }}
    </a>
  </div>
</template>

<script>
export default {
  name: "Links",
  data() {
    return {
      links: [
        `https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7913072/`,
        `https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3639863/`,
        `https://pubmed.ncbi.nlm.nih.gov/18326600/`,
        `https://pubmed.ncbi.nlm.nih.gov/31161192/`,
        `https://pubmed.ncbi.nlm.nih.gov/21835556/`,
        `https://pubmed.ncbi.nlm.nih.gov/21520342/`,
        `https://pubmed.ncbi.nlm.nih.gov/19109001/`,
        `https://pubmed.ncbi.nlm.nih.gov/34132409/`,
        `https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3123991/`,
        `https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5590066/`,
        `https://pubmed.ncbi.nlm.nih.gov/23883699/`,
        `https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8004891/`,
        `https://pubmed.ncbi.nlm.nih.gov/33506272/`,
        `https://pubmed.ncbi.nlm.nih.gov/30102953/`,
        `https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6126939/`,
      ]
    }
  }
}
</script>

<style scoped>

</style>
