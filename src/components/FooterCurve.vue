<template>
 <div>
  <footer>
    <div id="container">
      <div id="contacts">
        <p>{{mail}}</p>
        <p>{{phone}}</p>
      </div>       
      <div id="mentions">
        <p>{{mention}}</p>
      </div>
    </div>
  </footer>
 </div>
</template>

<script>
export default {
  data(){
    return{
      mail:'ossiekcjohnson@gmail.com❤❤❤',
      phone: '088 566 4781',
      mention: '2022 | Copyright😒🤷‍♂️'
    }
  }

};
</script>

<style>
footer {
  display: flex;

  margin: auto;
  padding: 10 0px;
  /* background-color:#666;
  height: 15vh;
  justify-content: center;
  align-items: flex-end;
  font-family: Open Sans; */
}

#container {
  padding-top: 20px;
  margin-top: 20px;
  width: 100vw;
  color: #222;
  background-color:  rgb(129, 120, 120);
  display:flex;
  flex-direction: column;
  align-items: center;
}

#contacts{
  display: flex;
  justify-content: space-around;
  align-items: center;
  width: 100%;
  color: #222;
   text-shadow:
      0 0 7px #fff,
      0 0 10px #fff,
      0 0 21px #fff,
      0 0 42px rgb(255, 23, 240),
      0 0 82px rgb(238, 0, 255),
      0 0 92px rgb(255, 0, 140),
      0 0 102px rgb(255, 0, 153),
      0 0 151px #0fa;
}
#socials {
  text-align: right;
}

#social div{
  height: 30px;
  width: 30px;
  background-color: white;
  border-radius: 50%;
}

#mentions p {
  font-size: 1em;
  padding-bottom: 10px;
   text-shadow:
      0 0 7px #fff,
      0 0 10px #fff,
      0 0 21px #fff,
      0 0 42px rgb(255, 23, 240),
      0 0 82px rgb(238, 0, 255),
      0 0 92px rgb(255, 0, 140),
      0 0 102px rgb(255, 0, 153),
      0 0 151px #0fa;
}

</style>