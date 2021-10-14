<!-- HTML 코드가 들어갈 곳 -->
<template>
  <div>
    <h1>This is Home Page</h1>

    <form action="">
      <!-- <InputField :name="name" @update-name="updateName" /> -->
      <!-- <InputField :name="name" @update-name="name = $event.target.value" /> -->
      <InputField v-model="name" />
      <br /><button>Submit</button>
    </form>
    {{ name }}

    <!-- props -->
    <!-- <Becca title="Home Title" name="Becca" /> -->
  </div>
</template>

<!-- 데이터, 메소드 등 배웠던 것이 들어갈 곳 -->
<script>
// import Becca from "@/components/Becca.vue"; // import를 하면 사용 가능
import InputField from "@/components/InputField.vue";

export default {
  components: {
    InputField,
  },
  data() {
    return {
      name: "",
    };
  },
  // methods: {
  //   updateName(name) {
  //     this.name = name; // name에 e.target.value가 넘어옴
  //   },
  // },
  // components: {
  //   Becca,
  // },
};
</script>

<!-- HTML 스타일이 들어갈 곳 -->
<!-- scoped : 이 HTML 페이지에만 적용 (쓰지 않으면 전체에 적용됨) -->
<style scoped>
h1 {
  color: #42b983;
}
</style>