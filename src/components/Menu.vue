<template>
    <div>
        <nav>
            <ul>
                <ol v-for="todo in todos" v-bind:key="todo">  
                    {{ todo.text }}
                </ol>
            </ul>
        </nav>
    </div>
</template>

<script>
export default {
    name: "Menu",
    data() {
        return{
            todos: [
                { text: "Section 1" },
                { text: "Section 2" },
                { text: "Section 3" },
                { text: "Section 4" }, 
            ]
        }
    }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div {
    border:1px solid;
    margin-bottom: 10px;
    margin-left: 5px;
    margin-right: 5px;
    margin-top: 10px;   
}

ul {
   list-style-type: none;
   padding: 0;
}
ol {
   display: inline;
   margin: 0 10px;
}

</style>