<script setup>
import { Swiper, SwiperSlide } from "swiper/vue"
import "swiper/css"
</script>


<template>
  <Navigation />
  <Pagination />
  <div class="nav-container">

    <div class="fif-nav">
      <img class= "fif_logo" src= "@/assets/fif-logo.png" height="40" width="40">
      <h2> F.I.F</h2>
    </div>
    

    <div class="nav-items">
      <h3 style="color: white;">Actualités</h3>
      <h3>Les Élephants</h3>
      <h3>Competitions</h3>
      <h3>La F.I.F</h3>
    </div>

    <div class="social-links">
      <img src="@/assets/fb-logo.png" height="40" width="40">
      <img src="@/assets/yt-logo.png" height="40" width="60">
      <img src="@/assets/tt-logo.png" height="40" width="40">
    </div>

  </div>

  <div class="header-container">
    <img src="@/assets/fif-logo.png" height="50" width="50">
    <h1 id="green-text">LA F.I.F</h1>
    <h1>TOUTE L'ACTUALITE <br> FOOT IVOIRIENNE</h1>
  </div>


  <h3 class="alaune" style="color: #626368">A la une</h3>

  <div class="carousel-main">
    
    <Swiper :slides-per-view="1" :space-between="25">

      <SwiperSlide v-for="n in 1" :key="n">
        <div class="carousel-first" id="carousel-item">

          <img id="carousel-pic" src="@/assets/equipe1.jpg" width="460" height="340">
          
          <div id="article-lorem">
            <h3 id="green-text">Catégorie</h3>
            <h2 id="article-title">Lorem ipsum dolor sit amet.</h2>
            <h3 id="article-content">Beef ribs t-bone kielbasa pastrami. Veniam velit incididunt reprehenderit dolore aute pork belly qui drumstick deserunt jerky. Ipsum ut andouille mollit salami doner. Sunt minim ball tip quis laborum qui id prosciutto ea, aute strip steak shank esse. Pariatur veniam aliquip tenderloin landjaeger. Consectetur spare ribs hamburger short loin sed, aliqua aute. Tail incididunt chicken tri-tip occaecat buffalo ad pig qui capicola ribeye cupim velit filet mignon.</h3>

            <div class="read-btn" style="margin-left: 40%; margin-top: 50px;">
              <img src="@/assets/arrow-right.png" width="24" height="24" style="margin-top: 20px;">
              <h3>Lire</h3>
            </div>

          </div>

        </div>
      </SwiperSlide>

      <SwiperSlide v-for="n in 1" :key="n">
        <div class="carousel-second" id="carousel-item">
          <img id="carousel-pic" src="@/assets/equipe2.jpg" width="460" height="340">

          <div id="article-lorem">
            <h3 id="green-text">Catégorie</h3>
            <h2 id="article-title">Lorem ipsum dolor sit amet.</h2>
            <h3 id="article-content">Tri-tip pork belly alcatra, corned beef magna prosciutto pork loin. Capicola ex eu ham hock, do dolore doner. Meatloaf dolore eu ut spare ribs ham hock corned beef porchetta frankfurter commodo salami. Kevin t-bone chuck, minim hamburger laborum pariatur rump boudin ball tip. Consectetur deserunt hamburger et ex pork quis shank tri-tip turkey ham hock nulla tempor, exercitation elit.</h3>

            <div class="read-btn" style="margin-left: 40%; margin-top: 50px;">
              <img src="@/assets/arrow-right.png" width="24" height="24" style="margin-top: 20px;">
              <h3>Lire</h3>
            </div>

          </div>

        </div>
      </SwiperSlide>

      <SwiperSlide v-for="n in 1" :key="n">
        <div class="carousel-third" id="carousel-item">

          <img id="carousel-pic" src="@/assets/equipe3.jpg" width="460" height="340">

          <div class="article-lorem">
            <h3 id="green-text">Catégorie</h3>
            <h2 id="article-title">Lorem ipsum dolor sit amet.</h2>
            <h3 id="article-content">Bacon ipsum dolor amet non venison filet mignon landjaeger, prosciutto enim reprehenderit tenderloin aliquip culpa. Landjaeger dolore proident ham consequat buffalo. Eu ex do, ullamco id exercitation irure kevin strip steak. Cow id salami ad ea, qui ut jowl ex strip steak. Mollit chuck irure ex ipsum eu consectetur sed sint prosciutto fatback pork loin.</h3>

            <div class="read-btn" style="margin-left: 40%; margin-top: 50px;">
              <button class="read-btn">
                <img src="@/assets/arrow-right.png" width="24" height="24" style="margin-top: 20px;">
                <h3>Lire</h3>
              </button>
            </div>

          </div>

        </div>
      </SwiperSlide>
    </Swiper>
  </div>

  <div class="slider-pages">

    <div id="arrow-btn" style="padding-right: 0px;">
      <button class="page-btn">
        <img src="@/assets/arrow-left.png" width="48" height="48">
      </button> 
    </div>

    <div class="dots-wrapper">
      <div class="dots"></div>
      <div class="dots"></div>
      <div class="dots"></div>
    </div>



    <div id="arrow-btn">
      <button class="page-btn">
        <img src="@/assets/arrow-right.png" width="48" height="48">
      </button>
    </div>
  </div>


  <div>
    <img class="advert" src="@/assets/mcdonalds-angus-burger.webp" width="300" height="10">
  </div>

  <h3 class="section-text">Les Articles</h3>

  <div class="filters">

    <h3 style="color: white;">Filtrer</h3>
    <button id="filter-btn" style="background-color: #8EF6D3; color: black;">Tous</button>
    <div class="divider"></div>
    <button id="filter-btn">FIF TV</button>
    <button id="filter-btn">Les Élephants</button>
    <button id="filter-btn">Compétition</button>
    <button id="filter-btn">International</button>
    <button id="filter-btn">Ligue 1</button>
    <button id="filter-btn">Les petits poteaux</button>
    <button id="filter-btn">Le meilleur</button>

  </div>

  <div class="datas">

    <div class="scrolly-ad">
      <img src="@/assets/scrolly-ad.jpeg" alt="">
    </div>

    <div class="article-list">


      <div v-for="title in titles.slice(0,12)" :key="title.id">

        <div class="all-arts">


          <div class="article-wrap">

            <img src='@/assets/ic_flag.jpg' height="120" width="260" class="art-img">
            <h3 class="art-category">{{ title.Category }}</h3>
            <h3 class="art-title"> {{ title.Title }}</h3>


            <div class="art-bottom">
              <h3 class="art-date"> {{ title.Date }}</h3>
              <div class="duration-wrap">
                <img src="@/assets/clock.png" width="12" height="12" style="margin-top: 15px;">
                <h3 class="art-duration"> {{ title.Duration }}min</h3>
              </div>

            </div>

          </div>

        </div>

      </div>


    </div>
    


    


  </div>

  <div class="footer-wrap">

    <div class="footer-left">

      <div class="fif-footer">
        <img class= "fif_logo-footer" src= "@/assets/fif-logo.png" height="40" width="40" style="margin-top: 15px; margin-right: 15px;">
        <p style="color:white">F.I.F</p>
      </div>

      <p style="color:#626368 ; display: flex; justify-content: flex-start;">Fédération Ivoirienne de Football, <br> Élephants, DTN, Championnats, <br> Actualités, Photos, Vidéos</p>

      <div class="faq-wrapper">
        <p id="green-text"> Notre F.A.Q</p>
        <img src="@/assets/arrow-right.png" height="16" width="16" style="margin-top: 20px;">
      </div>

      <div class="social_footer">
        <img src="@/assets/fb-logo.png" height="40" width="40">
        <img src="@/assets/yt-logo.png" height="40" width="60">
        <img src="@/assets/tt-logo.png" height="40" width="40">
      </div>

      <div class="footer-last">
        <h3>Une question?</h3>
        <button class="contact-btn">Contactez nous</button>
      </div>


    </div>

    <div class="footer-right">

      <div class="footer_columns">

        <div class="column_one">
          <h3 id="bold-footer">Actualités</h3>
          <p id="footer-sections">LA F.I.F</p>
          <p id="footer-sections">Le meilleur des réseaux</p>
          <p id="footer-sections">Ligues</p>
          <p id="footer-sections">Internationale</p>
        </div>

        <div class="column_two">
          <h3 id="bold-footer">Les Élephants</h3>
          <p id="footer-sections">Équipe A</p>
          <p id="footer-sections">Équipe Féminine</p>
          <p id="footer-sections">Équipe A'</p>
          <p id="footer-sections">U23</p>
          <p id="footer-sections">U19</p>
          <p id="footer-sections">U17</p>
        </div>

        <div class="column_three">
          <h3 id="bold-footer">Compétitions</h3>
          <p id="footer-sections">Ligue 1</p>
          <p id="footer-sections">Division 2</p>
          <p id="footer-sections">Nationale</p>
          <p id="footer-sections">Les petits poteaux</p>
        </div>

        <div class="column_four">
          <h3 id="bold-footer">LA F.I.F</h3>
          <p id="footer-sections">Actualités</p>
          <p id="footer-sections">Qui sommes-nous ?</p>
          <p id="footer-sections">Organisation</p>
          <p id="footer-sections">DTN</p>
          <p id="footer-sections">Historique</p>
        </div>

      </div>

      <h3 style="color: #626368; font-size: 14px; margin-top: 120px; margin-right: 460px;">© Lorem - 2077 Lorem ipsum dolor si amet.</h3>

    </div>

  </div>


</template>

<script>
import allArticles from '@/packages/MOCK_DATA.json'

export default {
  data () {
    return {titles: allArticles}
  }
}
</script>

<style>
@font-face {
    font-family: "satoshi";
    src: url(@/fonts/satoshi/satoshi_regular.otf);
  }
  
  @font-face {
    font-family: "neutro";
    src: url(@/fonts/neutro/Neutro-Bold.otf);
  }
  
  body {
    background-color: #121213;
    margin: 0px;
  }
  
  #app {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }
  
  .nav-container {
    z-index: 2;
    font-family: satoshi;
    width: 100%;
    top: 0;
    left: 0;
    position: sticky;
    background-color: #171719;
    color: white;;
    display: flex;
    justify-content: space-around;
    padding-bottom: 20px;
    margin-bottom: 36px;
  }
  
  .fif-nav {
    margin-top: 15px;
    display: flex;
    flex-direction: row;
    padding-right: 75px;
  }
  
  .fif_logo {
    margin-top: 15px;
    margin-right: 10px;
  }
  
  .nav-items {
    margin-top: 15px;
    color: #626368;
    width: 750px;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
  }
  
  .social-links {
    margin-top: 25px;
    width:350px;
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
  }
  
  .header-container {
    font-family: neutro;
    color: white;
  
  }
  
  .header-container::after {
    content: '';
    position: absolute;
    z-index: -1;
    inset: 0;
    opacity: 1;
    background-image: url("@/assets/background-header.svg");
    background-size: 50%;
    background-repeat: no-repeat;
    background-position: 50% 15%;
  }
  
  .alaune {
    font-family: satoshi;
    margin-top: 150px;
    padding-right: 1700px;
  }
  
  .carousel-main {
    color: white;
    display: flex;
    justify-content: center;
    flex-direction: row-reverse;
    margin-left: 15%;
    margin-top: 50px;
    width: 1160px;
    border: 20px;
  }
  
  #green-text {
    color: #8EF6D3;
  }
  
  #dark-grey {
    color:#626368;
  }
  
  .section-text{
    font-family: satoshi;
    color: #626368;
    padding-right: 1700px;
  }
  
  #carousel-item {
    background-color: #1F1F23;
    width: fit-content;
    font-family: satoshi;
    justify-content: center;
    display: flex;
    flex-direction: row;
    border-radius: 40px;
    padding-right: 15px;
  }
  
  #carousel-pic {
    border-radius: 40px;
    margin-top: 50px;
    margin-bottom: 50px;
    margin-left: 50px;
    padding-right: 15px;
  }
  
  #article-content {
    color: #AFAFB6;
  }
  
  .advert {
    width: 728px;
    height: 90px;
    margin-top: 240 px;
  }
  
  .filters {
    width: 1600px;
    font-family: satoshi;
    background-color: #1F1F23;
    display: flex;
    margin-left: 5%;
    border-radius: 16px;
    justify-content: space-around;
    padding-top: 15px;
  }
  
  .divider {
    border: 1.5px solid #313139;
  }
  
   #filter-btn {
    font-family: satoshi;
    font-size: 16px;
    color: white;
    background-color: #1F1F23;
    border: 2px solid;
    border-radius: 40px;
    border-color: #2b2b31;
    width: 180px;
    height: 48px;
   }
  
   #filter-btn:hover {
    border-color: white;
   }
  
   .datas {
    display: flex;
    flex-wrap: wrap;
    flex-basis: 50%;
    justify-content: center;
    flex-direction: row;
    font-family: satoshi;
    color: white;
    max-width: 1400px;
   }
  
   .read-btn {
    display: flex;
    flex-direction: row;
   }
  
   .slider-pages {
    padding-top: 80px;
    padding-bottom: 80px;
    display: flex;
    flex-direction: row;
    justify-content: center;
    border-radius: 40px;
   }
  
   .dots-wrapper {
    margin-top: 20px;
    margin-right: 70px;
    margin-left: 70px;
    display: flex;
    width: 46px;
    justify-content: space-evenly;
    flex-direction: row;
   }
  
   .dots {
    background-color: white;
    border: 1.5px solid #1F1F23;
    border-radius: 40px;
    height: 6px;
    width: 6px;
   }
  
   .article-wrap {
    height: 400px;
    width: 300px;
    border-radius: 40px;
    border: 1px solid #1F1F23;
    display: flex;
    justify-content:space-evenly;
    flex-direction: column;
    background-color: #1F1F23;
    margin: 25px;
   }
  
   .art-bottom {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    color: #626368;
    font-size: 12px;
   }
  
   .art-category {
    font-size: 16px;
    margin-left: 15px;
    display: flex;
    justify-content: flex-start;
    color: #76f4b0;
   }
  
   .art-title {
    margin-left: 15px;
    display: flex;
    justify-content: flex-start;
   }
  
   .duration-wrap {
    display: flex;
    justify-content: end;
   }
  
   .art-img {
    margin-left: 1.2em;
    border-radius: 30px;
    margin-top: 20px;
    height: 250px;
   }
  
   .footer-wrap {
    display: flex;
    font-family: satoshi;
    background-color: #171719;
    justify-content: space-evenly;
   }
  
   .fif-footer {
    display: flex;
    flex-direction: row;
    font-size: 22px;
   }
  
   .footer-left {
    display: flex;
    align-items: flex-start;
    flex-direction: column;
   }
  
   .footer-right {
    width: 800px;
    display: flex;
    flex-direction: column;
   }
  
   .footer_columns {
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
   }
  
  
   .faq-wrapper {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    margin-top: 15px;
    margin-bottom: 15px;
   }
  
  
   #footer-sections {
    color: #c9cacf;
   }
  
   #bold-footer {
    color: white;
   }
  
   .footer-last {
    display: flex;
    flex-direction: row;
    color: white;
    padding-bottom: 15px;
    margin-top: 80px;
   }
  
   .contact-btn {
    font-size: 16px;
    margin-left: 20px;
    padding: 4px 8px;
    background-color: #171719;
    color: white;
    border: 3px solid white;
    border-radius: 40px;
    transition: .2s;
   }
  
   .contact-btn:hover {
    background-color: white;
    color: black;
   }
  
   .page-btn {
    background-color: #1F1F23;
    border: 1px #1F1F23;
    border-radius: 40px;
    transition: 0.2s;
   }
  
   .page-btn:hover {
    filter: invert();
   }
  
   .read-btn {
    width: 100px;
    background-color: #1F1F23;
    border: 1px solid white;
    border-radius: 40px;
    transition: 0.2s;
    display: flex;
    justify-content: center;
   }
  
   .read-btn:hover {
    filter: invert();
   }
  
   .scrolly-ad {
    margin-left: 1680px;
    position: sticky;
    top: 0;
   }
  
   .article-list {
    display: flex;
    flex-direction: row-reverse;
    flex-wrap: wrap;
   }


</style>

