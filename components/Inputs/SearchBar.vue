<template>
  <div class="search-bar-container">
    <ui-icon class="search-bar-icon">search</ui-icon>
    <input class="search-bar-input" placeholder="Mon futur jouet sera ..." />
  </div>
</template>

<style scoped>
.search-bar-container {
  display: flex;
  width: 40%;
  margin-bottom: 15px;
  border-radius: 30px;
  border: 2px solid #f2becf;
}

.search-bar-input {
  width: 100%;
  padding: 10px;
  outline: none;
  border: 0;
  border-radius: 30px;
  color: #e96f95;
}

.search-bar-input:focus {
  outline: none;
}

.search-bar-input::placeholder {
  color: #e96f95;
}

.search-bar-icon {
  padding: 10px;
  text-align: center;
  color: #f7e6ed;
}
</style>
