<script lang="ts">
import BaseButton from './BaseButton.vue';

export default {
  components: {
    BaseButton
  },
  data() {
    return {
      posts: [{
        id: 1,
        name: 'Invite Nyx',
        link: 'https://discord.com/oauth2/authorize?client_id=960533661109878805&scope=bot%20applications.commands&permissions=336886885630'
      }, {
        id: 2,
        name: 'Support Server',
        link: 'https://discord.gg/invite/YNppjePpje'
      }, {
        id: 3,
        name: 'GitHub (Source Code)',
        link: 'https://github.com/nyx-team/nyx'
      }]
    }
  }
}
</script>

<template>
  <div class="buttons">
    <BaseButton
      v-for="post in posts"
      :key="post.id"
      :name="post.name"
      :link="post.link"
    />
  </div>
</template>

<style scoped>
.buttons {
  display: flex;
  align-items: center;
  flex-direction: column;

  margin-top: -3rem;
}

.buttons > a {
  margin: 6px;
}
</style>
