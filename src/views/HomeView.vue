<template>
  <Section1 />
  <Section2 />
  <Section3 />
</template>

<script>
import Section1 from "@/components/Home/Homesection1.vue";
import Section2 from "@/components/Categories.vue";
import Section3 from "@/components/Home/Homesection3.vue";

export default {
  name: "HomeView",
  components: {
    Section1,
    Section2,
    Section3,
  },
};
</script>
