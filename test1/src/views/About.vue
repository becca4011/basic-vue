<template>
  <div class="about">
    <h1>This is an about page</h1>
    <Becca />
  </div>
</template>

<script>
import Becca from "@/components/Becca.vue"; // import를 하면 사용 가능

export default {
  components: {
    Becca,
  },
};
</script>