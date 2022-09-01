<template>
  <button class="button-icon-container">
    <ui-icon class="button-icon">{{ iconName }}</ui-icon>
    <p class="label">{{ label }}</p>
  </button>
</template>

<script>
export default {
  props: ["iconName", "label"],
  metaInfo() {
    return {
      title: this.iconName,
      label: this.label,
    };
  },
};
</script>

<style>
.button-icon {
}

.button-icon-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: transparent;
  border: 0;
  color: #e96f95;
  margin: 0 10px;
}

.button-icon-container:hover {
  color: #f7e6ed;
}

.label {
}
</style>
