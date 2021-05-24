<template>
  <div id="About" style="margin-top:30px">
  <div class="container">
      <div class="row">
      
        <div class="col-md-3 sidebar">

        
            <h1>Skills</h1>
            <ul>
              <div class="lii">
                <li>CSS</li>
                <li>HTML5</li>
                <li>CSS</li>
                <li>JavaScript</li>
                <li>VueJs</li>
                <li>ReactJs</li>
              </div>
              <div class="lii">
                <li>C/C++</li>
              <li>Python</li>
              <li>Django</li>
              <li>DSA</li>
                  <li>Problem Solving</li>
                  <li>System Design</li>
              </div>
            </ul>
            <h1>Links</h1>
            <ul>
              <div class="lii">
                <li>
                  <a href="https://www.linkedin.com/in/anuj-patel-b87399195/" target="blank">LinkedIn</a>
                </li>
                <li>
                  <a href="https://github.com/foxface-ap" target="blank">GitHub</a>
                </li>
              </div>
              <div class="lii">
                <li>
                  <a href="https://codeforces.com/profile/foxface_ap" target="blank">Codeforces</a>
                </li>
                <li>
                  <a href="https://www.codechef.com/users/foxface_ap" target="blank">CodeChef</a>
                </li>
              </div>
            </ul>

      </div>
      <div class="col-md-9 content">
        <h2 id="por">Position of Responsibility</h2>
        <ul>
          <h5 class="pos">1. RECursion, NIT Dgp Senior Coordinator</h5>
          <p class="details">Part of the Teaching and Web Development team, the task is to
            monitor the functioning of the official website of the club and
            conduct weekly classes for budding coders of the college.
          </p>    
          <h5 class="pos">2. Aarohan, NIT Dgp Senior Fest- Coordinator</h5>
          <p class="details">Responsible for conducting various fest activities and managing fest activities.Effectively multitasked and prioritized work according to need.
          </p>   
          <h5 class="pos">3. Developer at Edvise</h5>
          <p class="details">Developed UI for the ed-tech startup (Edvise) using React web framework. Worked well independently and with team.

          </p>     
        
        </ul>
      </div>
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

.lii {
  width:50%;
  float:left;
  font-size: 1.8rem;
}

@media only screen and (max-width: 1340px) {
  .lii {
    width:100%;
    float:none;
    font-size: 1.8rem;
  }
}


#por{
  font-size: 4rem;
  font-weight: 300px;
}
.pos{
   font-size: 2.5rem;
}
.details{
   font-size: 1.8rem;
   padding-top: 0px;
}

@media only screen and (max-width: 1200px) {
  #por{
    font-size: 2.8rem;
    font-weight: 300px;
  }
  .pos{
    font-size: 2.3rem;
  }
  .details{
    font-size: 1.8rem;
  }

}

.sidebar {
  height: 150%;
  transform: translate(20px);
  padding: 30px 0px 30px 30px;
  background: linear-gradient(to bottom, #ade7fa 0%, #007da7 100%); 
  color: #001b24;
  box-sizing: border-box;
  font-weight: 600;
}

.row{
  background: #006182; 
  border-radius: 15px;
}

#About
{
  width: 100%;
  height: 100%;
  padding: 3em 0em;
  /* background: transparent; */
  color: #67575D;
  line-height: 1.3;
}


.container {
  position: relative;
  max-width: 1400px;
  width: 80%;
  height: 70%;
  box-shadow: 0px 5px 15px 0px #37809f;
}

.sidebar a {
  color: #001b24;
  text-decoration: none;
  font-weight: 600;
}

.content {
  overflow: auto;
  padding-left: 40px;
  color: #dbf5fd;
}
.content p{
  text-align: left;
}

ul {
  list-style: none;
}

li {
  margin-bottom: 8px;
  width: 50%;
  width: 100%;
}

li:before {
  content: "+";
  margin-right: 8px;

}


@media (max-width: 900px) {

  .sidebar li {
    margin: 0;
    margin: 4px;
  }
  .sidebar{
    border-top-left-radius: 15px;
    border-top-right-radius: 15px;
    transform: translate(0px);
  }
  .content p{
    margin: 1px;
    
  }
  .content {
    padding-left: 30px;
  }
  .container {
  position: relative;
  max-width: 1400px;
  width: 90%;
  height: 70%;
  box-shadow: 0px 5px 15px 0px #37809f;
}
  
}

</style>
