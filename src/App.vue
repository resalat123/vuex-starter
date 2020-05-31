<template>
    <div id="app">
        <compBookListOne :book="books"></compBookListOne>
        <compBookListTwo :book="books"></compBookListTwo>
    </div>
</template>

<script>
import compBookListOne from "./components/BookListOne"
import compBookListTwo from "./components/BookListTwo"
export default {
    data(){
        return{
            books: [
              {name: "Harry Potter", price: 100},
              {name: "Lord of The Rings", price: 150},
              {name: "Night Circus", price: 90},
              {name: "Lost World", price: 200}
            ]
        }
    },
    components:{
      compBookListOne,
      compBookListTwo
    }
}
</script>
