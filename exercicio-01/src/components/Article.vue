<template>
    <div>
        <ul>
            <li v-for="article in articles" v-bind:key="article.content">
               <article>{{article.content.}}</article>
            </li>
        </ul>
                
    </div>    
</template>

<script>
export default {
    name: "Article",
    data(){
        return{
            articles: [
                {content: {          
                    title: "Title 1 ",
                    content: "Content 1"
                }},

                {content: {          
                    title: "Title 2",
                    content: "Content 2"
                }},

                {content: {          
                    title: "Title 3",
                    content: "Content 3"
                }}
            ]
        };
    }
}
</script>

<style  scoped>
   ul{
        list-style-type: none;                        
    }

    li{
        border-style: solid;
    }
</style>