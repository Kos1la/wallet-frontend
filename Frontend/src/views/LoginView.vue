<script lang="ts">
export default {
  data() {
    return {
      email: '',
      password: '',
      rememberMe: false
    }
  },
  methods: {
    login() {}
  }
}
</script>

<template>
  <div class="pt-8 pb-8 flex flex-col justify-center items-center">
    <div class="max-w-md w-full px-4 py-8 rounded-md shadow-md bg-gray-100">
      <label for="email" class="block text-lg font-semibold text-gray-700 mb-2">Login</label>
      <form class="space-y-4" @submit.prevent="login">
        <div>
          <input
            type="email"
            id="email"
            placeholder="Your email"
            class="block w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:border-purple-500"
            v-model="email"
          />
        </div>
        <div>
          <input
            type="password"
            id="password"
            placeholder="Your password"
            class="block w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:border-purple-500"
            v-model="password"
          />
        </div>
        <div class="flex items-center justify-between">
          <label for="remember" class="flex items-center cursor-pointer">
            <input
              type="checkbox"
              id="remember"
              class="mr-2 border-gray-300 rounded focus:ring-purple-500"
              v-model="rememberMe"
            />
            <span class="text-sm text-gray-600">Remember me</span>
          </label>
          <a href="#" class="text-sm text-blue-600 hover:underline">Forgot password?</a>
        </div>
        <button
          type="submit"
          class="block w-full px-4 py-2 bg-purple-500 text-white font-semibold rounded-md shadow-md hover:bg-purple-600 focus:outline-none focus:bg-purple-600"
        >
          Login
        </button>
        <hr class="my-4 border-t border-gray-300" />
        <div class="space-y-2">
          <button
            class="block w-full px-4 py-2 bg-gray-700 text-white font-semibold rounded-md shadow-md hover:bg-gray-800 focus:outline-none focus:bg-gray-800"
          >
            Login with GitHub
          </button>
          <button
            class="block w-full px-4 py-2 bg-red-500 text-white font-semibold rounded-md shadow-md hover:bg-red-600 focus:outline-none focus:bg-red-600"
          >
            Login with Google
          </button>
        </div>
        <div class="text-center">
          <span class="text-gray-600">Don't have an account?</span>
          <RouterLink to="/registration">Registration</RouterLink>
        </div>
      </form>
    </div>
  </div>
</template>
