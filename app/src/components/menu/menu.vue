<template src="./menu.html"></template>

<script>
export default {
  data() {
    return {
      menus: [
        { path: "trainList", text: "路線検索", icon: "el-icon-search" },
        { path: "watchList", text: "登録路線状況", icon: "el-icon-tickets" },
        { path: "realTimeInfo", text: "つぶやき検索", icon: "el-icon-time" }
      ]
    };
  },
  methods: {
    changePage(pageName) {
      this.$router.push("/" + pageName);
    }
  }
};
</script>