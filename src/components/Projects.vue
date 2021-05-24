<template>

  <div id="sec-3">
  <h1 id="heading">Projects I've worked on</h1>
  <div class="container">
    <div class="container3">
        <div class="faders">
            <div class="left"></div>
            <div class="right"></div>
        </div>

        <div class="items">
            <div class="entry">
                <p class="name">Get Started</p>
                <a href="https://recursionnitd.in/" target="_blank">LINK</a>
                <p class="quote">
                    Get Started section in RECursion Website provides indepth study material for CP. 
                    Implemented using Django.
                </p>
            </div>
            <div class="entry">
                <p class="name">UI/UX Designer</p>
                <p class="quote">Edvise is an ed-tech startup, I was responsible for designing website for the organisation. Implemented using ReactJs and Material-UI.</p>
            </div>
            <div class="entry">
                <p class="name">Ecommerce Website</p>
                <p class="quote">Website contains features like user authentication,adding product to cart, whishlist, and products. Implemented using Django.</p>
            </div>
            <div class="entry">
                <p class="name">REChase</p>
                <a src="http://rechase.pythonanywhere.com/" target="_blank">LINK</a>
                <p class="quote">An Online treasure hunt, hosted during pandemic, in Aarohan 2021, Tech fest NIT-Dgp. Implemented using Django.</p>
            </div>
            <div class="entry">
                <p class="name">Portfolio</p>
                <a src="http://rechase.pythonanywhere.com/" target="_blank">LINK</a>
                <p class="quote">My current Portfolio site. Contains about my interest, skills and projects. Implemented using VueJs and CSS.</p>
            </div>
            <div class="entry">
                <p class="name">Two Player Scorer</p>
                <a href="#" target="_blank">Two Player Scorer</a>
                <p class="quote">
                    Simple Scoring application for two player games. Here players can set number of rounds and maintaintrack of current standings.
                </p>
            </div>
            <div class="entry">
                <p class="name">Get Started</p>
                <a href="#" target="_blank">asafsa</a>
                <p class="quote">
                    Get Started section in RECursion Website provides indepth study material for CP. 
                    Implemented using Django.
                </p>
            </div>
               
        </div>
    </div>
  </div> 
  <Footer/>
  </div>

  
</template>

<script>
import Footer from "./Footer.vue";
export default {
  name: 'app',
  components: { 
    Footer,
  }
}
</script>

<style scopped>

#heading {
    text-align: center;
    margin: 2em;
    padding-top: 70px;
    color: #fff;
}


.container3 {
    width: 100%;
    overflow: hidden;
    position: relative;
    background-color: #ade7fa;
    color: #ade7fa;
}
.container{
    background-color: #ade7fa;
}

.items {
    display: flex;
    align-items: center;
    width: fit-content;
    animation: carouselAnim 5s infinite alternate linear;
}

.entry {
    display: flex;
    align-items: center;
    flex-direction: column;
    position: relative;
    width: 250px;
    background: #006182;
    margin: 1em;
    padding: .5em;
    border-radius: 8px;
    box-shadow: 4px 4px 5px 0px rgba(0,0,0,0.05);
}

.entry a
{
  color:#ade7fa;
}
.entry a:hover
{
  color:#001b24;
  text-decoration:none;
}
   
p {
    text-align: center;
    padding: 1em;
}

p.name {
    font-weight: bold;
}

@keyframes carouselAnim {
    from {
        transform: translate(0,0);
    }
    to {
        transform: translate(calc(-100% + (6*300px)));
    }
}


 

@media only screen and (max-width: 768px) {
    .items {
        animation: carouselAnim 15s infinite alternate linear;
    }

    @keyframes carouselAnim {
        from {
            transform: translate(0,0);
        }
        to {
            transform: translate(calc(-100% + (2*300px)));
        }
    }
}

.faders {
    width: 100%;
    position: absolute;
    height: 100%;
    background-color: #ade7fa;
}

.left, .right {
    background: linear-gradient(to right, #ade7fa 0%,rgba(158, 150, 150, 0) 100%);
    width: 5%;
    height: 100%;
    position: absolute;
    z-index: 200;
}
.left {
    left: -0.25%;
}

.right {
    right: 0;
    background: linear-gradient(to left, #ade7fa  0%,rgba(255,255,255,0) 100%);
    right: -0.45%;
}
    


</style>
