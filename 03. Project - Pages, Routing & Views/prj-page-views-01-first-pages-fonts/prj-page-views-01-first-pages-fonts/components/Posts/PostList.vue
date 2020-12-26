<template>
    <section class="post-link">
          <PostPreview :is-admin="isAdmin" id="1" title="Blog title 1" previewText="Preview Text 1"/>
          <PostPreview :is-admin="isAdmin" id="2" title="Blog title 2" previewText="Preview Text "/>
    </section>
</template>

<style scoped>
    .post-link {
    display: flex;
    padding: 20px;
    box-sizing: border-box;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    }
</style>

<script>
import PostPreview from "@/components/Posts/PostPreview.vue"
export default {
  props: {
      isAdmin: {
          type: Boolean,
          default: false
      }
  },
    components: {
        PostPreview
    }
}
</script>