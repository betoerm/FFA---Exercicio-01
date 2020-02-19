<template>
    <div>
        <ul>
            <li v-for="image in images" v-bind:key="image.content">
                <img {{image.content}}/>
            </li>
        </ul>
                
    </div>    
</template>

<script>
export default {
    name: "Images",
    data(){
        return{
            images: [
                {content: {          
                    alt: "Image 1 ",
                    src: "#"
                }},

                {content: {          
                    alt: "Image",
                    src: "#"
                }},

                {content: {          
                    alt: "Image",
                    src: "#"
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