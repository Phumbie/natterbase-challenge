<template>
  <div>
    <div class="tasks container-fluid">
      <div>
        <div class="task-title d-flex justify-content-between">
          <h5 class="my-auto">Backlog</h5>
          <div class="my-auto">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="11"
              height="3"
              viewBox="0 0 11 3"
              fill="none"
            >
              <path
                d="M6.125 1.5C6.125 1.15482 5.84518 0.875 5.5 0.875C5.15482 0.875 4.875 1.15482 4.875 1.5C4.875 1.84518 5.15482 2.125 5.5 2.125C5.84518 2.125 6.125 1.84518 6.125 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M1.75 1.5C1.75 1.15482 1.47018 0.875 1.125 0.875C0.779822 0.875 0.5 1.15482 0.5 1.5C0.5 1.84518 0.779822 2.125 1.125 2.125C1.47018 2.125 1.75 1.84518 1.75 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M10.5 1.5C10.5 1.15482 10.2202 0.875 9.875 0.875C9.52982 0.875 9.25 1.15482 9.25 1.5C9.25 1.84518 9.52982 2.125 9.875 2.125C10.2202 2.125 10.5 1.84518 10.5 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
        </div>
        <div class="add mb-3">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="9"
            height="9"
            viewBox="0 0 9 9"
            fill="none"
          >
            <path
              d="M9 5.14286H5.14286V9H3.85714V5.14286H0V3.85714H3.85714V0H5.14286V3.85714H9V5.14286Z"
              fill="#23B3E8"
            />
          </svg>
        </div>
        <div class="module-card">
          <addModule v-for="i in 10" :key="i" />
        </div>
      </div>
      <div>
        <div class="task-title d-flex justify-content-between">
          <h5 class="my-auto">Todo</h5>
          <div class="my-auto">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="11"
              height="3"
              viewBox="0 0 11 3"
              fill="none"
            >
              <path
                d="M6.125 1.5C6.125 1.15482 5.84518 0.875 5.5 0.875C5.15482 0.875 4.875 1.15482 4.875 1.5C4.875 1.84518 5.15482 2.125 5.5 2.125C5.84518 2.125 6.125 1.84518 6.125 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M1.75 1.5C1.75 1.15482 1.47018 0.875 1.125 0.875C0.779822 0.875 0.5 1.15482 0.5 1.5C0.5 1.84518 0.779822 2.125 1.125 2.125C1.47018 2.125 1.75 1.84518 1.75 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M10.5 1.5C10.5 1.15482 10.2202 0.875 9.875 0.875C9.52982 0.875 9.25 1.15482 9.25 1.5C9.25 1.84518 9.52982 2.125 9.875 2.125C10.2202 2.125 10.5 1.84518 10.5 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
        </div>
        <div class="add">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="9"
            height="9"
            viewBox="0 0 9 9"
            fill="none"
          >
            <path
              d="M9 5.14286H5.14286V9H3.85714V5.14286H0V3.85714H3.85714V0H5.14286V3.85714H9V5.14286Z"
              fill="#23B3E8"
            />
          </svg>
        </div>
        <div class="module-card">
          <div class="empty-module">
            <!-- <h1>hi</h1> -->
          </div>
        </div>
      </div>
      <div>
        <div class="task-title d-flex justify-content-between">
          <h5 class="my-auto">In Progress</h5>
          <div class="my-auto">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="11"
              height="3"
              viewBox="0 0 11 3"
              fill="none"
            >
              <path
                d="M6.125 1.5C6.125 1.15482 5.84518 0.875 5.5 0.875C5.15482 0.875 4.875 1.15482 4.875 1.5C4.875 1.84518 5.15482 2.125 5.5 2.125C5.84518 2.125 6.125 1.84518 6.125 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M1.75 1.5C1.75 1.15482 1.47018 0.875 1.125 0.875C0.779822 0.875 0.5 1.15482 0.5 1.5C0.5 1.84518 0.779822 2.125 1.125 2.125C1.47018 2.125 1.75 1.84518 1.75 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M10.5 1.5C10.5 1.15482 10.2202 0.875 9.875 0.875C9.52982 0.875 9.25 1.15482 9.25 1.5C9.25 1.84518 9.52982 2.125 9.875 2.125C10.2202 2.125 10.5 1.84518 10.5 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
        </div>
        <div class="add">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="9"
            height="9"
            viewBox="0 0 9 9"
            fill="none"
          >
            <path
              d="M9 5.14286H5.14286V9H3.85714V5.14286H0V3.85714H3.85714V0H5.14286V3.85714H9V5.14286Z"
              fill="#23B3E8"
            />
          </svg>
        </div>
        <div class="module-card">
          <div class="empty-module">
            <!-- <h1>hi</h1> -->
          </div>
        </div>
      </div>
      <div>
        <div class="task-title d-flex justify-content-between">
          <h5 class="my-auto">In Review</h5>
          <div class="my-auto">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="11"
              height="3"
              viewBox="0 0 11 3"
              fill="none"
            >
              <path
                d="M6.125 1.5C6.125 1.15482 5.84518 0.875 5.5 0.875C5.15482 0.875 4.875 1.15482 4.875 1.5C4.875 1.84518 5.15482 2.125 5.5 2.125C5.84518 2.125 6.125 1.84518 6.125 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M1.75 1.5C1.75 1.15482 1.47018 0.875 1.125 0.875C0.779822 0.875 0.5 1.15482 0.5 1.5C0.5 1.84518 0.779822 2.125 1.125 2.125C1.47018 2.125 1.75 1.84518 1.75 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M10.5 1.5C10.5 1.15482 10.2202 0.875 9.875 0.875C9.52982 0.875 9.25 1.15482 9.25 1.5C9.25 1.84518 9.52982 2.125 9.875 2.125C10.2202 2.125 10.5 1.84518 10.5 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
        </div>
        <div class="add">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="9"
            height="9"
            viewBox="0 0 9 9"
            fill="none"
          >
            <path
              d="M9 5.14286H5.14286V9H3.85714V5.14286H0V3.85714H3.85714V0H5.14286V3.85714H9V5.14286Z"
              fill="#23B3E8"
            />
          </svg>
        </div>
        <div class="module-card">
          <div class="empty-module">
            <!-- <h1>hi</h1> -->
          </div>
        </div>
      </div>
      <div>
        <div class="task-title d-flex justify-content-between">
          <h5 class="my-auto">Done</h5>
          <div class="my-auto">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="11"
              height="3"
              viewBox="0 0 11 3"
              fill="none"
            >
              <path
                d="M6.125 1.5C6.125 1.15482 5.84518 0.875 5.5 0.875C5.15482 0.875 4.875 1.15482 4.875 1.5C4.875 1.84518 5.15482 2.125 5.5 2.125C5.84518 2.125 6.125 1.84518 6.125 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M1.75 1.5C1.75 1.15482 1.47018 0.875 1.125 0.875C0.779822 0.875 0.5 1.15482 0.5 1.5C0.5 1.84518 0.779822 2.125 1.125 2.125C1.47018 2.125 1.75 1.84518 1.75 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M10.5 1.5C10.5 1.15482 10.2202 0.875 9.875 0.875C9.52982 0.875 9.25 1.15482 9.25 1.5C9.25 1.84518 9.52982 2.125 9.875 2.125C10.2202 2.125 10.5 1.84518 10.5 1.5Z"
                fill="#03293D"
                stroke="#03293D"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
        </div>
        <div class="add">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="9"
            height="9"
            viewBox="0 0 9 9"
            fill="none"
          >
            <path
              d="M9 5.14286H5.14286V9H3.85714V5.14286H0V3.85714H3.85714V0H5.14286V3.85714H9V5.14286Z"
              fill="#23B3E8"
            />
          </svg>
        </div>
        <div class="module-card">
          <div class="empty-module">
            <!-- <h1>hi</h1> -->
          </div>
        </div>
      </div>
    </div>
    <div class="add-button">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="101"
        height="101"
        viewBox="0 0 101 101"
        fill="none"
      >
        <g filter="url(#filter0_d)">
          <circle cx="50.5" cy="47.5" r="40.5" fill="#23B3E8" />
        </g>
        <g clip-path="url(#clip0)">
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M63.8648 48.715H51.7148V60.865C51.7148 61.5357 51.1705 62.08 50.4998 62.08C49.8291 62.08 49.2848 61.5357 49.2848 60.865V48.715H37.1348C36.4641 48.715 35.9198 48.1707 35.9198 47.5C35.9198 46.8293 36.4641 46.285 37.1348 46.285H49.2848V34.135C49.2848 33.4643 49.8291 32.92 50.4998 32.92C51.1705 32.92 51.7148 33.4643 51.7148 34.135V46.285H63.8648C64.5355 46.285 65.0798 46.8293 65.0798 47.5C65.0798 48.1707 64.5355 48.715 63.8648 48.715Z"
            fill="white"
          />
        </g>
        <defs>
          <filter
            id="filter0_d"
            x="0"
            y="0"
            width="101"
            height="101"
            filterUnits="userSpaceOnUse"
            color-interpolation-filters="sRGB"
          >
            <feFlood flood-opacity="0" result="BackgroundImageFix" />
            <feColorMatrix
              in="SourceAlpha"
              type="matrix"
              values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
            />
            <feOffset dy="3" />
            <feGaussianBlur stdDeviation="5" />
            <feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0" />
            <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow" />
            <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape" />
          </filter>
          <clipPath id="clip0">
            <rect width="29.16" height="29.16" fill="white" transform="translate(35.9198 32.92)" />
          </clipPath>
        </defs>
      </svg>
    </div>
  </div>
</template>
<script>
import addModule from "../addModules";
export default {
  components: {
    addModule,
  },
};
</script>
<style scoped>
.tasks {
  display: grid;
  grid-template-columns: repeat(5, 18%);
  justify-items: center;
  grid-gap: 1.5rem;
  width: 90%;
  margin: auto;
  position: relative;
}
.add {
  text-align: center;
  /* width: 100%; */
  height: 3rem;
  background: #ffffff;
  box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.1);
  border-radius: 5px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 1rem;
}
.tasks > div {
  /* margin: 0 0.5rem; */
  width: 100%;
}
.task-title {
  width: 100%;
}
.empty-module {
  height: 100%;
  background-color: white;
  border-radius: 5px;
  margin-top: 1rem;
}
.module-card {
  height: 100%;
}
.add-button {
  position: absolute;
  bottom: 3rem;
  right: 3rem;
}
</style>