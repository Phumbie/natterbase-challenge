<template>
  <div class="module-card">
    <div class="container-fluid">
      <div class="row">
        <div class="col-md-10">
          <p class="my-auto">
            Apply gredient colours on the
            dashboard sidenav
          </p>
        </div>
        <div class="col-md-2 d-flex a">
          <div class="d-flex">
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
      </div>
      <div class="row">
        <div class="col-md-6">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="11"
            height="11"
            viewBox="0 0 11 11"
            fill="none"
          >
            <g opacity="0.5">
              <path
                d="M5.49983 0.458336C2.71534 0.458336 0.45816 2.71563 0.45816 5.5C0.45816 8.28449 2.71534 10.5417 5.49983 10.5417C8.28432 10.5417 10.5415 8.28449 10.5415 5.5C10.5415 2.71563 8.28432 0.458336 5.49983 0.458336ZM5.49983 9.625C3.22168 9.625 1.37483 7.77826 1.37483 5.5C1.37483 3.22186 3.22168 1.375 5.49983 1.375C7.77797 1.375 9.62483 3.22186 9.62483 5.5C9.62483 7.77826 7.77797 9.625 5.49983 9.625ZM7.19887 6.55096C7.37785 6.72994 7.37785 7.02018 7.19887 7.19916C7.10949 7.28853 6.99205 7.33334 6.87483 7.33334C6.75761 7.33345 6.64028 7.28865 6.55079 7.19916L5.17579 5.82416C5.08985 5.73822 5.04149 5.62169 5.04149 5.5V2.75C5.04149 2.49689 5.24671 2.29167 5.49983 2.29167C5.75294 2.29167 5.95816 2.49689 5.95816 2.75V5.31025L7.19887 6.55096Z"
                fill="#03293D"
              />
            </g>
          </svg>
          <small class="ml-2">Due Aug 3</small>
        </div>
        <div class="col-md-6 text-right my-auto">
          <div class="image d-flex justify-content-end">
            <img src="@/assets/round1.png" alt />
            <img class="img-row" src="@/assets/round2.png" alt />
            <img class="img-row" src="@/assets/round3.png" alt />
            <img class="img-row" src="@/assets/Ellipse.png" alt />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
.module-card {
  /* white */
  width: 100%;
  margin-bottom: 1rem;
  background: #ffffff;
  border-radius: 5px;
  padding: 0.5rem;
}
.img-row {
  margin-left: -0.3rem;
}
p {
  color: #03293d;
}
</style>