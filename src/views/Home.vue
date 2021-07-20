<template>
  <div>
    <div class="lookbook-container">
      <div class="loading" v-if="isLoading">
        <img lazyload src="../assets/img/logo-comuna.png" />
        <progress-bar
          class="loadingBar"
          bar-color="#fff"
          bg-color="#e40524"
          text-fg-color="#fff"
          size="medium"
          :val="increasing_pct"
          :text="increasing_pct + '%'"
        />
      </div>
      <div class="instructions" v-show="isCover">
        <p>Para una mejor experiencia, navega con los botones</p>
        <div class="instructions_page-btn">
          <img src="../assets/img/up-arrow.png" alt="" />
          <img src="../assets/img/arrow-down.png" alt="" />
        </div>
        <button class="instructions_btn" @click="isCover = !isCover">
          Empezar a navegar
        </button>
      </div>
      <div class="page-btn">
        <a :href="'#section0' + currentStep" @click="Prev" :class="[currentStep == '1' ? 'disabled' : '' ]">
          <img src="../assets/img/up-arrow.png" alt=""
        /></a>
        <a :href="'#section0' + currentStep" @click="Next" :class="[currentStep == '14' ? 'disabled' : '' ]">
          <img src="../assets/img/arrow-down.png" alt=""
        /></a>
      </div>
      <progress-bar
          class="bar-progress"
          bar-color="#e40524"
          bg-color="#fff"
          :val="currentStep * 7.2"
        />
      <span class="bricsa-square"></span>
      <div class="section section01-container" id="section01">
        <img lazyload class="section-bg" src="../assets/img/01.jpg" />
        <div class="section-01">
          <img
            lazyload
            class="section-logo"
            src="../assets/img/logo-comuna.png"
          />
          <p class="call">
            Vívelo por <br />
            dentro y<br />
            por fuera
          </p>
          <p class="downgrade">
            Sal a vivir tu <br />
            nuevo departamento.
          </p>
          <p class="uptext">Vívelo</p>
        </div>
      </div>
      <div class="section section02-container" id="section02">
        <video
          muted
          playsinline
          autoplay
          loop
          preload="auto"
          class="section-bg"
        >
          <source src="../assets/img/video01.mp4" type="video/mp4" />
        </video>
        <div class="section-02">
          <img src="../assets/img/02.jpg" />
          <p class="title">Date una vuelta y respira</p>
          <p v-scrollanimation class="subtitle">
            ¡Está rodeado de áreas verdes!
          </p>
        </div>
      </div>
      <div class="section section03-container" id="section03">
        <img
          v-scrollanimation
          lazyload
          class="section-bg"
          src="../assets/img/03.jpg"
          alt=""
        />
        <div class="disfruta_container">
          <img
            v-scrollanimation
            lazyload
            class="disfruta"
            src="../assets/img/disfruta.png"
          />
        </div>
        <div class="section-bg02_container">
          <img
            v-scrollanimation
            lazyload
            class="section-bg02"
            src="../assets/img/04.jpg"
            alt=""
          />
        </div>
        <div class="section-03">
          <p class="title">
            Disfruta <br />
            tu terraza <br />y tu plaza
          </p>
          <div class="subtitle_container">
            <p v-scrollanimation class="subtitle">
              Depto. con opción a terraza privada.
            </p>
          </div>
          <div class="subtitle02_container">
            <p v-scrollanimation class="subtitle02">
              Frente a Plaza Zañartu y cercano a otros parques.
            </p>
          </div>
        </div>
      </div>
      <div class="section section05-container" id="section04">
        <div class="section-bg_container">
          <img
            v-scrollanimation
            lazyload
            class="section-bg"
            src="../assets/img/05.jpg"
          />
        </div>
        <div class="section-05">
          <div class="title_container">
            <p v-scrollanimation class="title">
              ¡Siempre algo <br />
              que hacer!
            </p>
          </div>
          <div class="subtitle_container">
            <p v-scrollanimation class="subtitle">
              Múltiples espacios <br />
              y áreas comunes.
            </p>
          </div>
          <div class="imgcut_container">
            <img
              v-scrollanimation
              lazyload
              class="imgcut"
              src="../assets/img/06.jpg"
            />
          </div>
        </div>
      </div>
      <div class="section section06-container" id="section05">
        <div class="section-06">
          <img lazyload class="imgtop" src="../assets/img/20.jpg" />
          <div class="title_container">
            <p v-scrollanimation class="title">
              ¡Que rico <br />
              <strong>vivir así!</strong>
            </p>
          </div>
          <div class="subtitle_container">
            <p v-scrollanimation class="subtitle">
              Salón lounge<br />
              para lucirte con<br />
              tus amigos.
            </p>
          </div>
          <div class="imgbottom_container">
            <img
              v-scrollanimation
              lazyload
              class="imgbottom"
              src="../assets/img/08.jpg"
            />
          </div>
        </div>
      </div>
      <div class="section section07-container" id="section06">
        <div class="sectionbg_container">
          <img
            v-scrollanimation
            lazyload
            class="section-bg"
            src="../assets/img/4.jpg"
          />
        </div>
        <div class="section-07">
          <div class="title_container">
            <p v-scrollanimation class="title">El espacio perfecto</p>
          </div>
          <div class="subtitle_container">
            <p v-scrollanimation class="subtitle">
              para <br />
              ser tú
            </p>
          </div>
          <div class="imgcut_container">
            <img
              v-scrollanimation
              lazyload
              class="imgcut"
              src="../assets/img/10.jpg"
            />
          </div>
          <div class="downgrade_container">
            <p v-scrollanimation class="downgrade">
              Diseño Flexible a la medida<br />
              de cómo quieras vivir.
            </p>
          </div>
        </div>
      </div>
      <div class="section section08-container" id="section07">
        <div class="sectionbg_container">
          <img
            v-scrollanimation
            lazyload
            class="section-bg"
            src="../assets/img/11.jpg"
          />
        </div>
        <div class="sectionbg02_container">
          <img
            v-scrollanimation
            lazyload
            class="section-bg02"
            src="../assets/img/12.jpg"
          />
        </div>
        <div class="section-08">
          <div class="title01_container">
            <p v-scrollanimation class="title">
              ¿Quedarse<br />
              en cama?<br />
              ¡Buena idea!
            </p>
          </div>
          <div class="title02_container">
            <p v-scrollanimation class="title02">
              Un picoteo<br />
              ¡y a relajarse!
            </p>
          </div>
          <div class="subtitle01_container">
            <p v-scrollanimation class="subtitle">
              Ventanas termopanel con<br />
              marco PVC (aislación térmica<br />
              y acústica).
            </p>
          </div>
          <div class="subtitle02_container">
            <p v-scrollanimation class="subtitle02">
              Cocina abierta y conectada<br />
              con el living.
            </p>
          </div>
        </div>
      </div>
      <div class="section section10-container" id="section08">
        <div class="sectionbg-container">
          <img
            v-scrollanimation
            lazyload
            class="section-bg"
            src="../assets/img/13.jpg"
          />
        </div>
        <div class="section-10">
          <div class="title_container">
            <p v-scrollanimation class="title">
              Muévete<br />
              indoor o<br />
              outdoor
            </p>
          </div>
          <div class="subtitle_container">
            <p v-scrollanimation class="subtitle">
              Gimnasio interior<br />
              con salida al jardín.
            </p>
          </div>
        </div>
      </div>
      <div class="section section11-container" id="section09">
        <video
          muted
          playsinline
          autoplay
          loop
          preload="auto"
          class="section-bg"
        >
          <source src="../assets/img/video02.mp4" type="video/mp4" />
        </video>
        <div class="section-11">
          <div class="title_container">
            <p v-scrollanimation class="title">Así da gusto</p>
          </div>
          <div class="subtitle_container">
            <p v-scrollanimation class="subtitle">trabajar</p>
          </div>
          <div class="downgrade_container">
            <p v-scrollanimation class="downgrade">Zonas Cowork.</p>
          </div>
          <div class="section11-img_container">
            <img
            lazyload
              v-scrollanimation
              class="section-11__img01"
              src="../assets/img/08.jpg"
            />
          </div>
          <img lazyload class="section-11__img02" src="../assets/img/14.jpg" />
        </div>
      </div>
      <div class="section section12-container" id="section010">
        <div class="sectionbg_container">
          <img
            v-scrollanimation
            lazyload
            class="section-bg"
            src="../assets/img/15.jpg"
          />
        </div>
        <div class="section-12">
          <div class="title_container">
            <p v-scrollanimation class="title">
              Recibe<br />
              lo que quieras
            </p>
          </div>
          <div class="subtitle_container">
            <p v-scrollanimation class="subtitle">tranquilo</p>
          </div>
          <div class="downgrade_container">
            <p v-scrollanimation class="downgrade">Smart lockers.</p>
          </div>
        </div>
      </div>
      <div class="section section13-container" id="section011">
        <div class="sectionbg_container">
          <img
            v-scrollanimation
            lazyload
            class="section-bg"
            src="../assets/img/16.jpg"
          />
        </div>
        <div class="section-13">
          <div class="entorno_container">
            <img
              v-scrollanimation
              lazyload
              class="entorno"
              src="../assets/img/entorno.png"
            />
          </div>
          <p class="title">¡Mantengamos viva</p>
          <p class="subtitle">la vida de barrio!</p>
          <div class="downgrade_container">
            <p v-scrollanimation class="downgrade">
              Ubicado en un barrio tradicional de Ñuñoa, cercano a todo lo que
              necesitas.
            </p>
          </div>
          <img lazyload class="fachada" src="../assets/img/17.jpg" />
        </div>
      </div>
      <div class="section section14-container" id="section012">
        <video
          muted
          playsinline
          autoplay
          loop
          preload="auto"
          class="section-bg"
        >
          <source src="../assets/img/video03.mp4" type="video/mp4" />
        </video>
        <div v-scrollanimation class="section-14">
          <img lazyload class="section-14__img01" src="../assets/img/11.jpg" />
          <p class="title">
            Vívelo<br />
            por dentro<br />
            y por fuera
          </p>
          <p class="subtitle">
            La llave para comenzar<br />
            a disfrutarlo<br />
            la tienes tú.
          </p>
          <img lazyload class="section-14__img02" src="../assets/img/18.jpg" />
          <img lazyload class="section-14__img03" src="../assets/img/19.jpg" />
        </div>
      </div>
      <div class="section section15-container" id="section013">
        <video
          autoplay
          muted
          loop
          playsinline
          preload="auto"
          class="section-bg"
        >
          <source src="../assets/img/video04.mp4" type="video/mp4" />
        </video>
        <img lazyload src="../assets/img/logo-comuna.png" />
      </div>
      <div class="section section16-container" id="section014">
        <div class="section-16">
          <img lazyload class="logo" src="../assets/img/bricsa.png" />

          <img lazyload class="bptl" src="../assets/img/bptl.png" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ProgressBar from "vue-simple-progress";
export default {
  components: {
    ProgressBar,
  },
  data() {
    return {
      currentStep: "1",
      isLoading: true,
      increasing_pct: 0,
      isCover: true,
    };
  },
  methods: {
    load() {
      this.isLoading = true;
      setTimeout(() => {
        this.isLoading = false;
      }, 5000);
    },
    Prev() {
      this.currentStep--;
    },
    Next() {
      this.currentStep++;
    },
  },
  created() {
    this.load();
    setInterval(() => {
      if (this.is_paused) return;

      this.increasing_pct = Math.min(this.increasing_pct + 1, 100);
    }, 23);
  },
};
</script>

<style lang="scss" scoped>
.lookbook-container {
  position: relative;
  overflow: hidden;
  height: 100vh;
}
.section {
  position: relative;
  overflow: hidden;
  min-height: 101vh;
}

.bricsa-square {
  display: block;
  position: fixed;
  right: 0;
  top: 20px;
  width: 50px;
  height: 50px;
  background: #e40524;
  z-index: 99;
}
@keyframes breath {
  0% {
    transform: scale(0.9);
  }
  100% {
    transform: scale(1);
  }
}
.loading {
  transition: all 1s both;
  background: #e40524;
  z-index: 100;
  position: absolute;
  display: grid;
  grid-template-rows: repeat(2, min-content);
  row-gap: 20px;
  justify-content: center;
  justify-items: center;
  align-items: center;
  align-content: center;
  width: 100%;
  height: 100vh;
  img {
    animation: breath 1s both infinite alternate-reverse;
    width: 40%;
  }
  .loadingBar {
    width: 60%;
  }
}

.instructions {
  background: #e40524;
  position: relative;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  display: grid;
  justify-content: center;
  justify-items: center;
  align-content: center;
  align-items: center;
  row-gap: 30px;
  z-index: 14;
  p {
    color: #fff;
    font-size: 26px;
    width: 90%;
    text-align: center;
    font-weight: 300;
    margin: 0;
  }
  .instructions_page-btn {
    width: 50px;
    display: grid;
    justify-items: center;
    align-items: center;
    position: relative;
    border: solid 1px #fff;
    img {
      width: 70%;
      padding: 5px;
      border: none;
      background: #e40524;
    }
  }
  .instructions_btn {
    color: #fff;
    background: rgba(0, 0, 0, 0);
    border: solid 2px #fff;
    border-radius: 10px;
    padding: 10px;
    cursor: pointer;
    transition: 400ms;
    &:hover {
      background: #b9041c;
    }
  }
}
@keyframes arrow-down {
  0% {
    margin-top: 0;
  }
  100% {
    margin-top: 10px;
  }
}

.page-btn {
  z-index: 13;
  position: fixed;
  bottom: 0;
  right: 0;
  display: grid;
  a {
    width: 30px;
    height: 30px;
    padding: 10px;
    border: none;
    background: #e40524;
    cursor: pointer;
    transition: 400ms;
    &:hover {
      background: #b9041c;
    }
    img {
      width: 100%;
    }
  }
  .disabled{
    pointer-events: none;
  }
}

.bar-progress{
  width: 100%;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 13;
}

.section-bg {
  height: 100%;
  object-fit: cover;
  position: absolute;
  z-index: -1;
  left: -100%;
}
.section01-container {
  .section-bg {
    animation-name: section01-bg;
    animation-duration: 3s;
    animation-direction: normal;
    animation-fill-mode: both;
    left: -100%;
  }
  @keyframes section01-bg {
    0% {
      left: 0;
    }
    100% {
      left: -100%;
    }
  }
  .section-01 {
    background: rgba(0, 0, 0, 0.3);
    width: 100%;
    height: 100%;
    position: absolute;
    display: block;
    top: 0;
    left: 0;
    z-index: 1;
    .section-logo {
      width: 100px;
      position: absolute;
      top: 50px;
      left: 20px;
    }
    .call {
      transition: all 400ms;
      text-align: left;
      width: 70%;
      color: #fff;
      font-size: 60px;
      font-weight: bolder;
      line-height: 0.8;
      position: absolute;
      bottom: 36%;
      left: 20px;
    }
    .downgrade {
      text-align: left;
      width: 69%;
      color: #fff;
      font-size: 30px;
      font-weight: 300;
      line-height: 0.8;
      position: absolute;
      bottom: 25%;
      left: 20px;
    }
    .uptext {
      animation-name: uptext;
      animation-duration: 3s;
      animation-fill-mode: both;
      transform: rotate(-90deg);
      font-size: 180px;
      position: absolute;
      right: -200px;
      margin: 0;
      font-weight: bolder;
      color: #fff;
      top: 100%;
    }
    @keyframes uptext {
      0% {
        top: 100%;
      }
      100% {
        top: 20%;
      }
    }
  }
}
.section02-container {
  position: relative;

  .section-02 {
    position: absolute;
    width: 80%;
    height: 75%;
    left: 10%;
    top: 13.5%;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      filter: brightness(0.7);
    }
    .title {
      position: absolute;
      color: #fff;
      width: 100%;
      font-size: 70px;
      text-align: center;
      bottom: 30%;
      font-weight: 800;
      line-height: 0.9;
    }
    .subtitle {
      transition: all ease-in-out;
      transition-duration: 2s;
      bottom: -100%;
      opacity: 0;
      color: #fff;
      width: 100%;
      font-weight: 300;
      font-size: 40px;
      text-align: center;
      line-height: 1;
    }
    .enter {
      position: absolute;
      color: #fff;
      width: 100%;
      font-size: 40px;
      text-align: center;
      line-height: 1;
      bottom: 0;
      opacity: 1;
    }
  }
}
.section03-container {
  .section-bg {
    position: absolute;
    z-index: 3;
    transition: all 6s ease-in-out 1s;
    left: 0;
  }
  .enter {
    left: -300%;
  }
  .disfruta_container {
    .disfruta {
      transition: all 5s ease-in-out 4s;
      position: absolute;
      top: 0;
      left: 50%;
      z-index: 2;
    }
    .enter {
      left: -140%;
    }
  }
  .section-bg02_container {
    .section-bg02 {
      position: absolute;
      transition: all 3s ease-in-out 4s;
      z-index: 1;
      height: 100vh;
      left: 0;
    }
    .enter {
      left: -100%;
    }
  }
  .section-03 {
    background: rgba($color: #000000, $alpha: 0.3);
    width: 100%;
    height: 100%;
    position: absolute;
    display: block;
    top: 0;
    left: 0;
    z-index: 3;
    display: grid;
    align-items: center;
    justify-content: center;
    .title {
      position: absolute;
      color: #fff;
      width: 80%;
      font-size: 60px;
      text-align: center;
      bottom: 32%;
      left: 10%;
      font-weight: 800;
      line-height: 0.9;
      z-index: 3;
    }
    .subtitle_container {
      .subtitle {
        position: absolute;
        color: #fff;
        width: 80%;
        font-size: 30px;
        font-weight: 300;
        text-align: center;
        bottom: 20%;
        left: 10%;
        line-height: 1;
        z-index: 3;
        transition: all 4s ease-in-out 2s;
      }
      .enter {
        left: -100%;
      }
    }
    .subtitle02_container {
      .subtitle02 {
        position: absolute;
        color: #fff;
        width: 80%;
        font-size: 30px;
        font-weight: 300;
        text-align: center;
        bottom: 20%;
        left: 100%;
        line-height: 1;
        z-index: 3;
        transition: all 3s ease-in-out 4s;
      }
      .enter {
        left: 10%;
      }
    }
  }
}
.section05-container {
  .section-bg_container {
    .section-bg {
      transition: all 4s ease-in-out;
      height: 100%;
      object-fit: cover;
      position: absolute;
      z-index: -1;
      left: -100%;
    }
    .enter {
      left: -50%;
    }
  }
  .section-05 {
    background: rgba($color: #000000, $alpha: 0.3);
    width: 100%;
    height: 100%;
    position: absolute;
    display: block;
    top: 0;
    left: 0;
    z-index: 1;
    .title_container {
      .title {
        transition: all 1s ease-in-out;
        position: absolute;
        color: #fff;
        width: 90%;
        font-size: 40px;
        text-align: center;
        top: 0;
        opacity: 0;
        left: 5%;
        font-weight: 800;
        line-height: 0.9;
      }
      .enter {
        top: 5% !important;
        opacity: 1;
      }
    }
    .subtitle_container {
      .subtitle {
        transition: all 1s ease-in-out 1s;
        position: absolute;
        color: #fff;
        width: 80%;
        font-size: 30px;
        font-weight: 300;
        text-align: center;
        top: 0;
        opacity: 0;
        left: 10%;
        line-height: 1;
      }
      .enter {
        top: 20% !important;
        opacity: 1;
      }
    }
    .imgcut_container {
      .imgcut {
        transition: all 2.5s ease-in-out 2s;
        filter: brightness(0.7);
        width: 60%;
        height: 55%;
        object-fit: cover;
        object-position: center;
        position: absolute;
        bottom: 0;
        right: -60%;
      }
      .enter {
        right: 0;
      }
    }
  }
}
.section06-container {
  .section-06 {
    .imgtop {
      filter: brightness(0.7);
      height: 45%;
      width: 180%;
      position: absolute;
      top: 0;
      left: 0;
      object-fit: cover;
      object-position: -240px center;
    }
    .imgbottom_container {
      .imgbottom {
        transition: all 3s ease-in-out;
        height: 55%;
        width: 270%;
        position: absolute;
        bottom: 0;
        left: -70%;
        object-fit: cover;
      }
      .enter {
        left: -20%;
      }
    }
    .title_container {
      .title {
        transition: all 2s ease-in-out;
        position: absolute;
        color: #fff;
        width: 90%;
        font-size: 50px;
        text-align: center;
        top: 0;
        left: -80%;
        font-weight: 300;
        line-height: 0.9;
      }
      .enter {
        left: 5%;
      }
    }
    .subtitle_container {
      .subtitle {
        transition: all 2s ease-in-out;
        position: absolute;
        color: #fff;
        width: 80%;
        font-size: 30px;
        font-weight: 300;
        text-align: center;
        top: 20%;
        left: 100%;
        line-height: 1;
      }
      .enter {
        left: 10%;
      }
    }
  }
}
.section07-container {
  .sectionbg_container {
    .section-bg {
      left: -10%;
      transition: all 7s ease-in-out;
    }
    .enter {
      left: -190%;
    }
  }
  .section-07 {
    background: rgba($color: #000000, $alpha: 0.3);
    width: 100%;
    height: 100%;
    position: absolute;
    display: block;
    top: 0;
    left: 0;
    z-index: 1;
    .imgcut_container {
      .imgcut {
        transition: all 2s ease-in-out;
        width: 40%;
        height: 25%;
        object-fit: cover;
        object-position: -100px center;
        position: absolute;
        left: -39%;
        bottom: 25%;
      }
      .enter {
        left: 0;
      }
    }
    .title_container {
      .title {
        transition: all 2s ease-in-out;
        position: absolute;
        color: #fff;
        width: 90%;
        font-size: 30px;
        text-align: center;
        top: 70%;
        left: 5%;
        font-weight: 300;
        line-height: 0.9;
        opacity: 0;
      }
      .enter {
        opacity: 1;
        top: 8%;
      }
    }
    .subtitle_container {
      .subtitle {
        transition: all 2s ease-in-out;
        position: absolute;
        color: #fff;
        width: 80%;
        font-size: 100px;
        font-weight: 800;
        text-align: center;
        top: 70%;
        left: 10%;
        line-height: 1;
        opacity: 0;
      }
      .enter {
        opacity: 1;
        top: 2%;
      }
    }
    .downgrade_container {
      .downgrade {
        transition: all 2s ease-in-out;
        position: absolute;
        color: #fff;
        width: 70%;
        font-size: 23px;
        left: 15%;
        font-weight: 300;
        bottom: 0;
        opacity: 0;
      }
      .enter {
        opacity: 1;
        bottom: 5%;
      }
    }
  }
}
.section08-container {
  .sectionbg_container {
    .section-bg {
      transition: all 6s ease-in-out 1s;
      position: absolute;
      filter: brightness(0.7);
      z-index: 0;
      left: -100%;
    }
    .enter {
      left: 160%;
    }
  }
  .sectionbg02_container {
    .section-bg02 {
      transition: all 6s ease-in-out 6s;
      position: absolute;
      height: 100vh;
      filter: brightness(0.7);
      z-index: -1;
      left: -100%;
    }
    .enter {
      left: -330%;
    }
  }
  .section-08 {
    color: #fff;
    .title01_container {
      .title {
        transition: all 1s ease-in-out 1s;
        position: absolute;
        color: #fff;
        width: 90%;
        font-size: 50px;
        text-align: center;
        bottom: 17%;
        left: 5%;
        font-weight: 800;
        line-height: 0.9;
        filter: blur(20px);
        opacity: 0;
      }
      .enter {
        animation: fade-out 1s both 6s;
        filter: blur(0);
        opacity: 1;
      }
      @keyframes fade-out {
        0% {
          filter: blur(0);
          opacity: 1;
        }
        100% {
          filter: blur(20px);
          opacity: 0;
        }
      }
    }
    .subtitle01_container {
      .subtitle {
        transition: all 1s ease-in-out 1s;
        position: absolute;
        color: #fff;
        width: 80%;
        font-size: 22px;
        font-weight: 300;
        text-align: center;
        bottom: 5%;
        left: 10%;
        line-height: 1;
        opacity: 0;
        filter: blur(20px);
        opacity: 0;
      }
      .enter {
        animation: fade-out 1s both 6s;
        filter: blur(0);
        opacity: 1;
      }
      @keyframes fade-out {
        0% {
          filter: blur(0);
          opacity: 1;
        }
        100% {
          filter: blur(20px);
          opacity: 0;
        }
      }
    }
    .title02_container {
      .title02 {
        transition: all 1s ease-in-out 6s;
        position: absolute;
        color: #fff;
        width: 90%;
        font-size: 40px;
        text-align: center;
        top: 3%;
        left: 5%;
        font-weight: 800;
        line-height: 0.9;
        filter: blur(20px);
        opacity: 0;
      }
      .enter {
        filter: blur(0);
        opacity: 1;
      }
    }
    .subtitle02_container {
      .subtitle02 {
        transition: all 1s ease-in-out 6s;
        position: absolute;
        color: #fff;
        width: 80%;
        font-size: 26px;
        font-weight: 300;
        text-align: center;
        top: 16%;
        left: 10%;
        line-height: 1;
        filter: blur(20px);
        opacity: 0;
      }
      .enter {
        filter: blur(0);
        opacity: 1;
      }
    }
  }
}
.section10-container {
  .sectionbg-container {
    .section-bg {
      transition: all 5s ease-in-out 1s;
      position: absolute;
      height: 100vh;
      filter: brightness(0.7);
      left: -10%;
    }
    .enter {
      left: -120%;
    }
  }
  .section-10 {
    color: #fff;
    .title_container {
      .title {
        transition: all 1s ease-in-out 1s;
        animation: section10_title 1s both 1s;
        position: absolute;
        color: #fff;
        width: 90%;
        font-size: 60px;
        text-align: center;
        top: 3%;
        left: 5%;
        font-weight: 800;
        line-height: 0.9;
        filter: blur(20px);
        opacity: 0;
      }
      .enter {
        filter: blur(0);
        opacity: 1;
      }
    }
    .subtitle_container {
      .subtitle {
        transition: all 1s ease-in-out 1s;
        position: absolute;
        color: #fff;
        width: 80%;
        font-size: 26px;
        font-weight: 300;
        text-align: center;
        bottom: 10%;
        left: 10%;
        line-height: 1;
        filter: blur(20px);
        opacity: 0;
      }
      .enter {
        filter: blur(0);
        opacity: 1;
      }
    }
  }
}
.section11-container {
  .section-bg {
    filter: brightness(0.7);
  }
  .section-11 {
    color: #fff;
    .section-11__img01,
    .section-11__img02 {
      filter: brightness(0.7);
      position: absolute;
      top: 0;
      left: 0;
      object-fit: cover;
      width: 75%;
      height: 90%;
    }
    .section11-img_container {
      .section-11__img01 {
        transition: all 2s ease-in-out 4s;
        z-index: 1;
        left: 0;
      }
      .enter {
        left: -75%;
      }
    }
    .section-11__img02 {
      object-position: 10%;
    }
    .title_container {
      .title {
        transition: all 1s ease-in-out 1s;
        z-index: 2;
        position: absolute;
        width: 80%;
        left: 10%;
        text-align: left;
        bottom: 0%;
        font-size: 50px;
        font-weight: 300;
        opacity: 0;
      }
      .enter {
        bottom: 27%;
        opacity: 1;
      }
    }
    .subtitle_container {
      .subtitle {
        transition: all 1s ease-in-out 1s;
        z-index: 2;
        position: absolute;
        width: 80%;
        left: 10%;
        bottom: -15%;
        font-size: 70px;
        font-weight: 800;
        text-align: right;
        opacity: 0;
      }
      .enter {
        bottom: 15%;
        opacity: 1;
      }
    }
    .downgrade_container {
      .downgrade {
        transition: all 1s ease-in-out 1s;
        z-index: 2;
        position: absolute;
        bottom: 0%;
        font-size: 30px;
        width: 80%;
        left: 10%;
        text-align: center;
        opacity: 0;
      }
      .enter {
        bottom: 16%;
        opacity: 1;
      }
    }
  }
}
.section12-container {
  .sectionbg_container {
    .section-bg {
      transition: all 3s ease-in-out 1s;
      left: -20%;
      object-position: 100%;
      filter: brightness(0.7);
    }
    .enter {
      left: -120%;
    }
  }
  .section-12 {
    color: #fff;
    .title_container {
      .title {
        transition: all 1s ease-in-out 1s;
        animation: section12_title 1s both 1s;
        z-index: 2;
        position: absolute;
        width: 80%;
        left: 10%;
        top: -10%;
        font-size: 50px;
        font-weight: 300;
        opacity: 0;
      }
      .enter {
        top: 0;
        opacity: 1;
      }
    }
    .subtitle_container {
      .subtitle {
        transition: all 1s ease-in-out 1s;
        z-index: 2;
        position: absolute;
        width: 80%;
        left: 10%;
        top: 0%;
        font-size: 70px;
        font-weight: 800;
        opacity: 0;
      }
      .enter {
        top: 13%;
        opacity: 1;
      }
    }
    .downgrade_container {
      .downgrade {
        transition: all 1s ease-in-out 1s;
        z-index: 2;
        position: absolute;
        top: 0%;
        font-size: 30px;
        width: 80%;
        left: 10%;
        font-weight: 300;
        opacity: 0;
      }
      .enter {
        top: 30%;
        opacity: 1;
      }
    }
  }
}
.section13-container {
  .sectionbg_container {
    .section-bg {
      transition: all 3s ease-in-out 1s;
      position: absolute;
      height: 100%;
      filter: brightness(0.7);
      left: -100%;
    }
    .enter {
      left: -70%;
    }
  }
  .section-13 {
    color: #fff;
    .entorno_container {
      .entorno {
        transition: all 4s ease-in-out;
        height: 150px;
        position: absolute;
        top: 1%;
        left: 80%;
      }
      .enter {
        left: -100%;
      }
    }
    .title {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 10%;
      bottom: 66%;
      font-size: 40px;
      font-weight: 300;
    }
    .subtitle {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 10%;
      bottom: 53%;
      font-size: 50px;
      font-weight: 800;
      line-height: 0.9;
    }
    .downgrade_container {
      .downgrade {
        transition: all 1s ease-in-out 1s;
        z-index: 2;
        position: absolute;
        bottom: 39%;
        font-size: 22px;
        width: 80%;
        left: 10%;
        font-weight: 300;
        filter: blur(100px);
        opacity: 0;
      }
      .enter {
        filter: blur(0);
        opacity: 1;
      }
    }
    .fachada {
      position: absolute;
      bottom: 3%;
      left: 10%;
      width: 80%;
      height: 30%;
      object-fit: cover;
      object-position: bottom;
    }
  }
}
.section14-container {
  .section-bg {
    filter: brightness(1);
  }
  .section-14 {
    transition: all 1s ease-in-out 1s;
    color: #fff;
    position: absolute;
    width: 100%;
    height: 100%;
    top: 90%;
    left: 0;
    opacity: 0;
    .section-14__img01 {
      z-index: 2;
      filter: brightness(0.7);
      width: 60%;
      height: 30%;
      object-fit: cover;
      position: absolute;
      top: 0;
      right: 10%;
    }
    .section-14__img02 {
      filter: brightness(0.7);
      position: absolute;
      width: 70%;
      height: 80%;
      object-fit: cover;
      left: 15%;
      top: 10%;
    }
    .section-14__img03 {
      z-index: 2;
      width: 60%;
      height: 30%;
      object-fit: cover;
      position: absolute;
      bottom: 0;
      left: 10%;
    }
    .title {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 20%;
      text-align: left;
      top: 28%;
      font-size: 50px;
      font-weight: 800;
      line-height: 1;
    }
    .subtitle {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 20%;
      top: 55%;
      font-size: 20px;
      text-align: left;
      font-weight: 300;
    }
  }
  .enter {
    top: 0;
    opacity: 1;
  }
}
.section14-container {
  .section-bg {
    filter: brightness(1);
  }
  .section-14 {
    color: #fff;
    position: absolute;
    width: 100%;
    height: 100%;
    top: 90%;
    left: 0;
    opacity: 0;
    .section-14__img01 {
      z-index: 2;
      filter: brightness(0.7);
      width: 60%;
      height: 30%;
      object-fit: cover;
      position: absolute;
      top: 0;
      right: 10%;
    }
    .section-14__img02 {
      filter: brightness(0.7);
      position: absolute;
      width: 70%;
      height: 80%;
      object-fit: cover;
      left: 15%;
      top: 10%;
    }
    .section-14__img03 {
      z-index: 2;
      width: 60%;
      height: 30%;
      object-fit: cover;
      position: absolute;
      bottom: 0;
      left: 10%;
    }
    .title {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 20%;
      text-align: left;
      top: 28%;
      font-size: 50px;
      font-weight: 800;
      line-height: 1;
    }
    .subtitle {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 20%;
      top: 55%;
      font-size: 20px;
      text-align: left;
      font-weight: 300;
    }
  }
  .enter {
    top: 0;
    opacity: 1;
  }
}
.section15-container {
  .section-bg {
    height: 100vh;
  }
  img {
    width: 40%;
    position: absolute;
    left: 30%;
    bottom: 20%;
  }
}
.section16-container {
  background: #e40524;
  display: flex;
  .section-16 {
    display: grid;
    height: 100%;
    grid-template-columns: 100%;
    grid-template-rows: repeat(2, min-content);
    row-gap: 30px;
    justify-content: center;
    justify-items: center;
    align-items: center;
    align-content: center;
    align-self: center;
    .logo {
      width: 60%;
    }
    .bptl {
      width: 40%;
    }
  }
}

@media screen and (max-width: 426px) {
  .section01-container {
    .section-01 {
      .call {
        font-size: 50px;
        bottom: 40%;
      }
      #section1_vivelo {
        font-size: 150px;
        right: -160px;
      }
    }
  }
  .section02-container {
    .section-02 {
      .title {
        font-size: 50px;
      }
    }
  }
  .section03-container {
    .section-03 {
      .title {
        font-size: 40px;
      }
      .subtitle {
        font-size: 25px;
        bottom: 15%;
      }
      .subtitle02 {
        font-size: 25px;
        bottom: 15%;
      }
    }
  }
  .section08-container {
    .section-08 {
      .subtitle02 {
        top: 18%;
      }
    }
  }
  .section13-container {
    .section-13 {
      .title {
        font-size: 38px;
      }
      .subtitle {
        font-size: 40px;
      }
    }
  }
}
@media screen and (max-width: 321px) {
  .section01-container {
    .section-01 {
      .call {
        font-size: 40px;
      }
      #section1_vivelo {
        font-size: 150px;
        right: -160px;
      }
    }
  }
  .section02-container {
    .section-02 {
      .subtitle {
        font-size: 30px;
      }
    }
  }
  .section05-container {
    .section-05 {
      .subtitle {
        top: 21%;
      }
    }
  }
  .section06-container {
    .section-06 {
      .subtitle {
        font-size: 26px;
        top: 23%;
      }
    }
  }
  .section07-container {
    .section-07 {
      .subtitle {
        font-size: 80px;
      }
    }
  }
  .section12-container {
    .section-12 {
      .subtitle {
        font-size: 50px;
      }
    }
  }
  .section13-container {
    .section-13 {
      .title {
        font-size: 32px;
        bottom: 63%;
      }
      .subtitle {
        font-size: 33px;
        bottom: 55%;
      }
      .downgrade {
        font-size: 20px !important;
        width: 90% !important;
        left: 5% !important;
      }
    }
  }
}
</style>
