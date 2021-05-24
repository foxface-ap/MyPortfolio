<template>
  <div id="Footer">
    <footer class="site-footer">
      <div style="border-radius: 0px;">
        <div class="row" style="padding-top: 10px; padding: 2vw 10.5vw; margin-right: 0px;margin-left: 0px;border-radius: 0px;">
          <div class="col-md-3">
            <h6>© Anuj 2021</h6>
            <p class="text-justify footer-links" style="padding-top:0px">Handcrafted with Vue and CSS.</p>
            <ul class="social-icons">
              <div><a class="facebook" href="#"><i class="fa fa-facebook"></i></a></div>
              <div><a class="twitter" href="#"><i class="fa fa-whatsapp"></i></a></div>
              <div><a class="instagram" href="#"><i class="fa fa-instagram"></i></a></div>
            </ul>
          </div>

          

          <div class="col-md-3">
            <h6>Contacts</h6>
            <ul class="footer-links">
              <li><a href="mailto:anujpatel181299gmail.com" target="_blank">Email</a></li>
              <li><a href="tel:+916307675032" target="_blank">Phone</a></li>
              <!-- <li><a href='https://wa.me/27722840005' target='_blank'>dsgd</a></li> -->
            </ul>
          </div>

          <div class="col-md-6">
            <h6>About</h6>
            <p class="text-justify footer-links" style="padding-top:0px">
                        Through constant learning and creation, I try to produce
                        aesthetic software to the highest standard. I’m
                        largely framework agnostic but technologies I love
                        right now are Django, React, Vue and Styled Components.
            </p>
            
          </div>
        </div>
      </div>
        
            
           
</footer>

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

#Footer
{
  margin-top: 100px;
}

.site-footer
{
  font-size:15px;
  line-height:24px;
  color:#ade7fa;
  border-radius: none;
}



.site-footer hr.small
{
  margin:20px 0
}
.site-footer h6
{
  color: #001b24;
  font-size:16px;
  text-transform:uppercase;
  margin-top:5px;
  letter-spacing:2px;
  font-weight: 600;
  text-shadow: 0 0 5px #ade7fa;
}

.site-footer a
{
  color:#ade7fa;
}
.site-footer a:hover
{
  color:#3366cc;
  text-decoration:none;
}
.footer-links
{
  padding-left:0;
  list-style:none
}
.footer-links li
{
  display:block
}
.footer-links a
{
  color:#ade7fa;
}
.footer-links a:active,.footer-links a:focus,.footer-links a:hover
{
  color:#001b24;
  text-decoration:none;
}
.footer-links.inline li
{
  display:inline-block
}
.site-footer .social-icons a
{
  width:40px;
  height:40px;
  line-height:40px;
  margin-left:6px;
  margin-right:0;
  border-radius:100%;
  background-color:hsla(195, 89%, 83%, 0.185);
}
.copyright-text
{
  margin:0
}
@media (max-width:991px)
{
  .site-footer [class^=col-]
  {
    margin-bottom:30px
  }
}
@media (max-width:767px)
{
  .site-footer
  {
    padding-bottom:0
  }
  .site-footer .copyright-text,.site-footer .social-icons
  {
    text-align:center
  }
}
.social-icons
{
  padding-left:0;
  max-width: 300px;
  margin-bottom:0;
  list-style:none;
  display: flex;
}
.social-icons li
{
  display:inline-block;
  margin-bottom:4px
}
.social-icons li.title
{
  margin-right:15px;
  text-transform:uppercase;
  color:#ade7fa;
  font-weight:700;
  font-size:13px
}
.social-icons a{
  color:#ade7fa;
  font-size:20px;
  display:inline-block;
  line-height:44px;
  width:44px;
  height:44px;
  text-align:center;
  margin-right:8px;
  border-radius:100%;
  -webkit-transition:all .2s linear;
  -o-transition:all .2s linear;
  transition:all .2s linear
}
.social-icons a:active,.social-icons a:focus,.social-icons a:hover
{
  color:#fff;
  background-color:#29aafe;
}
.social-icons.size-sm a
{
  line-height:34px;
  height:34px;
  width:34px;
  font-size:14px
}
.social-icons a.facebook:hover
{
  background-color:#4267B2;
}
.social-icons a.twitter:hover
{
  background-color: #25D366;
}
.social-icons a.linkedin:hover
{
  background-color:#007bb6;
}
.social-icons a.instagram:hover
{
  background-color:#ea4c89;
}
@media (max-width:767px)
{
  .social-icons li.title
  {
    display:block;
    margin-right:0;
    font-weight:600;
  }
}

</style>
