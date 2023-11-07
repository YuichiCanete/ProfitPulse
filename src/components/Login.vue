<script setup>
    import InputText from 'primevue/inputtext';
    import Button from 'primevue/button';
    import test from '../App.vue'
    
    console.log(test)

</script>


<template>
    
    <div class="container">
        <div class="titleContainer">
            <h1>Profit Pulse</h1>
            <p>Simplify and <br>
            Accelerate Your <br>
            Business Management</p>
        </div>

        <div class="loginContainer">
            <InputText type="text" v-model="value" placeholder="Username" class="inputText"/> <br>
            <InputText type="password" v-model="value" placeholder="Password" class="inputText"/> <br>
            <Button label="Login" class="button"/>

            <Button label="Signup" class="button" />
        </div>
    </div>

    

    
</template>

<style scoped>

    .container {
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 20vh;
    }

    .titleContainer {
        flex: 2;
        margin: 25px;
        margin-left: 200px;
        font-size: 35px;
    }

    .loginContainer {
        flex: 1;
        background-color: rgb(255, 255, 255,.5);
        padding: 25px;
        border-radius: 15px;
        margin: 50px;
        margin-right: 200px;
    }
    
    .button , .inputText{
        margin: 5px;
    }

</style>

