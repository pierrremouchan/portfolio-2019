<template>
  <main class="experiments-container">
    <div class="brief-container">
      <div class="h1-wrapper">
        <h1>@PIERREMOUCHAN</h1>
      </div>

      <div class="desc-wrapper">
        <p class="description">
          My <strong class="strong-red">lovely playground</strong>, my Instagram account
          <br />
          <span>WTF incoming... 🙃</span>
        </p>
      </div>
    </div>
    <div id="instafeed"></div>
  </main>
</template>

<script>
import { toExperiments, fromExperiments } from '~/assets/js/transitions/fromToExperiments';

export default {
  data() {
    return {};
  },
  head() {
    return {
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Portfolio - @pierremouchan on Instagram 🤙'
        }
      ]
    };
  },
  mounted() {
    toExperiments();
  },
  beforeRouteLeave(to, from, next) {
    fromExperiments(next);
  }
};
</script>

<style lang="scss">
.experiments-container {
  position: relative;
  padding-top: 25vh;
  z-index: $beforefg - 1;
  margin: 0 auto;
  .brief-container {
    text-align: center;
    .h1-wrapper {
      margin: 0 auto 60px auto;
      overflow: hidden;
      h1 {
        font-family: $font-title;
        line-height: normal;
        font-size: 50px;
        white-space: pre-wrap;
        word-break: break-all;
        font-weight: 900;

        @include mq($from: tablet) {
          font-size: 70px;
          white-space: nowrap;
        }
        @include mq($from: desktop_plus) {
          font-size: 100px;
        }
        @include mq($from: wide) {
          font-size: 120px;
        }
      }
    }
    .desc-wrapper {
      overflow: hidden;

      .description {
        font-size: 35px;
        line-height: 40px;
        @include mq($from: tablet) {
          font-size: 40px;
          line-height: 40px;
        }
        @include mq($from: desktop_plus) {
          font-size: 50px;
        }

        span {
          font-size: 18px;
        }
      }
    }
  }
  #instafeed {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 0 auto 5vh auto;
    @include mq($from: desktop) {
      justify-content: center;
      flex-wrap: wrap;
      flex-direction: row;
      margin-bottom: 0;
      width: 75%;
    }

    .insta-img {
      z-index: $up;
      opacity: 0;
      overflow: hidden;
      position: relative;
      width: 350px;
      height: 350px;
      &:not(:last-child) {
        margin-bottom: 5vh;
      }

      @include mq($from: tablet) {
        margin: 2.5vh;
      }

      &__mask {
        position: absolute;
        top: 0;
        z-index: $up;
        background-color: $black;
        width: 100%;
        height: 100%;
      }

      a {
        display: block;
        width: 350px;
        height: 350px;
        img {
          transition: 0.5s;
          &:hover {
            transform: scale(1.1) rotate(5deg);
          }
        }
      }
    }
  }
}
</style>
