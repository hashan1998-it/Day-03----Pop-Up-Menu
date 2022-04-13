<template>
    <div class="main">  
        <div class="content">
            <img src="~/static/img/cancel.png" alt="" srcset="" @click="$emit('showPop')">
            <h2>This is the Pop up Menu</h2>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sed, fuga nam repellat quaerat quae, voluptate debitis impedit totam quisquam recusandae, numquam ipsam consectetur amet eius exercitationem officia aliquid facere modi?</p>
        </div>
    </div>
</template>

<style scoped>
.main{
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    overflow: auto;
    background: rgba(0, 0, 0, 0.5);
    z-index: 1;

}
.content{
    width: 80%;
    max-width: 60rem;
    background-color: #eee;
    margin: 15% auto;
    padding: 2rem;
    border: 1px solid #777;
    animation: slide ease 0.8s;
    text-align: center;
    height: 50%;
    transform: translateY(-30%);

}
.content img{
    cursor: pointer;
    width: 32px;
    height: 32px;
    display: flex;
    margin-left: auto;

}
p{
    padding-top: 50px;
}

@keyframes slide{
    from{
        transform: translateY(-70%);
    }
    to{
        transform: translateY(-30%);
    }
}

</style>