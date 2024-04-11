<script>
export default {
    name: 'AppFooterLinks',
    
}
</script>

<template>
<section id="footer-links">
    <div class="container">
        <div class="row">
            <div class="col-4">
                <div class="row ">
                    <div class="col-4 p-3">
                        <h5>DC COMICS</h5>
                        <ul class="p-0 m-0 mb-3">
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                     
                        <h5>SHOP</h5>
                        <ul class="p-0 m-0">
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectables</a></li>
                        
                        </ul>
                    </div>
                
                    
                    <div class="col-4 p-3">
                        <h5>DC</h5>
                        <ul class="p-0 m-0">
                            <li><a href="#">Terms Of Use</a></li>
                            <li><a href="#">Privacy policy(New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscription</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                    </div>
                    <div class="col-4 p-3">
                        <h5>SITES</h5>
                        <ul class="p-0 m-0">
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>
                
                    
                </div>
            </div>
            <div class="col-8 d-flex justify-content-end align-items-center "><img class="" src="../assets/img/dc-logo-bg.png" alt=""></div>
        </div>
    </div>
</section>
</template>

<style scoped lang="scss">
section{
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    height: 500px;
    .container{
        height: 100%;
        >.row{
            height: 100%;
            .col-4{

               

                color: aliceblue;
                a{
                    color: gray;
                }
            }
        }
    }
    .col-8{
        height: 100%;
    
        overflow-y: hidden;
    
        img{
            height: 140%;
           
            
         
        }

    }
}


</style>