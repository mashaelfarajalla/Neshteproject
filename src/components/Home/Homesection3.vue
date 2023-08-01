<template>
  <div class="container mt-5">
    <div class="row justify-content-between">
      <div class="col-6 col-lg-3 order-2 order-lg-1">
        <div class="row">
          <div
            class="col-auto rounded-3"
            style="
              box-shadow: 0px 10px 50px 0px rgba(0, 0, 0, 0.1);
              height: max-content;
            "
          >
            <TypesSection />
          </div>
        </div>

        <div class="row mt-5">
          <div class="col-auto">
            <Announcement4 class="w-100" />
          </div>
        </div>
      </div>
      <div class="col-lg order-1 me-3 order-lg-2">
        <CuttingSection />
        <Announcement />
        <CuttingSection />
        <Announcement3 />
        <CuttingSection />
      </div>
    </div>
  </div>
</template>
<script>
import Announcement from "../Announcement.vue";
import CuttingSection from "../CuttingSection.vue";
// import TypesSection from "./TypesSection";
import TypesSection from "../TypesSection.vue";
import Announcement2 from "../Announcement2";
import Announcement3 from "../Announcement3";
import Announcement4 from "../Announcement4";

export default {
  components: {
    TypesSection,
    CuttingSection,
    Announcement,
    Announcement2,
    Announcement3,
    Announcement4,
  },
};
</script>
