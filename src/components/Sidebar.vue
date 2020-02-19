<template>
    <div>
        <nav>
            <ul>
                <ol v-for="todo in sidebar" v-bind:key="todo">  
                    {{ todo.text }}
                </ol>
            </ul>
        </nav>
    </div>
</template>

<script>
export default {
    name: "Sidebar",
    data() {
        return{
            sidebar: [
                { text: "Section 1" },
                { text: "Section 2" },
                { text: "Section 3" },
                { text: "Section 4" },
                { text: "Section 5" },
                { text: "Section 6" },
                { text: "Section 7" },
                { text: "Section 8" }, 
                { text: "Section 9" },
                { text: "Section 10" },
                { text: "Section 11" },
                { text: "Section 12" },
                { text: "Section 13" },
                { text: "Section 14" },
                { text: "Section 15" }   
            ]
        }
    }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div {
    border:1px solid;
    margin-bottom: 20px;
    margin-right: 5px;
    margin-top: 20px; 
    width: 210px; 
    float: right;
    height: 700px
   
}

ul {
   list-style-type: none;
   padding: 0;
}
ol {
   
   text-align: left;
   padding-top: 14px;
   padding-bottom: 5px;
}

</style>