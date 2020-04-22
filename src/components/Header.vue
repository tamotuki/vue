<template>
<div class="home">
   <header>
   <div class="flex between">
      <h1 class="header-logo">estra inc.</h1>
       <nav class="header-nav">
          <ul>
              <li><a v-on:click="clickHome()">home</a></li>
             <li><a v-on:click="clickAbout()">about</a></li>
               <li><a @click="clickService()">service</a></li>
               <li><a @click="clickWorks()">works</a></li>
               <li><a @click="clickPrice()">price</a></li>
               <li><a @click="clickContact()">contact</a></li>
           </ul>
       </nav>
   </div>
   

    <div id="hamburger">
        <span></span>
        <span></span>
        <span></span>
    </div>
</header>

</div>
</template>

<script>
export default{
    methods: {
        clickHome() {
            alert('homeページに行きます')
            this.$router.push('/')
        },
        clickAbout() {
            alert('aboutページに行きます')
            this.$router.push('/About')
        },
           
        clickService() {
            alert('serviceページへいきます')
            this.$router.push('/Service')
             },
        clickWorks() {
            alert('workページへいきます')
            this.$router.push('/')
            },
        clickPrice() {
            alert('priceページへいきます')
            this.$router.push('/')
            },
         clickContact() {
        alert('contactページへいきます')
        this.$router.push('/Contact')
         } }
 }




 
  </script>
<style scoped>
 header {
   height: 70px;
   background: #000;
 }
 .header-logo {
   font-size: 20px;
   font-weight: bold;
   margin-left: 35px;
   color: #fff;
   line-height: 70px;
 }
 .header-nav li {
   display: inline-block;
   margin-right: 35px;
   font-size: 16px;
 }
 .header-nav a {
   color: #fff;  
 }
 @media screen and (max-width:760px) {
   .header-nav {
     display: none;
   }
   #hamburger {
     width: 40px;
     height: 40px;
     position: absolute;
     cursor: pointer;
     z-index: 100;
     top: 15px;
     right: 20px;
     transition: .4s;
   }
   #hamburger span {
     position: absolute;
     left: 2px;
     display: block;
     width: 35px;
     height: 2px;
     background-color: #fff;
     transition: .8s;
   }
   #hamburger span:nth-of-type(1) {
       top: 10px;
   }
   #hamburger span:nth-of-type(2) {
       top: 20px;
   }
   #hamburger span:nth-of-type(3) {
       top: 30px;
   }
 }

</style>
