<template>
   <footer class="footer">
          <div class="container">
             <div class="footer-box">
                 <a href="index.html"  class="footer-logo logo">
                     <img src="../assets/images/logo.png" alt="logo">
                 </a>
                 <div class="footer-nav">
                    <ul>
                        <li>Ресторанам</li>
                        <li>Курьерам</li>
                        <li>Пресс-центр</li>
                        <li>Контакты</li>
                    </ul>
                 </div>
                 <div class="footer-social">
                    <img src="../assets/images/socials/Inst.png" alt="INST"/>
                    <img src="../assets/images/socials/FB.png" alt="FB"/>
                    <img src="../assets/images/socials/VK.png" alt="VK"/>
                 </div>
     
             </div>
          </div>
         </footer>
</template>

<script>
export default {

}
</script>

<style scoped>
.footer {
  display: flex;
  align-items: center;
  min-height: 156px;
  padding: 60px 0;
}
.footer-box {
  height: 100%;
  display: flex; 
  align-items: center;
  justify-content: space-between;
  gap: 36px;
  flex-wrap: wrap;
}
.footer-nav {
  flex-grow: 1;

}
.footer-nav ul {
display: flex;
align-items: center;
list-style: none;
padding: 0;
margin: 0;
gap:15px;
flex-wrap: wrap;
}
.footer-nav ul li {
font-weight: 400;
font-size: 18px;
color: #595959;
}
.footer-social {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 20px;
}
</style>