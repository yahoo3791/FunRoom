<template>
  <div class="deluxeDouble_sm d-block d-md-none">
    <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel">
      <div class="carousel-indicators">
        <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"
          aria-current="true" aria-label="Slide 1"></button>
        <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"
          aria-label="Slide 2"></button>
        <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"
          aria-label="Slide 3"></button>
      </div>
      <div class="carousel-inner">
        <div class="carousel-item active overflow-hidden w-100" style="height:210px">
          <img src="@/assets/pic/room01.png" class="d-block w-100" style="object-fit:cover;" alt="...">
        </div>
        <div class="carousel-item overflow-hidden w-100" style="height:210px">
          <img src="@/assets/pic/room02.png" class="d-block w-100" style="object-fit:cover;" alt="...">
        </div>
        <div class="carousel-item overflow-hidden w-100" style="height:210px">
          <img src="@/assets/pic/room03.png" class="d-block w-100" style="object-fit:cover;" alt="...">
        </div>
      </div>
      <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators"
        data-bs-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators"
        data-bs-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>
    <div class="collapse_sm container-fluid">
      <div class="row" style="background:#F1F1F1;">
        <div class="col-6" :class="{ 'border-b': isEvaluation }">
          <a @click.prevent="checkIntroduction()" class="border-0 fs-6 btn d-block" data-bs-toggle="collapse"
            href="#collapseExample" role="button" aria-expanded="false" aria-controls="collapseExample">
            <span class="d-block article_a">????????????</span>
          </a>
        </div>
        <div class="col-6" :class="{ 'border-b': isIntroduction }">
          <router-link to="/room/deluxedouble/CommentReview" @click.prevent="checkEvaluation()"
            class="border-0 fs-6 btn d-block" data-bs-toggle="collapse" href="#collapseExample2" role="button"
            aria-expanded="false" aria-controls="collapseExample">
            <span class="d-block article_a">????????????(128)</span>
          </router-link>
        </div>
      </div>
      <p>
      </p>
      <div class="collapse show" id="collapseExample" :class='{ "d-none":isIntroduction }'>
        <div class="card card-body border-0">
          <div class="container">
            <div class="row">
              <div class="col-12 d-flex justify-content-between align-items-center">
                <div class="box">
                  <h2 class="fs-4 article_h2">Deluxe Double Room</h2>
                </div>
                <div class="box">
                  <div class="left">
                    <span class="text-info content_span">??????(???????????????)</span><br>
                    <p class="fs-5"><span class="fs-3 aside_seasonPrice_p">$2,888</span>/???</p>
                  </div>
                  <div class="right">
                    <span class="text-info content_span">??????(???????????????)</span><br>
                    <p class="fs-5"><span class="fs-3 aside_seasonPrice_p">$3,000</span>/???</p>
                  </div>
                </div>
              </div>
              <div class="col-12">
                <p class="article_p" style="text-align:justify;word-spacing: -2px;">Single Room is only reserved for one
                  guest. There is a
                  bedroom with a
                  single size bed and a private
                  bathroom. Everything you need prepared for you: sheets and blankets, towels, soap and shampoo,
                  hairdryer are provided. In the room there is AC and of course WiFi.</p>
              </div>
              <div class="col-7 ">
                <div class="row content_span">
                  <div class="col-12">
                    <h3 class="fs-5 pb-2">????????????</h3>
                  </div>
                  <div class="col-7 col-md-7">
                    <p class="fw-bolder">????????????</p>
                  </div>
                  <div class="col-5 col-md-5">
                    <p>1</p>
                  </div>
                  <div class="col-7 col-md-7">
                    <p class="fw-bolder">??????</p>
                  </div>
                  <div class="col-5 col-md-5">
                    <p>?????????</p>
                  </div>
                  <div class="col-7 col-md-7">
                    <p class="fw-bolder">????????????</p>
                  </div>
                  <div class="col-5 col-md-5">
                    <p>1</p>
                  </div>
                  <div class="col-7 col-md-7">
                    <p class="fw-bolder">????????????</p>
                  </div>
                  <div class="col-5 col-md-5">
                    <p>18????????????</p>
                  </div>
                </div>
              </div>
              <div class="col-5 content_span">
                <div class="col-12">
                  <h3 class="fs-5 pb-2">??????/????????????</h3>
                </div>
                <div class="col-sm-6 col-md-6">
                  <p class="fw-bolder">????????????</p>
                </div>
                <div class="col-sm-6 col-md-6">
                  <p class="">15:00~21:00</p>
                </div>
                <div class="col-sm-12 col-md-6">
                  <p class="fw-bolder">????????????</p>
                </div>
                <div class="col-sm-12 col-md-6">
                  <p class="">10:00??????</p>
                </div>
              </div>
              <div class="row">
                <div class="col-12">
                  <h3 class="fs-5 pb-2">????????????</h3>
                </div>
                <div class="col-12">
                  <ul class="article_icon px-0">
                    <li style="width:70px"><img src="@/assets/icon/wifi02.png" alt=""><br>
                      <p>wifi</p>
                    </li>
                    <li style="width:70px"><img src="@/assets/icon/breakfast02.png" alt=""><br>
                      <p>??????</p>
                    </li>
                    <li style="width:70px"><img src="@/assets/icon/minibar01.png" alt=""><br>
                      <p class="opacity-25">minibar</p>
                    </li>
                    <li style="width:70px"><img src="@/assets/icon/roomservce01.png" alt=""><br>
                      <p class="opacity-25">room<br>servce</p>
                    </li>
                    <li style="width:70px"><img src="@/assets/icon/phone02.png" alt=""><br>
                      <p>??????</p>
                    </li>
                    <li style="width:70px"><img src="@/assets/icon/aircon02.png" alt=""><br>
                      <p>??????</p>
                    </li>
                    <br>
                    <li style="width:70px"><img src="@/assets/icon/Group02.png" alt=""><br>
                      <p>??????</p>
                    </li>
                    <li style="width:70px"><img src="@/assets/icon/sofa01.png" alt=""><br>
                      <p class="opacity-25">??????</p>
                    </li>
                    <li style="width:70px"><img src="@/assets/icon/view01.png" alt=""><br>
                      <p class="opacity-25">View</p>
                    </li>
                    <li style="width:70px"><img src="@/assets/icon/smoke02.png" alt=""><br>
                      <p>????????????</p>
                    </li>
                    <li style="width:70px"><img src="@/assets/icon/children01.png" alt=""><br>
                      <p class="opacity-25">????????????</p>
                    </li>
                    <li style="width:70px"><img src="@/assets/icon/dog02.png" alt=""><br>
                      <p>????????????</p>
                    </li>
                  </ul>
                </div>
              </div>
              <div class="col-12 my-3">
                <button class="primaryBtn" @click="reservematerial()">????????????</button>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="collapse" id="collapseExample2" :class='{ "d-none": isEvaluation }'>
        <div class="card card-body border-0 my-3">
          <router-view></router-view>
        </div>
      </div>
    </div>
  </div>


  <div class="container d-none d-md-flex mb-5" id="deluxeDouble">
    <div class="left w-100">
      <div class="roomPic w-100">
        <img src="@/assets/pic/room01.png" alt="">
      </div>
    </div>
    <div class="right d-flex flex-column ms-2 w-100">
      <div class="roomPic w-100" style="margin-top: -10px;">
        <img src="@/assets/pic/room02.png" class="w-100" style="height:284px; object-fit: cover; overflow: hidden;"
          alt="">
      </div>
      <div class="roomPic w-100" style="margin-top: 10px;">
        <img src="@/assets/pic/room03.png" class="w-100" style="height:284px; object-fit: cover; overflow: hidden;"
          alt="">
      </div>
    </div>
  </div>
  <div class="container d-none d-md-flex justify-content-between mb-5">
    <div class="row">
      <div class="col-7">
        <div class="article">
          <div class="article_content">
            <div class="article_title pb-2 d-flex justify-content-between">
              <h2 class="article_h2">Deluxe Double Room</h2>
              <a href="" class="article_a text-decoration-underline text-primary"
                @click.prevent="openCommentModal()">????????????(128)</a>
            </div>
            <p class="article_p pb-3 text-info" style="text-align:justify; word-spacing:-2px;">Single Room is only
              reserved for
              one guest.
              There is a bedroom with a single size bed and a
              private
              bathroom. Everything you need prepared for you: sheets and blankets, towels, soap and shampoo, hairdryer
              are provided. In the room there is AC and of course WiFi.</p>
          </div>
          <div class="row mt-5">
            <div class="col-6">
              <div class="article_news row">
                <div class="col-12">
                  <h3 class="article_news_h3 fs-5 pb-2">????????????</h3>
                </div>
                <div class="col-6">
                  <p>????????????</p>
                </div>
                <div class="col-6">
                  <p>1</p>
                </div>
                <div class="col-6">
                  <p>??????</p>
                </div>
                <div class="col-6">
                  <p>?????????</p>
                </div>
                <div class="col-6">
                  <p>????????????</p>
                </div>
                <div class="col-6">
                  <p>1</p>
                </div>
                <div class="col-6">
                  <p>????????????</p>
                </div>
                <div class="col-6">
                  <p>18????????????</p>
                </div>
              </div>
            </div>
            <div class="col-6">
              <div class="article_time row">
                <div class="col-12">
                  <h3 class="article_time_h3 fs-5 pb-2">??????/????????????</h3>
                </div>
                <div class="col-6">
                  <p>????????????</p>
                </div>
                <div class="col-6">
                  <p>15:00~21:00</p>
                </div>
                <div class="col-6">
                  <p>????????????</p>
                </div>
                <div class="col-6">
                  <p>10:00??????</p>
                </div>
              </div>
            </div>
          </div>
          <div class="article_facilities mt-5">
            <h3 class="fs-5 pb-2">????????????</h3>
            <ul class="article_icon px-0">
              <li><img src="@/assets/icon/wifi02.png" alt=""><br>
                <p>wifi</p>
              </li>
              <li><img src="@/assets/icon/breakfast02.png" alt=""><br>
                <p>??????</p>
              </li>
              <li><img src="@/assets/icon/minibar01.png" alt=""><br>
                <p class="opacity-25">minibar</p>
              </li>
              <li><img src="@/assets/icon/roomservce01.png" alt=""><br>
                <p class="opacity-25">roomservce</p>
              </li>
              <li><img src="@/assets/icon/phone02.png" alt=""><br>
                <p>??????</p>
              </li>
              <li><img src="@/assets/icon/aircon02.png" alt=""><br>
                <p>??????</p>
              </li>
              <br>
              <li><img src="@/assets/icon/Group02.png" alt=""><br>
                <p>??????</p>
              </li>
              <li><img src="@/assets/icon/sofa01.png" alt=""><br>
                <p class="opacity-25">??????</p>
              </li>
              <li><img src="@/assets/icon/view01.png" alt=""><br>
                <p class="opacity-25">View</p>
              </li>
              <li><img src="@/assets/icon/smoke02.png" alt=""><br>
                <p>????????????</p>
              </li>
              <li><img src="@/assets/icon/children01.png" alt=""><br>
                <p class="opacity-25">????????????</p>
              </li>
              <li><img src="@/assets/icon/dog02.png" alt=""><br>
                <p>????????????</p>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-5">
        <div class="aside mt-5 pt-5">
          <div class="aside_seasonPrice pb-3 d-flex justify-content-around">
            <div class="left">
              <span class="text-info aside_seasonPrice_span">??????(???????????????)</span><br>
              <p class="fs-5 aside_seasonPrice_p "><span class="fs-3">$2,888</span>/???</p>
            </div>
            <div class="right">
              <span class="text-info aside_seasonPrice_span">??????(???????????????)</span><br>
              <p class="fs-5 aside_seasonPrice_p "><span class="fs-3">$3,000</span>/???</p>
            </div>
          </div>
          <form class="form_shadow needs-validation" novalidate>
            <div class="aside_form container gx-5 text-info">
              <label class="pt-5 form-label" for="validationTooltip01">??????</label>
              <input type="text" id="validationTooltip01" class="w-100 bg-success border-0 mb-2" style="height:40px"
                required>
              <div class="valid-tooltip">
                Looks good!
              </div>
              <label for="validationTooltip02">????????????</label>
              <input id="validationTooltip02" type="text" class="w-100 bg-success border-0 mb-2" style="height:40px">
              <label for="">E-mail</label>
              <input type="text" class="w-100 bg-success border-0 mb-2" style="height:40px">
              <div class="aside_date d-flex flex-wrap mb-4 justify-content-between">
                <div class="aside_checkin" style="width: 45%;">
                  <label for="validationTooltip03">????????????</label>
                  <input id="validationTooltip03" class="w-100 bg-success border-0" type="date" style="height:40px">
                </div>
                <div class="aside_checkout" style="width: 45%;">
                  <label for="validationTooltip04">????????????</label>
                  <input id="validationTooltip04" class="w-100 bg-success border-0" type="date" style="height:40px">
                </div>
              </div>
              <button type="submit" class="primaryBtn mb-3 aside_form_btn"
                @click="$refs.reservematerialModal.showModal()">????????????</button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
  <reservematerialModal ref="reservematerialModal" @click="checkRoom($event)"></reservematerialModal>
  <CheckMaterialModal ref="CheckMaterialModal"></CheckMaterialModal>
  <CommentReview_md ref="CommentReview_md"></CommentReview_md>
</template>

<script>
import reservematerialModal from '../components/ReservematerialModal.vue';
import CheckMaterialModal from '../components/CheckMaterialModal.vue';
import CommentReview_md from '../components/CommentReview_md.vue';

export default {
  data() {
    return {
      isIntroduction :false,
      isEvaluation :true,
    }
  },
  methods: {
    checkIntroduction() {
      this.isIntroduction = false
      this.isEvaluation = true
    },
    checkEvaluation() {
      this.isIntroduction = true
      this.isEvaluation = false
    },
    reservematerial() {
      this.$router.push('/checkout/reservematerial');
    },
    checkRoom(e) {
      console.log(123);
      console.log(e.target.innerText === "????????????");
      if ( e.target.innerText === "????????????" ) {
        this.$refs.reservematerialModal.hideModal();
        this.$refs.CheckMaterialModal.showModal();
      }
    },
    openCommentModal() {
      this.$refs.CommentReview_md.showModal();
    }
  },
  components:{
    reservematerialModal,
    CheckMaterialModal,
    CommentReview_md
  },
  created() {
  }
}
</script>