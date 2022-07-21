<template>
 <section id="home">
  <h1>My name is <span class="myName">Oslin Johnson</span></h1>
  <h2>I am <span ref="textContainer"></span></h2>
 </section>
</template>

<script>
export default {
  name: "HomeView",
  data() {
    return {
      text: [
        "a JavaScript Victim",
        "Error hunter",
        "styling illiterate"
      ],
    };
  } ,
  methods: {
    waitForMs(ms) {
      return new Promise((resolve) => setTimeout(resolve, ms));
    },
    async typeSentence(sentence, delay = 100) {
      let letters = sentence.split("");
      let i = 0;
      while (i < letters.length) {
        await this.waitForMs(delay);
        this.$refs.textContainer.append(letters[i]);
        i++;
      }
    },
    async deleteSentence() { 
      let sentence = this.$refs.textContainer.innerHTML;
      let letters = sentence.split("");
      while(letters.length > 0) {
        await this.waitForMs(100);
        letters.pop();
        this.$refs.textContainer.innerHTML = letters.join("")
      }
    },
    async sentenceLoop(sentenceList) {
      let i = 0;
      let t = true;
      while (t) {
        await this.typeSentence(sentenceList[i]);
        await this.waitForMs(1500)
        await this.deleteSentence()
        await this.waitForMs(500)
        i++;
        if(i >= sentenceList.length) {
          i = 0;
        }
      }

    },

  },
  async mounted() {
    this.sentenceLoop(this.text)
  },
}
</script>
<style scoped>
#home {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 30px;
}

h1 {
  font-size: 4rem;
}
h2 {
  position: relative;
  
}
h2 span:after{
  content: "";
  width: 3px;
  height: 100%;
  background: #333;
  position: absolute;
  animation: blink 1s infinite;
}
.myName{
 color: #fff;
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
@keyframes blink {
  0%,
  49% {
    background: #333;
  }
  50%,
  100% {
    background: white;
  }
}
</style>
