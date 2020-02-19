<template>
    <div>
        <ul>
            <li v-for="section in sections" v-bind:key="section.text">
                {{section.text}}
            </li>
        </ul>    
    </div>    
</template>

<script>
export default {
    name: "SectionHeader",
    data(){
        return{
            sections: [
                {text: "Section 1"},
                {text: "Section 2"}, 
                {text: "Section 3"}, 
                {text: "Section 4"}, 
            ]
        };
    }      
}
</script>

<style scoped>
   ul{
        list-style-type: none;                
        border-style: solid;
    }

    li{
        display: inline;
    }
    
</style>
