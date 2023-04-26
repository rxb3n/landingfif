<script setup>
import { Swiper, SwiperSlide } from "swiper/vue"
import "swiper/css"
</script>



<template>
  <Navigation />
  <Pagination />

    <!--------- NAVBAR ----------->

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

    <!--------- HEADER ----------->

  <div class="header-container">
    <img src="@/assets/fif-logo.png" height="50" width="50">
    <h1 id="green-text">LA F.I.F</h1>
    <h1>TOUTE L'ACTUALITE <br> FOOT IVOIRIENNE</h1>
  </div>

      <!--------- CAROUSEL ----------->


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

        <!--------- CAROUSEL ARROW BTNS ----------->

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

      <!--------- ARTICLES ----------->

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

    <div class="scrolly-ad" style="display: flex; position:sticky; right: 200px;">
      <img src="@/assets/scrolly-ad.jpeg" style="padding-top: 50px;">
    </div>

    <div class="article-list">

      <div v-for="title in titles.slice(0,12)" :key="title.id">

        <div class="all-arts">

          <div class="article-wrap">

            <img src='https://picsum.photos/200' height="120" width="260" class="art-img">
            <h3 class="art-category" style="margin-bottom: 1px;">{{ title.Category }}</h3>
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

      <!--------- PAGINATION ----------->

  <div id="pagination-wrapper">
    <paginate
      :page-count="20"
      :click-handler="functionName"
      :prev-text="'<'"
      :next-text="'>'"
      :container-class="'className'"
      :page-class="'page-item'"
    >
    </paginate>
  </div>

        <!--------- FOOTER ----------->

  <div id="lower-ad">
    <img src="@/assets/mcdonalds-angus-burger.webp" height="150px" style="padding-bottom: 25px;">
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

      <!--------- SCRIPTS ----------->

<script>
import allArticles from '@/packages/MOCK_DATA.json'
import Paginate from "vuejs-paginate-next";

export default {
  data () {
    return {titles: allArticles,}
  },


}
</script>

      <!--------- STYLE IMPORT ----------->

<style>@import url(styles.css);</style>

