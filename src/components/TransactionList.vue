<template>
    <h3>History</h3>
    <ul id="list" class="list">
        <li v-for="transaction in transactions" :key="transaction.id">
            cash <span>-$400</span>
            <button class="delete-btn">x</button>
        </li>
       
    </ul>
</template>

<script>
export default{
    data(){
        transactions: [
            {id:1, text: 'flower', amount: -19.99},
            {id:2, text: 'salary', amount: 299.99},
            {id:3, text: 'Book', amount: -10},
            {id:4, text: 'Camera', amount: 150},
        ]
    }
}
</script>