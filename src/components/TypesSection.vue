<template>
  <div
    v-for="item in Types"
    :key="item.id"
    class="row typesection mt-4 justify-content-center border-bottom"
  >
    <h4>{{ item.name }}</h4>
    <div class="row mb-4">
      <div
        v-for="i in item.images"
        :key="i.id"
        class="col-auto col-lg-3 col-xxl-auto border rounded-3 mx-2 my-1 types d-flex justify-content-center align-items-center "
      >
        <img :src="i.image" />
      </div>
    </div>
  </div>
</template>
<script>
import axios from "axios";

export default {
  data() {
    return {
      Types: [],
    };
  },
  async mounted() {
    let result = await axios.get("http://localhost:3000/types");
    this.Types = result.data[0];
    console.log(result.data);
  },
};
</script>
