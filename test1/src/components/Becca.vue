<template>
  <div>
    <!-- 이곳에 Home, About에서 지정한 타이틀 전달 -->
    <h1>{{ title }}</h1>

    <p>{{ name }}</p>
    <br />
    <button @click="updateName">Change Name</button>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      // required: false, // true : 무조건 title을 지정해야 함 (안쓰면 콘솔에 오류 메세지)
      default: "Default Title", // title을 지정하지 않으면 이걸 대신 사용
    },
    name: {
      type: String,
      default: "default name",
    },
  },
  data() {
    return {
      // name: "Becca", // props에 name을 사용해서 이것을 사용 불가능
    };
  },
  methods: {
    updateName() {
      this.name = "Becca Updated";
    },
  },
};
</script>

<style scoped>
</style>