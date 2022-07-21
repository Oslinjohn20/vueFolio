<template>
  <div class="about">
    <div class="cardTop">
     <svg width="497" height="219" viewBox="0 0 497 219" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path fill-rule="evenodd" clip-rule="evenodd" d="M-38.5 196C-38.5 196 34 91 133.5 91C233 91 427 159 532.5 30C638 -99 518 236 518 236L-49 246.5L-38.5 196Z" fill="#FF768E" />
      </svg>
    </div>
    <div class="body">

     <div class="timeline">
      <h3>
        Education
      </h3>
      <label ></label>
      <div class="box">
        <div class="container">
          <div class="lines">
            <div class="dot"></div>
            <div class="line"></div>
            <div class="dot"></div>
            <div class="line"></div>
            <div class="dot"></div>
            <div class="line"></div>
          </div>

          <div class="card">
            <div class="card">
              <h4>2006-2010</h4>
            <p>I attended Elsies River <br> Senior Secondary</p>
            </div>
            <div class="card-mid">
               <h4>2012-2013</h4>
            <p>I furthered my studies at NorthLink college Bellville campus studying motor mechanics</p>
            </div>
            <div class="card">
                 <h4>2013-2017</h4>
            <p>Furthered my studies at Imperial Technical Training Academy</p>
            </div>
          </div>
        </div>
        <div class="bottom">
          <a :href="'../../public/files/oslin johnson cv.pdf'" download>download</a>
        </div>
      </div>
     </div>
     </div>
  
  
  </div>
 
</template>

<script>
export default {
 
}
</script>

<style scoped>
*{
  /* margin: 0;
  padding: 0; */
  outline: none;
  text-decoration: none;
  list-style: none;
  font-family: "Mulish", sans-serif;
}
.about{
  min-height: 100vh;
 
}
.body {
  display: flex;
  padding-top: 50px;
  justify-content: center;

  transform: scale(0.8) translateY(-250px) translateX(-20px);
}
.cardTop {
  width: 400px;
  height: 284px;
  background: #fac24f;
  border-radius: 20px;
  display: flex;
  overflow: hidden;
  align-items: flex-end;
  transform: translate3d(580px, 50px, 10px);
}
.timeline {
  width: 355px;
  height: 696px;
  background: #ecf1f524;
  mix-blend-mode: normal;
  backdrop-filter: blur(5px);

  overflow: hidden;

  position: absolute;
  top: 144px;
  margin-left: 71px;
  box-shadow: 0px 20px 53px -30px rgba(95, 102, 173, 0.566816);
  border-radius: 10px;
}
.timeline h3 {
  font-family: Open Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 30px;
  color: #ffffff;

  margin-top: 40px;
}

.timeline label{
  font-family: Open Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 22px;
  /* identical to box height */
  margin-left: 66px;
  margin-top: 10px;
  color: #ffffff;
}
.box {
    width: 100%;
    height: 509px;
    background: #fbfcfd;
    margin-top: 99.5px;
}
.container{
  width: 100%;
  height: 357px;
  display: flex;
}
.lines{
  margin-left: 40px;
}
.dot{  width: 14px;
  height: 14px;
  background: #d1d6e6;
  border-radius: 7px;
}

.line {
  height: 103px;
  width: 2px;
  background: #d1d6e6;
  margin-left: 5.3px;
}

.cards {
  margin-left: 12px;
  transform: translateY(-50px);
  width: 249px;
  height: 93px;
  padding-top: 25px;
  background: #ffffff;
  box-shadow: 0 2px 2px 0 #eeeeee40;
  border-radius: 10px;
  box-shadow: 0px 16px 15px -10px rgba(105, 96, 215, 0.0944602);
  margin-bottom: 10px;      
}
.card {
  margin-left: 12px;
  transform: translateY(-50px);
  width: 249px;
  height: 93px;
  padding-top: 25px;
  background: #ffffff;
  box-shadow: 0 2px 2px 0 #eeeeee40;
  border-radius: 10px;
  box-shadow: 0px 16px 15px -10px rgba(105, 96, 215, 0.0944602);
  margin-bottom: 10px;
}
.card-mid {
  margin-left: 12px;
  transform: translateY(-50px);
  width: 249px;
  height: 120px;
  padding-top: 25px;
  background: #ffffff;
  box-shadow: 0 2px 2px 0 #eeeeee40;
  border-radius: 10px;
  box-shadow: 0px 16px 15px -10px rgba(105, 96, 215, 0.0944602);
  margin-bottom: 10px;
}
h4 {
  font-family: Open Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 19px;
  margin-left: 25px;
  margin-bottom: 5px;
  color: #2b2862;
}
p {
  font-family: Open Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 22px;
  color: #2b2862;
  margin-left: 25px;
}
.bottom {
  width: 100%;
  height: 107px;
  background: #fff;
  box-shadow: 0 0 2px #eeeeee50;
  padding-top: 45px;
}
.btn {
  width: 249px;
  height: 62px;
  background: #ffffff40;
  mix-blend-mode: normal;
  cursor: pointer;
  border: 1px solid #8260d780;
  border-radius: 5px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: Open Sans;
 font-style: normal;
 font-weight: bold;
  font-size: 14px;
 line-height: 19px;
 color: #2b2862;
 margin-left: 53px;
  transition: 0.3s;
  background: #2b2862;
  color: #fff;
  border-color: #2b2862;
}
.btn :hover{
  transform: scale(1.03);
}
</style>
