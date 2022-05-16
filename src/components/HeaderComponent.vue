<template>
<header class="container">
    <div class="heder-top ">
        <div class="logo">
<img src="../assets/img/dark-pet-logo.png" alt="">
        </div>
        <div class="serchbar">
            <input type="text" placeholder="Search...">
        </div>
        <div class="questions">
            <h4>Questions?</h4>
            <p>Call us : 1.800.123.4567</p>
        </div>
        <div class="profile">
<i class="fa-solid fa-bag-shopping"></i>
<i class="fa-solid fa-user"></i>
        </div>
    </div>
    <nav class="debug">
        <div v-for="(name, index) in navOptions" :key="index" >
           <div class="navoptions" >{{navOptions[1].name}}
              <div v-if="navOptions.options"> {{navOptions.options}}</div>
           </div>

        </div>
    </nav>
</header>
</template>

<script>
export default {
    name:'HeaderComponent',
    data(){ return{
        navOptions:[
            {
                id: 1,
                name: 'Home',
                optins:['Home-Alternate']
            },
            {
                 id: 2,
                name: 'Shop',
                optins:['Shop no sidebar', 'Shop single sidebar','Shop dual sidebar','Simple product','Variable product']
            },
            {
                 id: 3,
                name:'About'
            },
             {
                  id: 4,
                name:'Blog'
            },
             {
                  id: 5,
                name:'Contact'
            },
             {
                  id: 6,
                name:'Shop by brand',
                // options:[]
            }
        ]
}
}
}

</script>

<style lang="scss">
.heder-top{
    height: 50px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    border: 1px solid black;
}
.logo img{
    height: 30px;
}
.serchbar input{
    background-color:lightgray;
    padding: 4px;
    border: 1px solid lightgray;
    border-radius:30px;
    width: 200px;
}
.questions{
    display: flex;
}
.questions p{
    color: gray;
}
.profile i{
    margin-left: 10px;
    
}
nav{
    height: 50px;
    display: flex;
    justify-content: center;
}
.navoptions{
    margin: 14px;
}

</style>