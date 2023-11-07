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

            <h1>Inventory</h1>

            <div class="inventoryContainer">

                <div class="item">
                    <p style="width: 75%;">Chicken Manok</p>
                    <p style="width: 15%;">Quantity: 60</p>
                    <p style="width: 10%;">Price: P100</p>
                </div>

                <div class="item">
                    <p style="width: 75%;">Borgerr</p>
                    <p style="width: 15%;">Quantity: 9</p>
                    <p style="width: 10%;">Price: P75</p>
                </div>

                <div class="item">
                    <p style="width: 75%;">Large Fries</p>
                    <p style="width: 15%;">Quantity: 4000</p>
                    <p style="width: 10%;">Price: P200</p>
                </div>
                

            </div>

            <Button label="Add Product" class="addButton"></Button>

            
        </div>

        

    </div>
    
</template>

<style scoped>

    .addButton {
        margin-top: 15px;
        float: right;
    }

    .item{
        background-color: rgb(255,255,255,.5);
        display: flex;
        margin: 15px;
        padding: 10px;
        color: #151515;
    }

    .inventoryContainer {
        background-color: rgb(255,255,255,.5);
        padding: 10px;
        height: 75vh;
        overflow-y: scroll;
    }

    .container {
        display: flex;
    }

    .center {
        width: 100%;
        margin: 15px;
    }



</style>

