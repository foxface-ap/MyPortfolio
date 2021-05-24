<template>
  <div class="col-md-6 faceholder">
      <div class="cartoon hb">
      <div class="back-hair r ha hb"></div>
      <div class="ear ha ">
      </div>
       
      <div class="head">
        <div class="forehead ha hb"></div>
        <div class="mole r"></div>
        <div class="eye r ha hb blink"></div>
        <div class="eye r ha hb blink"></div>
        <div class="lip r "></div>
        <div class="mouth"></div>
        <div class="mustache"></div>
        <div class="mustache"></div>
        <div class="nose ha hb"></div>
        <div class="eyebrow squeeze"></div>
        <div class="eyebrow squeeze"></div>
        <div class="earhole1 r"></div>
       <div class="earhole2 r"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  components: { 
  }
}
</script>

<style scopped>

.faceholder
{
  background-image: radial-gradient(circle, #a3e6fc, #7fc3dc, #5ca1bd, #37809f, #006182);
  border-radius: 15px;
  
}

.cartoon {
  transform: translate(-4%, 18%);
  width: 81vmin;
  height: 81vmin;
}
@media only screen and (max-width: 855px) {
  .cartoon {
    transform: translate(0%,18%);
    width: 81vmin;
    height: 81vmin;
  }
}

.cartoon div {
  position: absolute;
  box-sizing: border-box;
}

.b {
  border: 0.5vmin solid;
}

.r {
  border-radius: 100%;
}

.hb::before,
.ha::after {
  content: "";
  display: block;
  position: absolute;
  box-sizing: border-box;
}

/****/
.cartoon {
  --hair: rgb(32, 24, 24);
  --iris: rgb(70, 36, 36);
  --skin: rgb(252, 189, 147);
  --line-face: #da8;

}

.head {
  width: 50%;
  height: 65%;
  background: var(--skin);
  border-radius: 100% / 25% 25% 115% 115%;
  top: 10%;
  left: 50%;
  transform: translate(-50%, 0);
  box-shadow:  -2vmin -7vmin var(--hair), 2vmin -7vmin var(--hair),inset 0px -10px 5px var(--hair);
  
      
}

.mole {
  width: 2.5%;
  height: 2%;
  background: var(--hair);
  left: 70%;
  top: 63%;
  transform: translate(70%, 80%);
}

.eye {
  width: 30%;
  height: 12%;
  background: rgb(243, 227, 227);
  border-radius: 100% / 100%;
  top: 33%;
  left: 9%;
  box-shadow: inset 0 5.2vmin 0 -4vmin rgba(219, 11, 11, 0.1), inset 0 5vmin 0 -4vmin var(--skin), 0 -3vmin 3vmin -1vmin rgba(0,0,0,0.05); 
}

.eye::before {
  width: 2.6vmin;
  height: 2.6vmin;
  background: #222;
  border-radius: 100%;
  top: 56%;
  left: 50%;
  transform: translate(-50%, -50%);
  box-shadow: 0 0 0 1.25vmin var(--iris);
}

.eye::after {
  width: 1vmin;
  height: 1vmin;
  background: #fff;
  border-radius: 100%;
  top: 35%;
  left: 55%;
  box-shadow: 0.5vmin 0.5vmin 0 -0.25vmin #fff;
}

.eye + .eye {
  left: 61%;
}

.nose {
  width: 16%;
  height: 36%;
  border-radius: 0 2vmin 5vmin 5vmin;
  border: 1vmin solid var(--line-face);
  border-right: 0.75vmin solid var(--line-face);
  border-left-color: transparent;
  border-top: 0;
  left: 50%;
  top: 31%;
  transform: translate(-50%, 0);
  background: var(--skin);
}

.eyebrow {
  width: 40%;
  height: 20%;
  border-radius: 10% 30% 0 0;
  box-shadow: -0.75vmin -2.7vmin 0 -1vmin var(--hair);
  top: 30%;
  left: 57%;
}

.eyebrow + .eyebrow {
  border-radius: 30% 10% 0 0;
  box-shadow: 0.75vmin -2.7vmin 0 -1vmin var(--hair);
  left: 2%;
}

.nose::before {
  width: 4vmin;
  height: 4vmin;
  border: 0.75vmin solid var(--line-face);
  border-radius: 50%;
  border-left-color: transparent;
  border-top-color: transparent;
  bottom: -1%;
  right: -3.45vmin;
  box-shadow: inset -1.1vmin -0.65vmin var(--skin);
}

.nose::after {
  width: 4vmin;
  height: 4vmin;
  border: 0.75vmin solid var(--line-face);
  border-bottom: 1vmin solid var(--line-face);
  border-radius: 50%;
  border-right-color: transparent;
  border-top-color: transparent;
  bottom: -1.1%;
  left: -2.9vmin;
  background: var(--skin);
}

.mustache {
  width: 30%;
  height: 7%;
  background: hsla(0, 14%, 11%, 0.973);;
  border-radius: 100% 10% 30%;
  left: 52%;
  top: 67%;
  transform-origin: left center;
  transform: translate(-100%, 0) rotate(-10deg);
}

.mustache + .mustache {
  left: 48%;
  border-radius: 20% 100% 10% 30%;
  transform-origin: right center;
  transform: rotate(10deg);
}

.lip {
  width: 35%;
  height: 9%;
  background: #f007;
  top: 70%;
  left: 50%;
  transform: translate(-50%, 0);
  background: var(--skin);
  box-shadow: inset 0 0 0 5vmin rgba(128, 0, 0, 0.2),0px 15px 10px -15px #111;
}


.ear {
  width: 15%;
  height: 30%;
  background: var(--skin);
  border-radius: 70% 70% 50% 120%;
  top: 30%;
  left: 19%;
  transform: rotate(-4deg);
}

.ear::after {
  width: 100%;
  height: 100%;
  border-radius: 70% 70% 100% 50%;
  background: var(--skin);
  transform: rotate(10deg);
  left: 37vmin;
  top: 10%;
}

.back-hair {
  width: 20%;
  height: 30%;
  background: var(--hair);
  color: var(--hair);
  left: 20%;
  top: 10%;
  box-shadow: 33vmin 0, 0vmin -6vmin, 33vmin -6vmin;
}

.back-hair::after,
.back-hair::before {
  width: 80%;
  height: 25%;
  background: var(--hair);
  border-radius: 50%;
  top: -37%;
  left: 40%;
  transform: rotate(-10deg);
  box-shadow: 23vmin 5vmin, 9vmin -2vmin 0 1vmin
}

.back-hair::after {
  top: -43%;
  left: 80%;
  transform: rotate(10deg);
  box-shadow: 13vmin -4vmin, 7vmin -3vmin;
}

.forehead {
  width: 60%;
  height: 0.5%;
  background: #0000000d;
  top: 16%;
  left: 50%;
  transform: translate(-50%, 0);
}

.forehead::before {
  width: 70%;
  height: 100%;
  background: #00000009;
  top: -2.25vmin;
  left: 15%;
}

.mouth {
  width: 35%;
  height: 0.5%;
  background: rgb(238, 117, 117);
  border-radius: 100%;
  top: 74%;
  left: 50%;
  transform: translate(-50%, 0);
}

.earhole1 {
  width: 5%;
  height: 10%;
  background: hsla(0, 0%, 0%, 0.288);
  left: 0%;
  top: 55%;
  transform: translate(-50%, 0%) rotate(-20deg);
  
}

.earhole2 {
  width: 5%;
  height: 10%;
  background: hsla(0, 0%, 0%, 0.288);
  left: 95%;
  top: 55%;
  transform: translate(50%, 0%) rotate(20deg);
  
}

.blink {
  animation: blink 2s step-start infinite;
}

@keyframes blink {
  90% {
    transform: none;
    animation-timing-function: ease-in;
  }
  93% {
    transform: translateY(15px) scaleY(0)
  }
  100% {
    animation-timing-function: ease-out;
  }
}

.squeeze {
  animation: squeeze 2s infinite;
}

@keyframes squeeze {
  80% {
    transform: none;
    animation-timing-function: ease-in;
  }
  90% {
    transform: translateY(3px) scaleY(1)
  }
  100% {
    animation-timing-function: ease-out;
  }
}

</style>
