<template>
  <header>
    <nuxt-link id="logo" aria-label="Home" to="/" @click.native="onRouteChange">
      <pm-logo></pm-logo>
    </nuxt-link>

    <nav>
      <ul>
        <li>
          <nuxt-link to="/" @click.native="onRouteChange">HOME</nuxt-link>
        </li>

        <li>
          <nuxt-link to="/experiments" @click.native="onRouteChange">EXP</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/about" @click.native="onRouteChange">ABOUT</nuxt-link>
        </li>
      </ul>
    </nav>
    <div id="awwwards" style="position: fixed; z-index: 999; transform: translateY(-50%); top: 50%;  right: 0">
      <a href="https://www.awwwards.com/sites/portfolio-pierre-mouchan" target="_blank">
        <svg width="53.08" height="171.358">
          <path class="js-color-bg" fill="black" d="M0 0h53.08v171.358H0z" />
          <g class="js-color-text" fill="white">
            <path
              d="M20.047 153.665v-2.134l6.387-2.411-6.387-2.413v-2.133h10.23v1.9h-6.314l5.379 1.959v1.374l-5.379 1.958h6.314v1.9zM29.898 141.038a3.319 3.319 0 0 1-1.361 1.294c-.573.297-1.221.445-1.943.445-.721 0-1.368-.148-1.943-.445a3.326 3.326 0 0 1-1.359-1.294c-.331-.565-.497-1.232-.497-2.002 0-.771.166-1.438.497-2.003a3.317 3.317 0 0 1 1.359-1.293c.575-.298 1.223-.446 1.943-.446.723 0 1.37.148 1.943.446a3.31 3.31 0 0 1 1.361 1.293c.33.564.496 1.232.496 2.003.001.77-.165 1.437-.496 2.002m-1.703-3.348c-.435-.33-.968-.496-1.602-.496-.633 0-1.167.166-1.6.496-.435.331-.651.779-.651 1.346 0 .564.217 1.013.651 1.344.433.332.967.498 1.6.498.634 0 1.167-.166 1.602-.498.434-.331.649-.779.649-1.344.001-.566-.215-1.015-.649-1.346M30.117 131.176c-.186.326-.386.548-.6.665h.76v1.812H19.93v-1.812h3.654c-.215-.166-.4-.414-.556-.746a2.422 2.422 0 0 1-.235-1.038c0-1.082.345-1.912 1.031-2.492.688-.579 1.611-.869 2.771-.869s2.083.29 2.771.869c.687.58 1.029 1.41 1.029 2.492 0 .419-.093.792-.278 1.119m-1.871-2.099c-.399-.32-.949-.481-1.651-.481-.711 0-1.265.161-1.659.481-.395.322-.592.731-.592 1.229s.197.904.592 1.22c.395.317.948.476 1.659.476.712 0 1.264-.158 1.659-.476.394-.315.592-.723.592-1.22s-.2-.907-.6-1.229M21.625 124.98c-.225.225-.502.337-.833.337s-.608-.112-.833-.337-.337-.502-.337-.833c0-.332.112-.608.337-.833s.502-.337.833-.337.608.112.833.337.336.501.336.833c0 .332-.111.609-.336.833m1.286-1.739h7.367v1.812h-7.367v-1.812zM19.93 119.389h10.349v1.813H19.93zM29.832 116.189c-.375.531-.853.921-1.433 1.169a4.548 4.548 0 0 1-3.611 0 3.339 3.339 0 0 1-1.433-1.169c-.375-.532-.563-1.196-.563-1.995 0-.77.184-1.413.55-1.93a3.282 3.282 0 0 1 1.381-1.14 4.23 4.23 0 0 1 1.71-.365h.746v5.072a1.798 1.798 0 0 0 1.169-.49c.332-.307.497-.724.497-1.249 0-.41-.094-.753-.278-1.031-.185-.277-.473-.529-.862-.753l.541-1.462c.691.302 1.224.724 1.592 1.265.371.541.557 1.234.557 2.083 0 .799-.188 1.463-.563 1.995m-4.086-3.574c-.408.089-.746.262-1.008.52-.263.258-.395.611-.395 1.06 0 .429.136.784.408 1.067.273.282.604.458.994.526v-3.173zM20.047 102.852v-1.899l10.231-3.464v2.046l-2.412.746v3.244l2.412.745v2.046l-10.231-3.464zm6.065-2.031l-3.552 1.08 3.552 1.082v-2.162zM22.91 97.414v-1.827l5.059-1.316-5.059-1.243v-1.695l5.059-1.242-5.059-1.316v-1.827l7.367 2.354v1.607l-4.763 1.273 4.763 1.27v1.609zM29.811 85.676c-.391.419-.94.628-1.652.628-.73 0-1.314-.277-1.754-.833-.438-.555-.658-1.306-.658-2.251v-1.286h-.32c-.36 0-.632.122-.812.366-.181.243-.271.55-.271.92 0 .633.282 1.058.848 1.272l-.352 1.534a2.316 2.316 0 0 1-1.482-.942c-.375-.513-.563-1.132-.563-1.864 0-.984.261-1.747.782-2.287.521-.541 1.289-.812 2.302-.812h4.4v1.491l-.937.19c.702.575 1.053 1.33 1.053 2.265 0 .654-.195 1.19-.584 1.609m-1.383-3.245c-.276-.331-.645-.497-1.104-.497h-.144v1.213c0 .4.078.709.233.93.156.219.394.327.716.327a.658.658 0 0 0 .52-.226c.132-.151.197-.349.197-.593 0-.439-.14-.822-.418-1.154M22.91 78.179v-1.813h1.199a2.93 2.93 0 0 1-.972-.965 2.324 2.324 0 0 1-.345-1.213c0-.273.05-.57.146-.892l1.682.336a1.452 1.452 0 0 0-.205.76c0 .576.262 1.048.783 1.418s1.342.556 2.461.556h2.617v1.813H22.91zM29.364 71.716c-.687.561-1.61.84-2.771.84-1.158 0-2.082-.279-2.77-.84s-1.029-1.352-1.029-2.375c0-.42.074-.802.226-1.147.151-.347.339-.607.563-.782H19.93v-1.813h10.348v1.813h-.76c.224.117.427.35.607.693.18.348.27.759.27 1.236 0 1.023-.344 1.814-1.031 2.375m-1.11-3.99c-.396-.316-.947-.476-1.66-.476-.711 0-1.264.159-1.657.476a1.493 1.493 0 0 0-.593 1.221c0 .496.197.906.593 1.229.394.32.946.481 1.657.481.703 0 1.252-.161 1.652-.481.4-.322.6-.732.6-1.229 0-.498-.198-.905-.592-1.221M35.48 17.006l-4.783 14.969h-3.265l-2.584-9.682-2.584 9.682h-3.267l-4.782-14.969h3.712L20.6 27.282l2.525-10.276h3.445l2.525 10.276 2.673-10.276zM37.978 27.163c1.425 0 2.495 1.068 2.495 2.495 0 1.425-1.07 2.495-2.495 2.495-1.426 0-2.495-1.07-2.495-2.495-.001-1.427 1.069-2.495 2.495-2.495"
            />
          </g>
        </svg>
      </a>
    </div>
  </header>
</template>

<script>
import { TweenMax, Expo, TimelineMax } from 'gsap';
import pmLogo from '~/static/images/icons/logo.svg?inline';
export default {
  components: {
    pmLogo
  },
  data() {
    return {};
  },
  created() {
    this.$store.watch(
      () => this.$store.getters['loader/alreadyLoaded'],
      isalreadyLoaded => {
        switch (isalreadyLoaded) {
          case true:
            TweenMax.fromTo('#logo svg', 1, { y: '-100%' }, { y: '0%', ease: Expo.easeOut });
            TweenMax.staggerFromTo('nav ul li', 2, { y: '-100%' }, { y: '0%', ease: Expo.easeOut }, 0.25);
            break;
        }
      }
    );
  },
  methods: {
    onRouteChange() {
      if (document.querySelector('.nuxt-link-exact-active')) {
        document.querySelector('.nuxt-link-exact-active').classList.remove('nuxt-link-exact-active');
      }

      const onRouteChangeTimeline = new TimelineMax({});
      onRouteChangeTimeline
        .staggerFromTo('nav ul li', 0.75, { y: '0%' }, { y: '-100%', ease: Expo.easeIn }, 0.1)
        .staggerFromTo(
          'nav ul li',
          0.75,
          { y: '100%' },
          {
            y: '0%',
            ease: Expo.easeOut
          },
          0.1
        );
    }
  }
};
</script>

<style lang="scss" scoped>
header {
  position: sticky;
  top: 0;
  left: 0;
  width: 100%;
  height: 56px;
  z-index: $beforefg;
  background-color: $white;
  #awwwards {
    display: none;
    @include mq($from: tablet) {
      display: block;
    }
  }

  #logo {
    position: absolute;
    width: 56px;
    height: 32px;
    left: 16px;
    top: 50%;
    transform: translateY(-50%);
    overflow: hidden;
    svg {
    }

    @include mq($from: tablet) {
      left: 50%;
      transform: translateX(-50%) translateY(-50%);
    }
  }
  nav {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    right: 16px;
    width: 75%;
    @include mq($from: tablet) {
      width: 40%;
    }
    @include mq($from: wide) {
      width: 20%;
    }
    ul {
      display: flex;
      flex-direction: row;
      justify-content: space-around;
      overflow: hidden;
      li {
        overflow: hidden;
        a {
          position: relative;
          letter-spacing: 4px;
          z-index: $normal;

          @include mq($until: 375px) {
            letter-spacing: 0;
          }
          &.nuxt-link-exact-active {
            font-weight: bold;

            &:before {
              content: '';
              background-color: $red;
              opacity: 0.8;
              width: 100%;
              height: 8px;
              z-index: $beforebg;

              position: absolute;
              bottom: -25%;
              transform: translateY(-50%);
              left: 0;
              transition: left 1s cubic-bezier(0.1, 0.86, 0.2, 1.23);
            }

            &:hover {
              &:before {
                left: 25%;
              }
            }
          }
          &:not(.nuxt-link-exact-active) {
            &:before {
              content: '';
              background-color: $red;
              opacity: 0.8;
              width: 100%;
              height: 8px;
              z-index: $beforebg;

              position: absolute;
              bottom: -25%;
              transform: translateY(-50%);
              left: -100%;
              transition: left 1s cubic-bezier(0.1, 0.86, 0.2, 1.23);
            }

            &:hover {
              &:before {
                left: 25%;
              }
            }
          }
        }
      }
    }
  }
}
</style>
