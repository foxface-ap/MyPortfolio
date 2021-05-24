<template>

<div id="Navbar">
   <section id="sec-1">
 
    <div id="tex" class="container" style="margin-top:50px">
  
      <div style="background-color:#006182; border-radius: 15px;" class="row">
        
          <Face/>

          <div class="col-md-6">
            <div class="description">
                    // display on-boarding message<br>
                    console.log("Hi there, I'm self-taught web developer from 
                    <span style="color: #FF9933;text-shadow: 0 0 3px #ade7fa;">I</span>
                    <span style="color: #FF9933;text-shadow: 0 0 3px #ade7fa;">N</span>
                    <span style="color: #fff;text-shadow: 0 0 3px #ade7fa;">D</span>
                    <span style="font-weight: 700;color: #138808;text-shadow: 0 0 3px #ade7fa;">I</span>
                    <span style="font-weight: 800;color: #138808;text-shadow: 0 0 3px #ade7fa;">A</span>
                    👋");
                    <hr>
                  {<br>
                    &nbsp; 1 &nbsp; class Person {<br>
                    &nbsp; 2 &nbsp;&nbsp;&nbsp;     constructor() {<br>
                    &nbsp; 3 &nbsp;&nbsp;&nbsp;&nbsp;       this.name = "Anuj Patel";<br>
                    &nbsp; 4 &nbsp;&nbsp;&nbsp;&nbsp;       this.property = ["DEV", "DESIGN"];<br>
                    &nbsp; 5 &nbsp;&nbsp;&nbsp;&nbsp;       this.age = new Date().getFullYear() - 2000;<br>
                    &nbsp; 6 &nbsp;&nbsp;&nbsp;&nbsp;     }<br>
                    &nbsp; 7  &nbsp;}<br>
                  }<br>
                  <br>
                    // create an object<br>
                    const person = new Person();<br>
                     <button class="btn bt"><a href="src\assets\Anuj's Resume.pdf" download><i class="fa fa-download"></i> Resume</a></button>
                </div>
        </div>
      </div>
    </div>

  
    
  </section>
  <section id="sec-2">
      <About/>
  </section>
</div>
</template>

<script>
import About from "./About.vue";
import Face from "./Face.vue";
export default {
  name: "app",
  components: {
    About,
    Face
  }
};
</script>

<style scopped>

.bt{
  border-radius: 36px; 
  float:right;
  transform: translate(-40px,-40px);
}

@media only screen and (max-width: 560px) {
    .bt{
    border-radius: 36px; 
    float: none;
    left: 50%;
    transform: none;
    margin-top:10px
  }
}
.bt a{
  border-radius: 60%;
  text-decoration: none;
  color: #0a2e3a;
}
.bt:hover{
  border-radius: 36px;
  background-color:#001b24;
}
.bt a:hover{
  border-radius: 60%;
  color: #dbf5fd;
  text-decoration: none;
}

.description{
  width: auto;
  height: auto;
  margin: 0 auto;
  padding: 15px;
  position: relative;
   font-size: 2.3rem;
  color: #dbf5fd;
}

@media only screen and (max-width: 1000px) {
    .description{
    font-size: 1.8rem;
    color: #dbf5fd;
  }
}


.container{
  border-radius: 15px;
}

#tex
{
  background-color:#006182;
  background: transparent;

}

html {
  scroll-behavior: smooth;
}
section {
  min-height: 100vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.scroll-down {
  height: 50px;
  width: 30px;
  border: 2px solid black;
  position: absolute;
  bottom: 20px;
  border-radius: 50px;
  cursor: pointer;
  left: 48.43%;
}
.scroll-down::before,
.scroll-down::after {
  content: "";
  position: absolute;
  top: 20%;
  left: 50%;
  height: 12px;
  width: 12px;
  transform: translate(-50%, -100%) rotate(45deg);
  border: 2px solid black;
  border-top: transparent;
  border-left: transparent;
  animation: scroll-down 1s ease-in-out infinite;
}
.scroll-down::before {
  top: 30%;
  animation-delay: 0.6s;
  animation: scroll-down 1.2s ease-in-out infinite; 
}

@keyframes scroll-down {
  0% {
    /* top:20%; */
    opacity: 0;
  }
  30% {
    opacity: 1;
  }
  60% {
    opacity: 1;
  }
  100% {
    top: 90%;
    opacity: 0;
  }
}

</style>

