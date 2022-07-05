<script lang="ts">
export default {
    props: ['name', 'link']
}
</script>

<template>
  <a :href="link">
    <button class="button" id="basebtn">
      <span>{{ name }}</span>
    </button>
  </a>
</template>

<style scoped>
#basebtn {
  text-decoration: none;
  text-align: center;

  border: none;
  border-radius: 16px;

  cursor: pointer;
}

.button {
  display: inline-block;
  background-color: #9edb25;

  color: midnightblue;
  padding: 14px 30px;
  font-size: 1.5rem;
  font-family: 'Inconsolata', monospace;

  transition: ease 0.5;
}

.button span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}

.button span:after {
  content: "→";
  position: absolute;
  opacity: 0;
  top: 0;
  right: -20px;
  transition: 0.5s;
}

.button:hover span {
  padding-right: 25px;
}

.button:hover span:after {
  opacity: 1;
  right: 0;
}
</style>