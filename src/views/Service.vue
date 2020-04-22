
  <template>
  <div id="business">
  <h2 class="section-title">service</h2>
  <div class="flex around business-wrap">
    <div class="business-cat" v-for="service in services" :key="service.id">
      <img src="../assets/img/business-icon.png" alt="">
      <h3>{{service.bis}}</h3>
      <p>{{service.content}}</p>
    </div>
    <div class="business-cat" v-for="service in services" :key="service.id">
      <img src="../assets/img/business-icon.png" alt="">
      <h3>{{service.bis}}</h3>
      <p>{{service.content}}</p>
    </div>
    <div class="business-cat" v-for="service in services" :key="service.id">
      <img src="../assets/img/business-icon.png" alt="">
      <h3>{{service.bis}}</h3>
      <p>{{service.content}}</p>
    </div>
    
  </div>
</div>
</template>
<script>
export default{
    data() {
        return{
            service: [
    {bis: 'ビジネスA', content: 'ビジネスの説明が入ります。ビジネスの説明が入ります。ビジネスの説明が入ります。ビジネスの説明が入ります。'},
    {bis: 'ビジネスB', content: 'ビジネスの説明が入ります。ビジネスの説明が入ります。ビジネスの説明が入ります。ビジネスの説明が入ります。'},
    {bis: 'ビジネスC', content: 'ビジネスの説明が入ります。ビジネスの説明が入ります。ビジネスの説明が入ります。ビジネスの説明が入ります。'}
]
            
        }    
        }
}
</script>
<style scoped>
 #business{
 background: url(../assets/img/bg3.jpg);
 background-size: cover;
}
#business .section-title {
 color: #fff;
 padding: 40px 0;
 margin: 0;
}
.business-wrap {
 text-align: center;
}
.business-cat {
 width: 28%;
 background-color: rgba(51, 51, 51, 0.5);
 padding: 20px 35px 30px;
 box-sizing: border-box;
 margin-bottom: 50px;
}

.business-cat h3 {
 font-size: 18px;
 font-weight: bold;
 margin-bottom: 10px;
 color: #fff;
}
.business-cat p {
 color: #fff;
}
.business-cat img {
 width: 100px;
 height: auto;
 margin: 0 auto 10px;
}
@media screen and (max-width:760){
    .business-cat {
        width: 80%;
    }
}

</style>