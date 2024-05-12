<script setup>
import logo from "@/assets/logo.svg";
import main from "@/assets/main.jpg";
import footerLogo from "@/assets/f_logo.png";
import CardImg01 from "@/assets/img1.jpg";
import CardImg02 from "@/assets/img2.jpg";
import CardImg03 from "@/assets/img3.jpg";
import CardImg04 from "@/assets/img4.jpg";
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import "swiper/css/navigation";
import { Navigation } from "swiper/modules";
</script>

<template>
  <header>
    <div class="inner">
      <h1>
        <a href="javascript:;">
          <img :src="logo" alt="Logo" />
        </a>
      </h1>
      <nav>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
      </nav>
    </div>
  </header>
  <swiper :navigation="true" :modules="modules" class="mySwiper">
    <swiper-slide>
      <div class="inner">
        <div class="txt_box">
          <h3>
            Lorem ipsum <br />
            dolor sit amet,
          </h3>
          <p>
            Lorem ipsum dolor sit amet, <br />
            consectetur sed do eiusmod tempor <br />
            incididunt ut labore et dolore magna aliqua.
          </p>
        </div>
      </div>
      <div class="img_box">
        <img :src="main" alt="메인비주얼1" />
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="inner">
        <div class="txt_box">
          <h3>
            Lorem ipsum <br />
            dolor sit amet,
          </h3>
          <p>
            Lorem ipsum dolor sit amet, <br />
            consectetur sed do eiusmod tempor <br />
            incididunt ut labore et dolore magna aliqua.
          </p>
        </div>
      </div>
      <div class="img_box">
        <img :src="main" alt="메인비주얼1" />
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="inner">
        <div class="txt_box">
          <h3>
            Lorem ipsum <br />
            dolor sit amet,
          </h3>
          <p>
            Lorem ipsum dolor sit amet, <br />
            consectetur sed do eiusmod tempor <br />
            incididunt ut labore et dolore magna aliqua.
          </p>
        </div>
      </div>
      <div class="img_box">
        <img :src="main" alt="메인비주얼1" />
      </div>
    </swiper-slide>
  </swiper>

  <section class="section con01">
    <div class="inner">
      <ul class="card_box">
        <li>
          <div class="card_list">
            <div class="img">
              <img :src="CardImg01" alt="카드이미지" />
            </div>
            <div class="txt_box">
              <div class="tit">
                <h4>Lorem ipsum <br />dolor sit amet,</h4>
                <p>
                  Lorem ipsum dolor sit amet, <br />
                  consectetur adipiscing elit,
                </p>
              </div>
              <div class="btm_box">
                <p class="sub_text">Lorem ipsum dolor sit amet,</p>
              </div>
            </div>
          </div>
        </li>
        <li>
          <div class="card_list">
            <div class="img">
              <img :src="CardImg02" alt="카드이미지" />
            </div>
            <div class="txt_box">
              <div class="tit">
                <h4>Lorem ipsum <br />dolor sit amet,</h4>
                <p>
                  Lorem ipsum dolor sit amet, <br />
                  consectetur adipiscing elit,
                </p>
              </div>
              <div class="btm_box">
                <p class="sub_text">Lorem ipsum dolor sit amet,</p>
              </div>
            </div>
          </div>
        </li>
        <li>
          <div class="card_list">
            <div class="img">
              <img :src="CardImg03" alt="카드이미지" />
            </div>
            <div class="txt_box">
              <div class="tit">
                <h4>Lorem ipsum <br />dolor sit amet,</h4>
                <p>
                  Lorem ipsum dolor sit amet, <br />
                  consectetur adipiscing elit,
                </p>
              </div>
              <div class="btm_box">
                <p class="sub_text">Lorem ipsum dolor sit amet,</p>
              </div>
            </div>
          </div>
        </li>
        <li>
          <div class="card_list">
            <div class="img">
              <img :src="CardImg04" alt="카드이미지" />
            </div>
            <div class="txt_box">
              <div class="tit">
                <h4>Lorem ipsum <br />dolor sit amet,</h4>
                <p>
                  Lorem ipsum dolor sit amet, <br />
                  consectetur adipiscing elit,
                </p>
              </div>
              <div class="btm_box">
                <p class="sub_text">Lorem ipsum dolor sit amet,</p>
              </div>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </section>

  <section class="section con02"></section>

  <footer>
    <div class="inner">
      <div class="f_logo">
        <h1>
          <a href="javascript:;">
            <img :src="footerLogo" alt-="" />
          </a>
        </h1>
        <div class="copy_box">
          <p>Copyrights 2024. 테스트 All Rights Reserved</p>
        </div>
      </div>
    </div>
  </footer>
</template>
