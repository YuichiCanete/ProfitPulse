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

            <h1>History</h1>

            <div class="inventoryContainer">
                
                <fieldset class="itemHistory">
                    <legend>10/27/2023</legend>
                    <div class="item">
                        <p style="width: 75%;">Large Fries</p>
                        <p style="width: 15%;">Quantity: 1</p>
                        <p style="width: 10%;">Price: P200</p>
                    </div>

                    <div class="item">
                        <p style="width: 75%;">Borgerr</p>
                        <p style="width: 15%;">Quantity: 2</p>
                        <p style="width: 10%;">Price: P75</p>
                    </div>

                    <p style="text-align: right; margin-right: 15px; font-size: 25px;">Total Fee: P350</p>

                </fieldset>
                
                

            </div>

            

            
        </div>

        

    </div>
    
</template>

<style scoped>

    .itemHistory {
        border: none;
        border-top: 2px solid #151515;
        border-bottom: 2px solid #151515;
    }

    legend {
        color: #003B89;
        font-size: 25px;
    }

    .item{
        background-color: rgb(255,255,255,.5);
        display: flex;
        margin: 15px;
        padding: 10px;
    }

    .inventoryContainer {
        color: #151515;
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

