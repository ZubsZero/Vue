<template>
    <div class="container">
        <div class="wrapper">
            <form action="post">
                <label for="text">Your Full Name:</label><br><br>
                <input type="text" v-model="Name"><br><br>
                <span>Your Name is {{ Name }} and you {{ choose }} and your phone number is {{ phoneNumber }} and you would like to purchase the following {{ items }}</span><br><br>
                <h4>Your Gender:</h4>
                <label for="Male">Male</label><input type="radio" v-model="choose" value="Male" id="Male">
                <label for="Female">Female</label><input type="radio" v-model="choose" value="Female" id="Male">
                <label for="Prefer not to say">Prefer not to say</label><input type="radio" v-model="choose" value="prefer not to say" id="Prefer not to say"><br><br>
                <label for="number">Full number</label><br><br>
                <input type="text" v-model="phoneNumber">
                <h4>Items you want to purchase</h4>
                <select name="items" id="items" multiple v-model="items" class="items">
                    <option value="Playstation 5">Playstation 5</option>
                    <option value="Call of Duty">Call of Duty</option>
                    <option value="Grand Theft Auto V">Grand Theft Auto V</option>
                    <option value="Spider-man 2">Spider-man 2</option>
                    <option value="Xbox Series X">Xbox Series X</option>
                    <option value="Forza">Forza</option>
                    <option value="Fifa 24">Fifa 24</option>
                    <option value="Ghost Of tsushima">Ghost Of tsushima</option>
                    <option value="Minecraft">Minecraft</option>
                    <option value="Fifa 23">Fifa 23</option>
                </select>





            </form>
        </div>
    </div>
</template>
<script>
 export default {
    data() {
        return{
            Name: '',
            choose:'',
            phoneNumber:'',
            items:'',
            
        }
    }
 }
</script>
<style>
 .container {
    margin-top: 30px;
    display: grid;
    place-items: center;
 }

 .wrapper {
    background-color: black;
    width: 24rem;
    height: 35rem;
    border-radius: 2rem;
 }

 form {
    margin: 30px;
 }

 label {
    color: white;
 }

 span, h4{
    color: white;
 }

 .items {
    width: 13rem;
    background-color: black ;
    color: white;
 }
 option:hover {
    background-color: white;
    color:black
 }
</style>