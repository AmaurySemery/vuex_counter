// snippet vbase

<template>
    <div>
        <h2>{{ currentValue }}</h2>
        <div>
            <button @click="increment">+</button>
            <button @click="decrement">-</button>
        </div>
    </div>
    
</template>

<script>
// snippet vdata
    export default {
        data() {
            return {
                currentValue: 0
            }
        },
// snippet vmethod
        methods: {
            increment() {
                this.currentValue = this.currentValue +1;
            },
            decrement() {
                this.currentValue = this.currentValue -1;
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>