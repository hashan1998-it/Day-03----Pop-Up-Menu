<template>
    <div>
        <h1><span>Let's</span> Make a Pop Up Menu</h1>
        <p>This is a simple pop up menu created with Nuxt.js Framework</p>
        <button @click="$emit('showPop')" class="btn btn-primary">Test Popup</button>
    </div>
</template>

<style scoped>
div{
    text-align: center;
    padding: 5px;
}

span{
    font-weight: 700;
}
p{
    font-weight: 300;
    font-size: 1.1rem;
    padding-top: 1.5rem;
}

</style>