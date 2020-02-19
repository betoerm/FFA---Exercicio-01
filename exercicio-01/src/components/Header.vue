<template>
    <div id="header">
       <img alt="logo" src="#">
        <ul>
            <li v-for="list in lists" v-bind:key="list.text">
                {{list.text}}
            </li>
        </ul>
         <input type="text" placeholder="Search..">
    </div>    
</template>

<script>
export default {
    name: "Header",
    data(){
        return{
            lists: [
                {text: "Topic 1"},
                {text: "Topic 2"}, 
                {text: "Topic 3"}, 
                {text: "Topic 4"}, 
            ]
        };
    }    
};
</script>

<style scoped>

    #header{
         border-style: solid;
    }
    img {
        width: 5%;
        height: 5%;
    }

   ul{
        list-style-type: none;
    }

    li{
        display: inline;
    }

</style>