<template>
    <div>
        <div id="article" v-for="todo in articles" v-bind:key="todo" >
                    {{ todo.text }}
        </div>
    </div>
</template>

<script>
export default {
    name: "Article",
    data() {
        return{
            articles: [
                { text: "Lorem ipsum augue eu volutpat potenti morbi per conubia in nostra sagittis vehicula porttitor, suscipit tristique aenean auctor enim mauris sociosqu sollicitudin ac pretium ut. commodo leo fringilla morbi fames quisque maecenas congue quis, facilisis nibh iaculis ligula commodo morbi. " },
                { text: "Lorem ipsum augue eu volutpat potenti morbi per conubia in nostra sagittis vehicula porttitor, suscipit tristique aenean auctor enim mauris sociosqu sollicitudin ac pretium ut. commodo leo fringilla morbi fames quisque maecenas congue quis, facilisis nibh iaculis ligula commodo morbi. " },
                { text: "Lorem ipsum augue eu volutpat potenti morbi per conubia in nostra sagittis vehicula porttitor, suscipit tristique aenean auctor enim mauris sociosqu sollicitudin ac pretium ut. commodo leo fringilla morbi fames quisque maecenas congue quis, facilisis nibh iaculis ligula commodo morbi. " } 
            ]
        }
    }
}
</script>

<style scoped>
#article{
    border:1px solid;
    height: 210px;
    text-align: left;
    margin-top: 30px;
    margin-bottom: 10px;
    padding-top: 10px;
    padding-left: 5px;
    width: 500px;
    
}
div{
    margin-right: auto;
    margin-left: auto;
}

</style>