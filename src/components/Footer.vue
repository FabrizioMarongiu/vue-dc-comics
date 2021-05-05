<template>
  <footer>
      <div class="main-footer">
          <img src="@/assets/dc-comics-assets/img/dc-logo-bg.png" alt="" class="logo">
          <div class="container">
              <div class="lists">
                  <div class="left-list">
                  <h3>dc comics</h3>
                  <ul>
                      <li>
                         <a href="#"> Characters</a>
                    </li>
                      <li>
                         <a href="#"> Comics</a>
                    </li>
                      <li>
                         <a href="#"> Movies</a>
                    </li>
                      <li>
                         <a href="#"> TV</a>
                    </li>
                      <li>
                         <a href="#"> Games</a>
                    </li>
                      <li>
                         <a href="#"> Videos</a>
                    </li>
                      <li>
                         <a href="#"> News</a>
                    </li>
                  </ul>

                  <h3>shop</h3>
                  <ul>
                      <li>
                         <a href="#"> Shop DC</a>
                    </li>
                      <li>
                         <a href="#"> Shop Dc Collectibles</a>
                    </li>
                     
                  </ul>
              </div>
              <div class="middle-list">
                  <h3>dc comics</h3>
                  <ul>
                      <li>
                         <a href="#"> Terms Of Use</a>
                    </li>
                      <li>
                         <a href="#"> Privacy policy (New)</a>
                    </li>
                      <li>
                         <a href="#"> Ad Choices</a>
                    </li>
                      <li>
                         <a href="#"> Advertising</a>
                    </li>
                      <li>
                         <a href="#"> Jobs</a>
                    </li>
                      <li>
                         <a href="#"> Subscriptions</a>
                    </li>
                      <li>
                         <a href="#"> Talent Workshops</a>
                    </li>
                      <li>
                         <a href="#"> CPSC Certificates</a>
                    </li>
                      <li>
                         <a href="#"> Ratings</a>
                    </li>
                      <li>
                         <a href="#"> Shop Help</a>
                    </li>
                      <li>
                         <a href="#"> Contact Us</a>
                    </li>
                  </ul>
              </div>

              <div class="right-list">
                  <h3>dc comics</h3>
                  <ul>
                      <li>
                         <a href="#"> DC</a>
                    </li>
                      <li>
                         <a href="#"> MAD Magazine</a>
                    </li>
                      <li>
                         <a href="#"> DC Kids</a>
                    </li>
                      <li>
                         <a href="#"> DC Universe</a>
                    </li>
                      <li>
                         <a href="#"> DC Power Visa</a>
                    </li>
                  </ul>
              </div>
              </div>
          </div>

      </div>
      <div class="bottom-footer">
            <div class="container link-footer">
                <a href="" class="btn">sign-up now!</a>
            
                <div class="follow">
                    <span class="follow-text">follow us</span>
                    <a href="#">
                        <img src="@/assets/dc-comics-assets/img/footer-facebook.png" alt="">
                    </a>
                    <a href="#">
                        <img src="@/assets/dc-comics-assets/img/footer-twitter.png" alt="">
                    </a>
                    <a href="#">
                        <img src="@/assets/dc-comics-assets/img/footer-youtube.png" alt="">
                    </a>
                    <a href="#">
                        <img src="@/assets/dc-comics-assets/img/footer-pinterest.png" alt="">
                    </a>
                    <a href="#">
                        <img src="@/assets/dc-comics-assets/img/footer-periscope.png" alt="">
                    </a>
                </div>
          </div>

      </div>
  </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style scoped lang="scss">
// MAIN FOOTER
.main-footer{
    height: 300px;
    background-image: url(../assets/dc-comics-assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
    overflow: hidden;
    padding: 30px 0;

    .logo{
        width:400px;
        position: absolute;
        top: -60px;
        right:240px;
    }
    .lists{
        display: flex;
        justify-content: start;
    }
    h3{
        font-size: 20px;
        color: white;
        text-transform: uppercase;
        margin-top: 20px;
    }
    li{
        list-style: none;
    }
    a{
        color: #747779;
        text-decoration: none;
        font-size: 14px;
    }
    .left-list,
    .middle-list,
    .right-list{
        margin: 0 20px
    }

}

// LINK FOOTER
.bottom-footer{
    height: 100px;
    background-color: #303030;
    
    .link-footer{
        display: flex;
        justify-content:space-between;
        align-items: center;
    }
    .btn{
        display:inline-block;
        width: 180px;
        height: 50px;
        border: 1px solid #0282f9;
        text-transform: uppercase;
        text-decoration: none;
        text-align: center;
        font-size: 20px;
        padding: 13px;
        color: white;
        
        &:hover{
            text-decoration: none;
            background-color: #4e91cf;
        }

    }
    .follow{
        display: flex;
        align-items: center;
    
        a{
        margin: 0 10px;
        }
        .follow-text{
            text-transform: uppercase;
            font-size: 20px;
            color:#0282f9;
            margin: 0 10px;
        }
    }
}


</style>