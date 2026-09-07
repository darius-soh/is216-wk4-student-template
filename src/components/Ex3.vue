<script setup>
    import { ref } from 'vue'

    // Add code here
    const choice = ref('username')

    
</script>
<template>
        <h1>Please select your login option</h1>
        <!-- Add/modify code in the following to have a dropdown list 
            which lets the user to select either to login with username or email -->
        <select v-model="choice">
            <option value="username">Username login</option>
            <option value="email">Email login</option>
        </select>
        
        <div v-if="choice === 'username'">
            <label>Username</label>
            <input placeholder="Enter your username">
        </div>

        <div v-else>
            <label>Email</label>
            <input placeholder="Enter your email">
        </div>
</template>

