<template>
    <div class="root">
        <label>
            Введите email:
            <input 
                type="email" 
                :value="email" 
                @input="emailInput($event.target.value)"
            />
        </label>
        <label>
            Введите пароль:
            <input type="password" :value="password" />
        </label>
    </div>
</template>

<script>
export default {
    name: 'MyComponent',
    data()  {
        return {
            email: 'example@mail.ru',
            password: '12345678'
        }
    }, 
    methods: {
        emailInput(value) {
            this.data = value
        }
    }
}

</script>