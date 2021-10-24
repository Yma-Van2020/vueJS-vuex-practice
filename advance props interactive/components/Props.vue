<template>
    <div>
        <h1>My Show</h1>
        
        <p><strong>Title</strong> {{ title }}</p>
        <p><strong>Episode #</strong> {{ episodeNumber }}</p>
        <p><strong>Published</strong> {{ published }}</p>
        <p v-show="isVisible"><strong>Optional</strong> {{ isVisible }}</p>
    </div>
</template>

<script>
    module.exports = {
        props:{
            title:{
                type:String,
                default: 'This is the default title'
            },
            published:{
                type:[Boolean, Number],
                default: false
            },
            episodeNumber:{
                type:Number,
                default: 18
            },
            isVisible:{
                type:Boolean,
                default:true
            }
        },
        
    }
</script>

<style>
    
</style>