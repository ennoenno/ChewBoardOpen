<template>
    <div class="commentBox">
      
        <div class="commentBoxTitle">
             {{comment.title}}
        </div>
        <div class="commentBoxBody">
            {{comment.owner}}

            
        </div>
        <div class="commentBoxAnswer">
            <div>
                Answer <input type="text" v-on:change="deleteComment">
            </div>
        </div>
       
    </div>
</template>

<script>
export default {
    name: "CommentItem",
    props: ["comment"],
    methods: {
        deleteComment() {
            console.log("123");
        }
    }
}
</script>

<style scoped>


.commentBox {
    margin: 20px;
    border: solid rgb(204, 204, 204) 1px;
    box-shadow: 3px 2px 14px 5px rgba(135,127,135,1);
}

.commentBoxTitle {
    padding: 10px;
    border-bottom: solid rgb(204, 204, 204) 1px;

}
.commentBoxBody {
    padding: 10px;
    border-bottom: solid rgb(204, 204, 204) 1px;

    min-height: 50px;
}

.commentBoxAnswer {
    display: flex;
    flex-direction: row-reverse;
    padding: 10px;
    
}
</style>