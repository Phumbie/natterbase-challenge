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
</style>