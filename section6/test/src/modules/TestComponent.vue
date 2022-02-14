<template>
  <div class="red-b">
    <div class="border__blue">scssのテストです</div>
    <div class="background__primary">scssグローバルのテスト</div>
    テストです {{ testData }}
  </div>
</template>

<script>
export default {
  name: "TestComponent",
  data() {
    return {
      testData: "テストdataです",
    };
  },
};
</script>

<style scoped lang="scss">
.red-b {
  border: red 1px solid;
}

.border {
  &__blue {
    border: 1px blue solid;
  }
}

.background__primary {
  background-color: $color-primary;
}
</style>
