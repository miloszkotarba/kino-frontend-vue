<script setup>
</script>

<template>
  <section class="hero">
    <nav>
      <div class="logo">
        <div class="logo-img">
          <svg
              enable-background="new 0 0 91 91"
              height="91px"
              id="Layer_1"
              version="1.1"
              viewBox="0 0 91 91"
              width="91px"
              xml:space="preserve"
              xmlns="http://www.w3.org/2000/svg"
          >
              <g>
                <path
                    d="M2.776,82.355c9.909,0.493,19.864,0.474,29.785,0.675c4.745,0.096,9.491,0.192,14.236,0.289   c4.266,0.088,8.71,0.533,12.947-0.112c5.219-0.794,7.587-4.099,8.733-8.277c5.639,2.646,11.217,5.551,16.513,8.796   c2.229,1.366,4.858-0.429,4.974-2.854c0.6-12.705,1.109-25.559,0.538-38.273c-0.119-2.633-2.789-4.175-5.129-2.943   c-4.98,2.626-10.757,4.983-15.659,8.17C69.66,46.556,69.6,45.282,69.527,44c-0.083-1.503-1.197-2.745-2.762-2.763   c-1.384-0.015-2.768-0.044-4.151-0.063c6.359-3.657,10.901-10.495,10.446-18.095c-0.318-5.311-3.085-10.052-7.46-13.059   C60.25,6.346,53.666,6.367,47.451,6.877c-3.608,0.297-4.903,3.281-4.257,5.765c-4.441,2.589-8.013,6.445-9.174,11.454   c-0.71-3.47-2.85-6.56-5.808-8.536c-4.253-2.841-9.419-2.818-14.321-2.421c-2.886,0.233-3.913,2.631-3.378,4.613   c-4.341,2.521-7.654,6.531-7.629,11.875c0.022,4.417,2.598,8.021,6.14,10.307c-1.642,0.024-3.28,0.068-4.91,0.159   C0.094,40.318,0,45.797,3.699,46.475C2.823,57.563,1.154,68.648,0.141,79.721C0.007,81.189,1.46,82.289,2.776,82.355z    M62.79,75.273c-1.683,3.313-6.137,2.772-9.281,2.717c-15.992-0.289-32.028-0.98-48.026-0.914   C5.749,66.959,5.75,56.777,6.235,46.671c9.681,0.56,19.595-0.043,29.273-0.036c9.551,0.007,19.103,0.03,28.654,0.112   c0.373,6.491,0.7,12.979,0.045,19.471C63.918,69.068,64.117,72.656,62.79,75.273z M83.681,47.916   c0.01,9.057,0.073,18.098-0.146,27.154c-4.364-2.729-13.597-8.698-13.898-8.805c0.276-4.265,0.338-8.479,0.262-12.711   C72.776,52.668,81.92,48.717,83.681,47.916z M39.096,26.115c0.532-4.416,3.713-7.801,7.6-10.17c0.595,0.11,1.255,0.127,1.984,0.01   c6.434-1.03,16.544-1.124,17.253,7.675c0.579,7.199-5.986,13.501-12.848,14.088C46.634,38.268,38.208,33.489,39.096,26.115z    M33.868,30.115c0.858,4.525,3.912,8.25,7.859,10.693c-2.073-0.043-4.146-0.083-6.219-0.128c-3.112-0.068-6.25-0.2-9.396-0.336   C29.905,38.096,32.828,34.394,33.868,30.115z M7.201,28.596c0.342-3.598,2.951-6.334,6.114-8.242   c0.466,0.084,0.982,0.096,1.553,0.004c5.275-0.837,13.589-0.764,13.738,6.58c0.114,5.564-4.898,10.26-10.234,10.735   C13.316,38.124,6.65,34.391,7.201,28.596z"
                />
              </g>
            </svg>
        </div>
        <h1>Screenix</h1>
      </div>
      <ul class="nav">
        <RouterLink to="/repertuar" class="link">
          <li>Repertuar</li>
        </RouterLink>
        <RouterLink to="/cennik" class="link">
          <li>Cennik</li>
        </RouterLink>
        <RouterLink to="/kontakt" class="link">
          <li>Kontakt</li>
        </RouterLink>
      </ul>
    </nav>
    <div class="container">
      <div class="left">
        <h1>Kino Screenix</h1>
        <div class="brand">Gdzie Każdy Kadr Jest Doskonały</div>
        <RouterLink :to="{ name: 'repertuar'}" class="a">
          <button>kup bilet </button>
        </RouterLink>
      </div>
      <div class="right">
        <img src="../assets/img/19198445-removebg.png" alt="Cinema Background"/>
      </div>
    </div>
  </section>
</template>

<style scoped>
.link {
  text-decoration: none;
}

.hero {
  min-height: 100vh;
  background: linear-gradient(to bottom, #49188d, #9b59b6);
  display: flex;
  align-items: center;
}

nav {
  position: fixed;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  max-width: 1700px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 2rem;
}

nav .logo h1 {
  color: var(--primary-color);
  font-size: 2.5rem;
  font-weight: 500;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 2.7rem;
}

nav ul .link li {
  color: var(--secondary-color);
  font-size: 1.3rem;
  font-weight: 300;
  text-transform: uppercase;
  letter-spacing: 0.5px;
  padding: 5px;
}

.hero .container {
  display: flex;
  flex-direction: row;
  align-items: center;
  max-width: 1700px;
  width: 100%;
  margin-inline: auto;
  padding-inline: 2rem;
}

.hero .container .left h1 {
  color: var(--primary-color);
  font-size: 5rem;
  font-weight: 500;
  text-transform: uppercase;
  white-space: nowrap;
  line-height: 120%;
}

.hero .container .left .brand {
  color: var(--secondary-color);
  font-size: 1.7rem;
  font-weight: 300;
}

.hero .container .left button {
  background: #4997fc;
  color: var(--primary-color);
  padding: 15px 45px;
  font-size: 1.6rem;
  text-transform: uppercase;
  border: none;
  border-radius: 5px;
  margin-top: 1.5rem;
  box-shadow: 0 0 3px 1px #764eaf;
  transition: background ease 0.2s;
}

.hero .container .left button:hover {
  cursor: pointer;
  background: rgb(62, 143, 248);
}

.hero .container .right {
  flex-grow: 1;
}

.hero .container .right img {
  width: 100%;
}

.logo {
  display: flex;
  align-items: center;
  gap: 1.5rem;
}

svg path {
  color: #fff !important;
  fill: #ddd !important;
}

svg {
  width: 55px;
  animation: pulsate 2.5s infinite;
}

@keyframes pulsate {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.15);
  }
  100% {
    transform: scale(1);
  }
}

@media screen and (max-width: 1300px) {
  .hero .container {
    flex-direction: column;
    margin-top: 2rem;
  }

  .hero nav {
    display: none;
  }

  .hero .container .left {
    text-align: center;
  }

  .hero .container .left h1 {
    font-size: 3.8rem;
  }

  .hero .container .left .brand {
    font-size: 1.3rem;
  }

  .hero .container .left button {
    display: block;
    margin-inline: auto;
    font-size: 1.3rem;
  }

  .hero .container .right {
    margin-top: 1.5rem;
    display: flex;
    justify-content: center;
  }

  .hero .container .right img {
    width: 80%;
  }
}

@media screen and (max-width: 600px) {
  html {
    font-size: 12px;
  }

  .hero .container {
    margin-top: 0;
  }
}

@media screen and (max-width: 400px) {
  html {
    font-size: 10px;
  }

  .hero .container {
    margin-top: 0;
  }
}

@media screen and (max-width: 300px) {
  html {
    font-size: 8px;
  }

  .hero .container {
    margin-top: 0;
  }
}
</style>
