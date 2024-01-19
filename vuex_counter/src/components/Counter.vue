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
    export default {
        methods: {
            increment() {
                this.$store.commit('INCREMENT_COUNTER');
            },
            decrement() {
                //this.currentValue = this.currentValue -1;
            }
        },
        computed: {
            currentValue() {
                return this.$store.state.currentValue;
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>