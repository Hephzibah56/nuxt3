<!-- <template>
    <div>
        <header>
        <nav>
            <NuxtLink to="/">PasswordChecker</NuxtLink>
            <ul>
                <li><NuxtLink to="/"> Home </NuxtLink></li>
                <li><NuxtLink to="/about"> About </NuxtLink></li>
                <li><NuxtLink to="/products"> Products </NuxtLink></li>
            </ul>
        </nav>
    </header> 
        <h2> About </h2>
        <p> Hephzibah is coding in Nuxtjs 3.0. About page</p>
        <div>{{ data }}</div>
    </div>
</template>

<script setup>
const  { data } =await useFetch(`/api/ninja`)

</script>

<style scoped>
h2{
    margin-bottom: 20px;
    font-size: 36px;
}

p{
    margin: 20px 0;
    
}
</style> -->


<template>
    <div>
      <h2>About</h2>
      <p>Hephzibah's Trial and call to API's</p>
      <p>Api response:</p>
      <div>{{ data }}</div>
    </div>
  </template>
  
  <style scoped>
    h2 {
      margin-bottom: 20px;
      font-size: 36px;
    }
    p {
      margin: 20px 0;
    }
  </style>
  
  <script setup>
    // const { data } = await useFetch('/api/ninja?name=mario')
    // const { data } = await useFetch('/api/ninja?name=mario', {
    //   method: 'post',
    //   body: {age: 30}
    // })
  
    const { data } = await useFetch('/api/currency/NGN')
  </script>