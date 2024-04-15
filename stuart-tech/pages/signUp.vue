<template>
    <div class="w-full px-5 pb-9 min-h-screen flex flex-col  items-center">

        <img src="../assets/images/logo.png" alt="Logo" class="size-40 mt-12" />
        <h1 class="text-2xl text-slate-200 mt-8 mb-16">Sign Up</h1>
        <Input class="w-full mt- mb-4" placeholder="Email" v-model="email" />
        <Input class="w-full mb-4" placeholder="Password" type="password" v-model="password" />
        <Input class="w-full mb-4" placeholder="Confirm Password" type="password" v-model="confirmPassword" />
        <div class="flex items-center mt-2">
            <input type="checkbox" checked class="mr-2 form-checkbox h-4 w-4 text-blue-600 transition duration-150 ease-in-out" id="newsletter-checkbox">
            <label for="newsletter-checkbox" class="text-gray-500 text-sm">I would like to receive your newsletter and other promotional information.</label>
        </div>
        <Button class="mt-8">
            Sign up
        </Button>
        <nuxt-link class="text-sm text-slate-200 mt-4" to="#" >Forget your password?</nuxt-link>
        <nuxt-link class="text-sm text-slate-200 mt-3" to="login">Login</nuxt-link>
    </div>
</template>

<script setup>
import { ref } from 'vue';
import Button from '../components/button.vue'
import Input from '../components/input.vue'

const email = ref('')
const password = ref('')
const confirmPassword = ref('')
</script>