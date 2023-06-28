<template>
 <!-- <h1 class="panel">The Admin Panel</h1>
    <hr>
    section for addig new plants 
    <h2 class="pl">Add Plant</h2>
    <form id="addPlantForm">
        <input type="text" id="plantName" placeholder="Enter the Plant Name" required>
        <input type="text" id="plantImage" placeholder="enter the Image URL" required>
        <input type="number" id="plantPrice" placeholder="Enter the price please" required>
        <button type="submit">Add Plant</button>
    </form>

    display plants 
    <h2>Plants</h2>
    <ul id="plantList"></ul> -->

    <div>
        <ul id="plantList">
            <li v-for="plant in plants" :key="plant.id">
            <table>
                <td>
                    <img :src="plant.image" :alt="plant.name" width="100">
                    <div>{{ plant.name }}</div>
                    <div>{{ plant.price }}</div>
                </td>
            </table>
            <button class="editButton" @click="editPlant(plant.id)">Edit</button>
            <button class="deleteButton" @click="deletePlanta(plant.id)">Delete</button>
            </li>
        </ul>
        <form id="addPlantForm" @submit.prevent="addPlant">
            <input type="text" id="plantName" v-model="newPlant.name" placeholder="Enter the name of the plant">
            <input type="text" id="plantImage" v-model="newPlant.image" placeholder="Enter the Image URL">
            <input type="number" id="plantPrice" v-model="newPlant.price" placeholder="Enter the price">
            <button type="sumbit">Submit</button>

        </form>
    </div>
</template>

<script>
export default {
    data () {
        return {
            plants: [],
            newPlant:{
                id: null,
                name: '',
                price: '',
                image: '',

            }
        }
    },
    mounted() {
        const storedPlants = localStorage.getItem('plants');
        if (storedPlants) {
            this.plants = JSON.parse(storedPlants);
        }
        else {
            this.plants = ['']
        }
    },
    methods: {
        renderPlantsLists() {
            localStorage.setItem('plants', JSON.stringify(this.plants));

        },
    },
    addPlant() {
        if (this.newPlant.name && this.newPlant.image && this.newPlant.price) {
            const newPlantId = this.plants.length + 1;
            const newPlant = {
                id: newPlantId,
                name: this.newPlant.name,
                image: this.newPlant.image,
                price: parseInt(this.newPlant.price),

            };
            this.plants.push(newPlant);
            this.renderPlantsLists();

            this.newPlant.name = '',
            this.newPlant.price = null;
            this.newPlant.image = ''

        }
    },
    deletePlant(plantId) {
        this.plants = this.plants.filter((plant) => plant.id != plantId);
        this.renderPlantsLists();
    },
    editPlant(plantId) {
        const plant = this.plants.find((plant) => plant.id === plantId);
        if (plant) {
        // Edit plant with ID
        console.log(`Edit plant with ID: ${plant.name}`);
      }
    },
    created() {
    this.renderPlantList();
  },
}
</script>


<style>
    
</style>