* {box-sizing: border-box;}
body {
  font-family: "Lora", serif;
  font-optical-sizing: auto;
  font-weight: 500px;
  font-style: italic;
}
/* .lora-<uniquifier> */
/* nav bar start */
.logoImage {
  width: 5%;
}
.nav-item a {
  position: relative;
}
@media screen and (min-width: 992px) {
  .nav-item a::before {
    content: "";
    position: absolute;
    background-color: black;
    width: 0%;
    height: 1.3px;
    left: 5px;
    bottom: 5px;
  }
  .nav-item a:hover::before {
    width: 80%;
    transition: 0.5s;
  }
}
/* nav bar end*/
/* Home page start */
.homeText:hover {
  cursor: pointer;
  letter-spacing: 3px;
  transition: 0.7s;
  text-shadow: black 2px 2px;
}
/* Home page end */
/* categories start */
.catego::before{
  content: "";
  width: 100%;
  height: 40px;
  position: absolute;
  left: 0;
  opacity: 0.5;
}
.catego-img img:hover{
  box-shadow: gray 2px 2px 2px 2px;
  transition: 0.5s;
}
/* categories end */
/* Bestseller  */
.overlaybox {
  position: relative;
}
.overlayimg {
  display: block;
  width: 100%;
  height: auto;
}
.overlay {
  position: absolute;
  bottom: 0;
  background: rgb(0, 0, 0);
  background: rgba(0, 0, 0, 0.5); /* Black see-through */
  color: #f1f1f1;
  width: 90%;
  transition: .5s ease;
  opacity:0;
  color: white;
  padding: 20px;
  text-align: center;
}
.overlaybox:hover .overlay {
  opacity: 1;
}
/* bestseller end */
/* card slider start */
/* for loptop screen */
@media screen and (min-width:568px) {
.cards-wrapper{
  display: flex;
}  
.card{
  margin: 0.5em;
  width: calc(100%/3);
}
.image-wrapper{
  height: 22vw;
  margin: 0 auto;
}
}
.image-wrapper img{
  max-width: 100%;
  max-height: 100%;
}
/* only one card will show and 2 cards will hide */
@media screen and (max-width:567px) {
  .card:not(:first-child){
    display: none;
  }
}
.card {
  box-shadow: gray 2px 2px 2px 2px;
}
/* styling carousel */
.carousel-control-prev,.carousel-control-next{
  background-color: black;
  width: 6vh;
  height: 6vh;
  border-radius: 50%;
  top: 50%;
  transform: translateY(-50%);
}
/* airpods section start */
.airpods-main{
  position: relative;
  max-width: 100%;
}
.airpods-overlay{
  color: white;
  width: 100%;
  position: absolute;
  left: 0;
  top: 50%;
}
.airpods-section img:hover{
  box-shadow:gray 2px 2px 2px 2px;
}
@media screen and (max-width:578px) {
  .airpods-overlay{
    width: 100%;
    left: 0;
    top: 38%;
  }
  .airpods-overlay h1 {
    font-size: 20px;
  }
  .airpods-overlay h3 {
    font-size: 17px;
  }
  .footer-div .footer-a a{
    margin: 10px 0;
  }
  .steve-text img{
    display: none;
  }
  .steve-h h5{
    display: none;
  }
}
@media screen and (max-width:768px) {
  .airpods-overlay{
    width: 100%;
    left: 0;
    top: 50%;
  }
  .airpods-overlay h1 {
    font-size: 20px;
  }
  .airpods-overlay h3{
    font-size: 18px;
  }
  .airpods-overlay h5{
    font-size: 15px;
  }
  .airpods-overlay a{
    font-size: 15px;
  }
  .footer-div .footer-a a{
    margin: 15px auto;
  }
  .footer-div .footer-a .exchange {
    margin: auto;
  }
}

/* airpods section end */
/* homepod section start */
@media screen and (max-width: 575px) {
  .homepod-text img{
    width: 30%;
  }
}
@media screen and (min-width:578px) {
  
  .homepod-text img{
    width: 30%;
  }
}
@media screen and (min-width:768px) {
  
  .homepod-text{
    line-height: 30px;
    border: 1px black outset;
  }
  .homepod-text img{
    width: 35%;
  }
}
@media screen and (min-width:  993px) {
.homepod-text{
  display: flex;
  align-items: center;
  font-size: larger;
  line-height: 50px;
  border: gray 1px solid;
  box-shadow:gray 3px 3px 3px 3px;
}
.homepod-text img{
  width: 40%;
}
}
/* footer start */
.steve-text{
  display: flex;
  align-items: center;
  text-align: center;
}
.steve-text .steve-h{
  margin: auto;
}
