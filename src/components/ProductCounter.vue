<template>
    <div class="root">
    <label>Выберете кол-во продуктов</label>
    <label>
        <button
            @click="DecrementCount"
        >-</button>
        <input
            type="number"
            :value="count"
            @input="InputCount($event.target.value)"
        />
        <button
            @click="IncrementCount"
        >+</button>
    </label>
    </div>
</template>

<script>
export default {
        name: 'ProductCounter',
        data() {
            return {
                count: 0
            }
        },
    methods: {
        IncrementCount() {
            this.count++
        },
        DecrementCount() {
            this.count--
        },
        InputCount(value) {
            this.count = value
        }
    }
}
</script>