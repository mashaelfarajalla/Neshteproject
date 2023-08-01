<template>
  <div class="announcement2section">
    <h3 class="mt-3">المزيد من الإعلانات</h3>
    <div
      v-for="item in Announcement"
      :key="item.id"
      class="row mt-4 justify-content-center"
    >
      <h4>{{ item.title }}</h4>
      <div class="col-12 rounded-3 my-1">
        <img :src="item.image" class="w-100" />
      </div>
    </div>
  </div>
</template>
<script>
import axios from "axios";

export default {
  data() {
    return {
      Announcement: [],
    };
  },
  async mounted() {
    let result = await axios.get("http://localhost:3000/Announcement2");
    this.Announcement = result.data;
    console.log(result.data);
  },
};
</script>
