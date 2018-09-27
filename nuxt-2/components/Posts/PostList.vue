<template>
    <div>
        <section class="post-list">
            <PostPreview 
                id="1"
                thumbnail="https://via.placeholder.com/950x150"
                title="Hello there!"
                previewText="This my first post!"/>
            <PostPreview 
                id="2"
                thumbnail="https://via.placeholder.com/950x150"
                title="Hello there! 2" 
                previewText="This my first post! 2"/>
            <PostPreview 
                id="3"
                thumbnail="https://via.placeholder.com/950x150"
                title="Hello there! 3"
                previewText="This my first post! 3"/>
      </section>
    </div>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview';
export default{
  components:{
    PostPreview
  }
}
</script>

<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>