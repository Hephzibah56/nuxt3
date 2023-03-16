<template>
    <div>
    <header class= "shadow-sm bg-white">
        <nav class="container mx-auto p-4 flex justify-between">
            <NuxtLink to="/" class="font-bold">PasswordChecker</NuxtLink>
            <ul class="flex gap-4">
                <li><NuxtLink to="/"> Home </NuxtLink></li>
                <li><NuxtLink to="/about"> About </NuxtLink></li>
                <li><NuxtLink to="/products" class="btn"> Products </NuxtLink></li>
                <li><NuxtLink to="/products/abc" class="btn"> Abc Products </NuxtLink></li>

            </ul>
            
            <!-- <a href ="/about">normal link--about page</a> -->
        </nav>
    </header>
        
    <!-- Output the page content -->
    <div class="container mx-auto p-4">
        <slot />   
        <!-- to show where pages content will come -->
    </div>
    </div>
</template>


<style scoped>
.router-link-exact-active {
    color:  #12b488
}
</style>
