<template>
    <div id="images">
        <ul>
            <li v-for="list in lists" v-bind:key="list.text">
                {{list.text}}
            </li>
        </ul>
    </div>    
</template>

<script>
export default {
    name: "Images",
    data(){
        return{
            lists: [
                {text: "Image 1"},
                {text: "Image 2"}, 
                {text: "Image 3"}, 
                {text: "Image 4"}, 
            ]
        };
    }    
};
</script>

<style scoped>
   ul{
        list-style-type: none;
    }

    li{
         border-style: solid;
    }

</style>