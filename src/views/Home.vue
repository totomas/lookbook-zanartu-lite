<template>
  <div>
    <full-page ref="fullpage" :options="options" id="fullpage">
      <div class="section">
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
          <img
            lazyload
            class="arrow-down"
            src="../assets/img/arrow-down.png"
            alt=""
          />
        </div>
      </div>
      <div class="section">
        <span class="bricsa-square"></span>
        <video autoplay class="section-bg">
          <source src="../assets/img/video01.mp4" type="video/mp4" />
        </video>
        <div class="section-02">
          <img src="../assets/img/02.jpg" />
          <p class="title">Date una vuelta y respira</p>
          <p class="subtitle">¡Está rodeado de áreas verdes!</p>
        </div>
      </div>
      <div class="section">
        <span class="bricsa-square"></span>
        <img lazyload class="section-bg" src="../assets/img/03.jpg" alt="" />
        <div class="section-03">
          <p class="title">
            Disfruta <br />
            tu terraza <br />y tu plaza
          </p>
          <p class="subtitle">Depto. con opción a terraza privada.</p>
        </div>
      </div>
      <div class="section">
        <span class="bricsa-square"></span>
        <img lazyload class="section-bg" src="../assets/img/04.jpg" alt="" />
        <div class="section-04">
          <img lazyload class="disfruta" src="../assets/img/disfruta.png" />
          <p class="title">
            Disfruta <br />
            tu terraza <br />y tu plaza
          </p>
          <p class="subtitle">
            Frente a Plaza Zañartu y cercano a otros parques.
          </p>
        </div>
      </div>
      <div class="section">
        <span class="bricsa-square"></span>
        <img lazyload class="section-bg" src="../assets/img/05.jpg" />
        <div class="section-05">
          <p class="title">
            ¡Siempre algo <br />
            que hacer!
          </p>
          <p class="subtitle">
            Múltiples espacios <br />
            y áreas comunes.
          </p>
          <img lazyload class="imgcut" src="../assets/img/06.jpg" />
        </div>
      </div>
      <div class="section">
        <span class="bricsa-square"></span>
        <div class="section-06">
          <img lazyload class="imgtop" src="../assets/img/20.jpg" />
          <p class="title">
            ¡Que rico <br />
            <strong>vivir así!</strong>
          </p>
          <p class="subtitle">
            Salón lounge<br />
            para lucirte con<br />
            tus amigos.
          </p>
          <img lazyload class="imgbottom" src="../assets/img/08.jpg" />
        </div>
      </div>
      <div class="section section07-container">
        <span class="bricsa-square"></span>
        <img lazyload class="section-bg" src="../assets/img/4.jpg" />
        <div class="section-07">
          <p class="title">El espacio perfecto</p>
          <p class="subtitle">
            para <br />
            ser tú
          </p>
          <img lazyload class="imgcut" src="../assets/img/10.jpg" />
          <p class="downgrade">
            Diseño Flexible a la medida<br />
            de cómo quieras vivir.
          </p>
        </div>
      </div>
      <div class="section section08-container">
        <span class="bricsa-square"></span>
        <img lazyload class="section-bg" src="../assets/img/11.jpg" />
        <div class="section-08">
          <p class="title">
            ¿Quedarse<br />
            en cama?<br />
            ¡Buena idea!
          </p>
          <p class="subtitle">
            Ventanas termopanel con<br />
            marco PVC (aislación térmica<br />
            y acústica).
          </p>
        </div>
      </div>
      <div class="section section09-container">
        <span class="bricsa-square"></span>
        <img lazyload class="section-bg" src="../assets/img/12.jpg" />
        <div class="section-09">
          <p class="title">
            Un picoteo<br />
            ¡y a relajarse!
          </p>
          <p class="subtitle">
            Cocina abierta y conectada<br />
            con el living.
          </p>
        </div>
      </div>
      <div class="section section10-container">
        <span class="bricsa-square"></span>
        <img lazyload class="section-bg" src="../assets/img/13.jpg" />
        <div class="section-10">
          <p class="title">
            Muévete<br />
            indoor o<br />
            outdoor
          </p>
          <p class="subtitle">
            Gimnasio interior<br />
            con salida al jardín.
          </p>
        </div>
      </div>
      <div class="section section11-container">
        <span class="bricsa-square"></span>
        <video autoplay class="section-bg">
          <source src="../assets/img/video02.mp4" type="video/mp4" />
        </video>
        <div class="section-11">
          <p class="title">Así da gusto</p>
          <p class="subtitle">trabajar</p>
          <p class="downgrade">Zonas Cowork.</p>
          <img class="section-11__img01" src="../assets/img/08.jpg" />
          <img class="section-11__img02" src="../assets/img/14.jpg" />
        </div>
      </div>
      <div class="section section12-container">
        <span class="bricsa-square"></span>
        <img lazyload class="section-bg" src="../assets/img/15.jpg" />
        <div class="section-12">
          <p class="title">
            Recibe<br />
            lo que quieras
          </p>
          <p class="subtitle">tranquilo</p>
          <p class="downgrade">Smart lockers.</p>
        </div>
      </div>
      <div class="section section13-container">
        <span class="bricsa-square"></span>
        <img lazyload class="section-bg" src="../assets/img/16.jpg" />
        <div class="section-13">
          <img lazyload class="entorno" src="../assets/img/entorno.png" />
          <p class="title">¡Mantengamos viva</p>
          <p class="subtitle">
            la vida de<br />
            barrio!
          </p>
          <p class="downgrade">
            Ubicado en un barrio<br />
            tradicional de Ñuñoa, cercano<br />
            a todo lo que necesitas.
          </p>
          <img lazyload class="fachada" src="../assets/img/17.jpg" />
        </div>
      </div>
      <div class="section section14-container">
        <span class="bricsa-square"></span>
        <video autoplay class="section-bg">
          <source src="../assets/img/video03.mp4" type="video/mp4" />
        </video>
        <div class="section-14">
          <img class="section-14__img01" src="../assets/img/11.jpg" />
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
          <img class="section-14__img02" src="../assets/img/18.jpg" />
          <img class="section-14__img03" src="../assets/img/19.jpg" />
        </div>
      </div>
      <div class="section section15-container">
        <div class="section-15">
          <img lazyload class="logo" src="../assets/img/bricsa.png" />

          <img lazyload class="bptl" src="../assets/img/bptl.png" />
        </div>
      </div>
    </full-page>
  </div>
</template>

<script>
import Vue from "vue";
import VueFullPage from "vue-fullpage.js";

Vue.use(VueFullPage);
export default {
  data() {
    return {
      options: {
        licenseKey: "YOUR_KEY_HEERE",
        menu: "#menu",
        anchors: [
          "page1",
          "page2",
          "page3",
          "page4",
          "page5",
          "page6",
          "page7",
          "page8",
          "page9",
          "page10",
          "page11",
          "page12",
          "page13",
          "page14",
          "page15",
          "page16",
        ],
      },
    };
  },
};
</script>

<style lang="scss" scoped>
.section {
  position: relative;
}

.bricsa-square {
  position: absolute;
  right: 0;
  top: 3%;
  width: 50px;
  height: 50px;
  background: #e40524;
  z-index: 2;
}

.section-bg {
  height: 100%;
  object-fit: cover;
  position: absolute;
  z-index: -1;
  left: -100%;
}
.section-01 {
  background: rgba($color: #000000, $alpha: 0.3);
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
    text-align: left;
    width: 70%;
    color: #fff;
    font-size: 60px;
    font-weight: bolder;
    line-height: 0.8;
    position: absolute;
    bottom: 30%;
    left: 20px;
  }
  .downgrade {
    text-align: left;
    width: 70%;
    color: #fff;
    font-size: 30px;
    font-weight: 300;
    line-height: 0.8;
    position: absolute;
    bottom: 25%;
    left: 20px;
  }
  .uptext {
    transform: rotate(-90deg);
    font-size: 230px;
    position: absolute;
    right: -250px;
    bottom: 170px;
    margin: 0;
    font-weight: bolder;
    color: #fff;
  }
  .arrow-down {
    width: 100px;
    position: absolute;
    margin: 0 auto;
    left: 150px;
    bottom: 20px;
  }
}
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
    bottom: 13%;
    font-weight: 800;
    line-height: 0.9;
  }
  .subtitle {
    position: absolute;
    color: #fff;
    width: 100%;
    font-size: 40px;
    text-align: center;
    bottom: 0;
    line-height: 1;
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
  z-index: 1;
  display: grid;
  align-items: center;
  justify-content: center;
  .title {
    position: absolute;
    color: #fff;
    width: 80%;
    font-size: 70px;
    text-align: center;
    bottom: 30%;
    left: 10%;
    font-weight: 800;
    line-height: 0.9;
  }
  .subtitle {
    position: absolute;
    color: #fff;
    width: 80%;
    font-size: 40px;
    font-weight: 400;
    text-align: center;
    bottom: 20%;
    left: 10%;
    line-height: 1;
  }
}
.section-04 {
  background: rgba($color: #000000, $alpha: 0.3);
  width: 100%;
  height: 100%;
  position: absolute;
  display: block;
  top: 0;
  left: 0;
  z-index: 1;
  display: grid;
  align-items: center;
  justify-content: center;
  .disfruta {
    height: 200px;
    position: absolute;
    right: -120%;
    top: 5%;
  }
  .title {
    position: absolute;
    color: #fff;
    width: 80%;
    font-size: 70px;
    text-align: center;
    bottom: 30%;
    left: 10%;
    font-weight: 800;
    line-height: 0.9;
  }
  .subtitle {
    position: absolute;
    color: #fff;
    width: 80%;
    font-size: 30px;
    font-weight: 400;
    text-align: center;
    bottom: 20%;
    left: 10%;
    line-height: 1;
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
  .title {
    position: absolute;
    color: #fff;
    width: 90%;
    font-size: 40px;
    text-align: center;
    top: 5%;
    left: 5%;
    font-weight: 800;
    line-height: 0.9;
  }
  .subtitle {
    position: absolute;
    color: #fff;
    width: 80%;
    font-size: 30px;
    font-weight: 400;
    text-align: center;
    top: 20%;
    left: 10%;
    line-height: 1;
  }
  .imgcut {
    filter: brightness(0.7);
    width: 60%;
    height: 55%;
    object-fit: cover;
    object-position: center;
    position: absolute;
    bottom: 0;
    right: 0;
  }
}
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
  .imgbottom {
    height: 55%;
    width: 270%;
    position: absolute;
    bottom: 0;
    left: 0;
    object-fit: cover;
    object-position: -300px 0;
  }
  .title {
    position: absolute;
    color: #fff;
    width: 90%;
    font-size: 50px;
    text-align: center;
    top: 5%;
    left: 5%;
    font-weight: 300;
    line-height: 0.9;
  }
  .subtitle {
    position: absolute;
    color: #fff;
    width: 80%;
    font-size: 30px;
    font-weight: 300;
    text-align: center;
    top: 20%;
    left: 10%;
    line-height: 1;
  }
}
.section07-container {
  .section-bg {
    left: -10%;
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
    .imgcut {
      width: 40%;
      height: 25%;
      object-fit: cover;
      object-position: -100px center;
      position: absolute;
      left: 0;
      bottom: 25%;
    }
    .title {
      position: absolute;
      color: #fff;
      width: 90%;
      font-size: 30px;
      text-align: center;
      top: 8%;
      left: 5%;
      font-weight: 300;
      line-height: 0.9;
    }
    .subtitle {
      position: absolute;
      color: #fff;
      width: 80%;
      font-size: 100px;
      font-weight: 800;
      text-align: center;
      top: 2%;
      left: 10%;
      line-height: 1;
    }
    .downgrade {
      position: absolute;
      color: #fff;
      width: 80%;
      font-size: 26px;
      left: 10%;
      font-weight: 300;
      bottom: 5%;
    }
  }
}
.section08-container {
  .section-bg {
    left: -155%;
    filter: brightness(0.7);
  }
  .section-08 {
    color: #fff;
    .title {
      position: absolute;
      color: #fff;
      width: 90%;
      font-size: 60px;
      text-align: center;
      bottom: 15%;
      left: 5%;
      font-weight: 800;
      line-height: 0.9;
    }
    .subtitle {
      position: absolute;
      color: #fff;
      width: 80%;
      font-size: 26px;
      font-weight: 300;
      text-align: center;
      bottom: 5%;
      left: 10%;
      line-height: 1;
    }
  }
}
.section09-container {
  .section-bg {
    left: -155%;
    filter: brightness(0.7);
  }
  .section-09 {
    color: #fff;
    .title {
      position: absolute;
      color: #fff;
      width: 90%;
      font-size: 60px;
      text-align: center;
      top: 3%;
      left: 5%;
      font-weight: 800;
      line-height: 0.9;
    }
    .subtitle {
      position: absolute;
      color: #fff;
      width: 80%;
      font-size: 26px;
      font-weight: 300;
      text-align: center;
      top: 24%;
      left: 10%;
      line-height: 1;
    }
  }
}
.section10-container {
  .section-bg {
    left: -10%;
    filter: brightness(0.7);
  }
  .section-10 {
    color: #fff;
    .title {
      position: absolute;
      color: #fff;
      width: 90%;
      font-size: 60px;
      text-align: center;
      top: 3%;
      left: 5%;
      font-weight: 800;
      line-height: 0.9;
    }
    .subtitle {
      position: absolute;
      color: #fff;
      width: 80%;
      font-size: 26px;
      font-weight: 300;
      text-align: center;
      bottom: 10%;
      left: 10%;
      line-height: 1;
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
    .title {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 10%;
      text-align: left;
      bottom: 27%;
      font-size: 50px;
      font-weight: 300;
    }
    .subtitle {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 10%;
      bottom: 15%;
      font-size: 70px;
      font-weight: 800;
      text-align: right;
    }
    .downgrade {
      z-index: 2;
      position: absolute;
      bottom: 16%;
      font-size: 30px;
      width: 80%;
      left: 10%;
      text-align: center;
    }
  }
}
.section12-container {
  .section-bg {
    left: -30%;
    object-position: 100%;
    filter: brightness(0.7);
  }
  .section-12 {
    color: #fff;
    .title {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 10%;
      top: 0;
      font-size: 50px;
      font-weight: 300;
    }
    .subtitle {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 10%;
      top: 13%;
      font-size: 70px;
      font-weight: 800;
    }
    .downgrade {
      z-index: 2;
      position: absolute;
      top: 30%;
      font-size: 30px;
      width: 80%;
      left: 10%;
      font-weight: 300;
    }
  }
}
.section13-container {
  .section-bg {
    height: 85%;
    filter: brightness(0.7);
    object-position: 200px;
  }
  .section-13 {
    color: #fff;
    .entorno {
      height: 150px;
      position: absolute;
      top: 1%;
      left: 10%;
    }
    .title {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 10%;
      bottom: 60%;
      font-size: 40px;
      font-weight: 300;
    }
    .subtitle {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 10%;
      bottom: 42%;
      font-size: 60px;
      font-weight: 800;
      line-height: 0.9;
    }
    .downgrade {
      z-index: 2;
      position: absolute;
      bottom: 33%;
      font-size: 24px;
      width: 80%;
      left: 10%;
      font-weight: 300;
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
    filter: brightness(0.7);
  }
  .section-14 {
    color: #fff;
    .section-14__img01 {
      z-index: 2;
      filter: brightness(0.7);
      width: 60%;
      height: 30%;
      object-fit: cover;
      position: absolute;
      top: 0;
      right: 0;
    }
    .section-14__img02 {
      filter: brightness(0.7);
      position: absolute;
      width: 90%;
      height: 80%;
      object-fit: cover;
      left: 5%;
      top: 10%;
    }
    .section-14__img03 {
      z-index: 2;
      width: 60%;
      height: 30%;
      object-fit: cover;
      position: absolute;
      bottom: 0;
      left: 0;
    }
    .title {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 10%;
      text-align: left;
      top: 18%;
      font-size: 50px;
      font-weight: 800;
      line-height: 1;
    }
    .subtitle {
      z-index: 2;
      position: absolute;
      width: 80%;
      left: 10%;
      top: 45%;
      font-size: 20px;
      text-align: left;
      font-weight: 300;
    }
  }
}
.section15-container {
    background: #e40524;
  .section-15 {
    display: grid;
    height: 100%;
    grid-template-columns: 100%;
    grid-template-rows: repeat(2, min-content);
    row-gap: 30px;
    justify-content: center;
    justify-items: center;
    align-items: center;
    align-content: center;
    .logo{
      width: 60%;
    }
    .bptl{
      width: 40%;
    }
  }
}
</style>
