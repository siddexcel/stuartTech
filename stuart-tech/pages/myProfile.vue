<template>
    <div>
        <div class="flex items-center justify-between p-2">
            <img class="size-6" src="../assets/images/menu.png"/>
            <h1 class="text-2xl text-white">My Profile</h1>
            <img class="size-12" src="../assets/images/avatar.png">
        </div>

        <div class="flex items-center justify-between p-2 text-white mt-5 px-4">
            <h1 class="text-2xl">John Doe</h1>
            <p class="text-sm">edit</p>
        </div>

        <div>
            <a class="underline px-5 block mt-2 text-white" href="mailto:">John_Doe@gmail.com</a>
        </div>

        <div class="w-full px-4 pb-9 flex flex-col"">
            <h1 class=" mt-8  text-white">Change Password:</h1>
            <Input class="w-full mt-5 mb-4" placeholder="Old Password" type="password" v-model="oldPassword" />
            <Input class="w-full mb-4" placeholder="Password" type="password" v-model="password" />
            <Input class="w-full mb-4" placeholder="Confirm Password" type="password" v-model="confirmPassword" />
        <Button class="mt-3">
        Change Password
       </Button>
       </div>
    </div>
    
</template>

<script setup>
import { ref } from 'vue';
import Button from '../components/button.vue'
import Input from '../components/input.vue'

const password = ref('')
const oldPassword = ref('')
const confirmPassword = ref('')
</script>