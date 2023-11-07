<script setup>
    import SideBar from './sideBar.vue'
    import InputText from 'primevue/inputtext';
    import Button from 'primevue/button';
</script>

<template>

    <div class="container">

        <div class="left">
            <SideBar/>
        </div>

        <div class="center">
            <h1>Add Product</h1>
            <div class="addContainer">

                <div class="fields">
                    <img src="https://static.thenounproject.com/png/212328-200.png" alt="img">
                    <InputText type="text" v-model="value" placeholder="Product Name" class="inputText"/> <br>
                    <InputText type="text" v-model="value" placeholder="Price" class="inputText"/> <br>
                    <InputText type="text" v-model="value" placeholder="Quantity" class="inputText"/> <br>
                </div>

                <div class="buttons" style="margin-top: 95px;">
                    <Button label="Cancel" style="margin-right: 15px;"></Button>
                    <Button label="Add"></Button>
                </div>

            </div>

            

        </div>


        

    </div>
    
</template>

<style scoped>

    .buttons {
        float: right;
    }


    .container {
        display: flex;
    }

    .center {
        width: 100%;
        margin: 15px;
    }
    .addContainer {
        color: #151515;
        background-color: rgb(255,255,255,.5);
        padding: 10px;
        height: 75vh;
    }

    .fields {
        height: 75%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }




</style>

