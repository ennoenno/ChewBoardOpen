<template>
<div>
    <div v-bind:key="comment.id" v-for="comment in comments">
        <CommentItem v-bind:comment="comment"/>
  
    </div>
</div>    
</template>

<script>
import CommentItem from './CommentItem'

export default {
    name: "Comments",
    components: {
        CommentItem
    },
    props: ["comments"]
    
}

</script>

<style scoped>

</style>