<template>
    <div class="flex min-h-screen text-gray-700 bg-custom-bg">

        <!-- MAIN CONTAINER -->
        <div class="container m-auto w-5/6 shadow-2xl bg-white rounded-2xl overflow-auto h-[90vh]">
            <!-- HEADER -->
            <header class="px-5 py-3 sm:py-2 flex flex-col sm:flex-row items-center justify-between rounded-t-2xl">
                <!-- Logo -->
                <div class="flex items-center space-x-2">
                    <img id="logoImg" class="w-16" src="assets/img/illustration.png" alt="Logo Image">
                    <h2 id="logoTitle" class="text-2xl font-bold text-indigo-700">Welcome</h2>
                </div>
                <!-- Navbar -->
                <nav class="text-md space-x-6">
                    <NuxtLink to="/" class="px-3 py-1 text-md">Home</NuxtLink>
                    <button @click="doLogin" class="px-6 py-2 text-md rounded-md bg-blue-700 hover:bg-blue-900 text-white ">Login</button>
                </nav>
            </header>

            <!-- CONTENT -->
            <main class="grid md:grid-cols-2 gap-5 items-center p-5 bg-blue-50">
                <!-- Left Content -->
                <div class="flex flex-col space-y-4 p-4 m-2 sm:p-8 border-2 bg-blue-200 bg-opacity-70 shadow-xl rounded-lg">
                    <h1 class="text-3xl font-semibold text-indigo-600">Welcome to Our Landing Page</h1>
                    <h3 id="promptLogin" class="text-lg">Please login to access other features</h3>
                    
                    <p id="failedLoginMessage" class="hidden text-md text-red-800 p-5 border-2 border-red-700 bg-red-300 bg-opacity-30"><b>Error!</b> The username/password you input is wrong. Please try again.</p>

                    <form id="loginForm" class="grid space-y-3" @submit.prevent="authAdmin" novalidate>             
                        <label for="usernameInput" class="block"><span class="dark:text-white">Username</span></label>
                        <input id="usernameInput" type="text" class="form-input mt-1 block border-0 rounded-md" placeholder="Please enter your username">
                        <p id="invalidUsername" class="hidden text-red-500 text-sm">Username must not be empty.</p>

                        <label for="passwordInput" class="block"><span class="dark:text-white">Password</span></label>
                        <input id="passwordInput" type="password" class="form-input mt-1 block border-0 rounded-md" placeholder="Please enter your password">
                        <p id="invalidPassword" class="hidden text-red-500 text-sm">Password must not be empty.</p>
                        <p id="capslockWarning" class="hidden text-yellow-500 text-sm">WARNING! Caps Lock is ON</p>
                        
                        <div class="flex gap-2 items-center">
                            <input id="showPassword" type="checkbox" class="form-checkbox text-indigo-600 block border-0" placeholder="Enter your username">
                            <label class="block">Show Password</label>
                        </div>
                        <button @click="authAdmin" type="submit" class="bg-indigo-600 hover:bg-indigo-800 px-4 py-3 rounded-md text-gray-100 tracking-widest">LOGIN</button>
                    </form>
                </div>

                <!-- Right Content -->
                <div class="flex flex-col items-center justify-center">
                    <img id="loginImg" class="w-[70%]" src="assets/img/illustration.png" alt="Illustration Image">
                    <blockquote class="text-md text-gray-600 relative">
                        <svg class="w-4 h-4 text-gray-400 dark:text-gray-600 mb-4" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 18 14">
                            <path d="M6 0H2a2 2 0 0 0-2 2v4a2 2 0 0 0 2 2h4v1a3 3 0 0 1-3 3H2a1 1 0 0 0 0 2h1a5.006 5.006 0 0 0 5-5V2a2 2 0 0 0-2-2Zm10 0h-4a2 2 0 0 0-2 2v4a2 2 0 0 0 2 2h4v1a3 3 0 0 1-3 3h-1a1 1 0 0 0 0 2h1a5.006 5.006 0 0 0 5-5V2a2 2 0 0 0-2-2Z"/>
                        </svg>
                        <p class="font-bold italic">The only limit to our realization of tomorrow will be our doubts of today.</p>
                        <p>&#8212; Franklin D. Roosevelt</p>         
                    </blockquote>
                </div>
            </main>

            <!-- Footer -->
            <footer class="p-3 bg-white rounded-b-3xl">
                <p class="text-xs text-center tracking-widest">&copy; 2023 BTJ Academy </p>
            </footer>

        </div>

    </div>
</template>

<script>
export default {
    methods: {
        authAdmin() {
            navigateTo('/dashboard').catch(err => {
                console.error('Error navigating to /dashboard:', err)
            });
            alert('Redirecting to Admin Dashboard Page')
        }
    }
}
</script>