<template>
  <!-- eslint-disable max-len -->
  <svg
    viewBox="0 0 100 100"
    xmlns="http://www.w3.org/2000/svg"
    style="height: 100%; width: 100%; background: rgb(255, 255, 255)"
    ref="svg"
    :x="`${coords.x}%`"
    :y="`${coords.y}%`"
  >
    <g
      class="ldl-scale"
      style="transform-origin: 50% 50%; transform: rotate(0deg) scale(0.8, 0.8)"
    >
      <title>{{ `id: ${id}` }}</title>
      <g class="ldl-ani">
        <linearGradient
          y2="79.426"
          x2="68.331"
          y1="31.426"
          x1="22.831"
          gradientUnits="userSpaceOnUse"
          id="a"
        >
          <stop
            stop-color="#a0c8d7"
            offset="0"
            style="stop-color: rgb(160, 200, 215); fill: rgb(0, 0, 0)"
          ></stop>
          <stop
            stop-color="#76a4bd"
            offset="1"
            style="stop-color: rgb(118, 164, 189); fill: rgb(0, 0, 0)"
          ></stop>
        </linearGradient>
        <g class="ldl-layer">
          <g
            class="ldl-ani"
            style="
              transform-origin: 50px 50px;
              transform: scale(0.91);
              animation: 2.22222s linear -2.22222s infinite alternate forwards running
                breath;
            "
            :style="{ 'animation-name': 'breath' }"
          >
            <path
              fill="url(#a)"
              d="M47.962 10.051c-20.276 1.006-36.785 17.429-37.9 37.699-.482 8.762 1.87 16.943 6.206 23.736l-4.889 14.443c-.564 1.667 1.027 3.258 2.693 2.693l14.443-4.889c6.793 4.336 14.974 6.688 23.736 6.206 20.27-1.115 36.693-17.624 37.699-37.9 1.175-23.701-18.288-43.165-41.988-41.988z"
            ></path>
          </g>
        </g>
        <g class="ldl-layer">
          <g class="ldl-ani">
            <g>
              <g class="ldl-layer">
                <g
                  class="ldl-ani"
                  style="
                    transform-origin: 50px 50px;
                    transform: scale(0.91);
                    animation: 2.22222s linear -2.22222s infinite alternate forwards
                      running breath;
                  "
                  :style="{ 'animation-name': 'breath' }"
                >
                  <path
                    fill="#fff"
                    d="M54.435 71.5h-8.87A1.565 1.565 0 0 1 44 69.935v-20.87c0-.864.701-1.565 1.565-1.565h8.87c.864 0 1.565.701 1.565 1.565v20.87c0 .864-.701 1.565-1.565 1.565z"
                    style="fill: rgb(255, 255, 255)"
                  ></path>
                </g>
              </g>
              <g class="ldl-layer">
                <g
                  class="ldl-ani"
                  style="
                    transform-origin: 50px 50px;
                    transform: scale(0.91);
                    animation: 2.22222s linear -2.22222s infinite alternate forwards
                      running breath;
                  "
                  :style="{ 'animation-name': 'breath' }"
                >
                  <path
                    fill="#fff"
                    d="M50 28a7.25 7.25 0 0 0 0 14.5A7.25 7.25 0 0 0 50 28z"
                    style="fill: rgb(255, 255, 255)"
                  ></path>
                </g>
              </g>
            </g>
          </g>
        </g>
        <g class="ldl-layer">
          <g
            class="ldl-ani"
            style="
              transform-origin: 50px 50px;
              transform: scale(0.91);
              animation: 2.22222s linear -2.22222s infinite alternate forwards running
                breath;
            "
            :style="{ 'animation-name': 'breath' }"
          >
            <path
              opacity=".1"
              d="M77.639 21.103c.011.603.04 1.201.04 1.808 0 27.323-11.319 51.604-28.865 67.069 1.135.033 2.28.022 3.437-.042 20.27-1.115 36.693-17.624 37.699-37.9.603-12.174-4.247-23.22-12.311-30.935z"
              style="fill: rgb(0, 0, 0)"
            ></path>
          </g>
        </g>
        <g class="ldl-layer">
          <g
            class="ldl-ani"
            style="
              transform-origin: 50px 50px;
              transform: scale(0.91);
              animation: 2.22222s linear -2.22222s infinite alternate forwards running
                breath;
            "
            :style="{ 'animation-name': 'breath' }"
          >
            <path
              stroke-miterlimit="10"
              stroke-linejoin="round"
              stroke-linecap="round"
              stroke-width="3"
              stroke="#fff"
              fill="none"
              d="M17.676 38.688a41.09 41.09 0 0 0-.542 1.781"
              style="stroke: rgb(255, 255, 255)"
            ></path>
          </g>
        </g>
        <g class="ldl-layer">
          <g
            class="ldl-ani"
            style="
              transform-origin: 50px 50px;
              transform: scale(0.91);
              animation: 2.22222s linear -2.22222s infinite alternate forwards running
                breath;
            "
            :style="{ 'animation-name': 'breath' }"
          >
            <path
              stroke-miterlimit="10"
              stroke-linejoin="round"
              stroke-linecap="round"
              stroke-width="3"
              stroke="#fff"
              fill="none"
              d="M29.237 22.583c-3.656 2.599-6.62 5.91-8.857 9.908"
              style="stroke: rgb(255, 255, 255)"
            ></path>
          </g>
        </g>
      </g>
    </g>
  </svg>
</template>

<script>
export default {
  props: ['coords', 'id'],
  data() {
    return {
      size: '10%',
    };
  },
  mounted() {
    const style = document.createElement('style');
    style.innerHTML = `
      @keyframes breath {
        0% {
          animation-timing-function: cubic-bezier(
            0.9647,
            0.2413,
            -0.0705,
            0.7911
          );
          transform: scale(0.9099999999999999);
        }
        51% {
          animation-timing-function: cubic-bezier(
            0.9226,
            0.2631,
            -0.0308,
            0.7628
          );
          transform: scale(1.02994);
        }
        100% {
          transform: scale(0.9099999999999999);
        }
      }
    `;
    this.$el.prepend(style);
  },
};
</script>
