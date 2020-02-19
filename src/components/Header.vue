<template>
    <div>
        <nav>
            <ul>
                <ol v-for="todo in todos" v-bind:key="todo">  
                    {{ todo.text }}
                </ol>
            </ul>
            <form>
                <input type="search" placeholder="Search" aria-label="Search">
                <button type="submit">Search</button>    
            </form>
        </nav>
    </div>
</template>

<script>
export default {
    name: "Header",
    data() {
        return{
            todos: [
                { text: "Topic 1" },
                { text: "Topic 2" },
                { text: "Topic 3" },
                { text: "Topic 4" }, 
            ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div {
    border:1px solid;
    margin: auto;
    padding-bottom: 10px;
    padding-right: 10px;
    text-align: right;
}

ul {
  list-style-type: none;
}

ol {
  display: inline;
  margin: 0 10px;
}

form {
    display: inline;
    margin-right: 10px;
}
</style>