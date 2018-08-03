<template>
    <div class="previewItemWrapper">
        <a :href="previewItem.imgUrl"><img :src="previewItem.imgUrl" alt="img"></a>
        <h3>{{previewItem.heading}}</h3>
        <hr>
        <p>{{previewItem.textContent}}</p>
        <a :href="previewItem.readMoreLink" class="btn-read-more">rEad MoRe</a>
    </div>
</template>

<script>
    export default {
        name: "AppPreviewListItem",
        props:{
            'previewItem':{
                imgUrl:'',
                heading:'',
                readMoreLink:'',
                textContent:'',
                id:''
            }
        }
    }
</script>

<style>
    .previewItemWrapper{
        padding:0 1em 150px 1em;
        position: relative;
        flex-basis:calc(33.33333% - 2em);
    }
    .previewItemWrapper img{
        height:140px;
    }
    .previewItemWrapper h3{
        margin-top:30px;
    }
    .btn-read-more{
        position: absolute;
        bottom:0;
        left:0;
        right:0;
        text-decoration: none;
        border:1px solid rgba(0,0,0,0.125);
        padding:1em 1.7em;
        width:50%;
        margin:auto;
        background-color:#A00000;
        color:#fff;
        text-transform:uppercase;
    }
    .btn-read-more:hover{
        background-color:#B10000;
    }
</style>