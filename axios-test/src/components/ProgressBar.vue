<template>

</template>

<script setup>

</script>

<style>
body {
  background: #f8f8f8;
}
#steps {
  width: 625px;
  margin-inline: auto;
  margin-top: 15px;
  margin-bottom: 60px;
}

.step {
  width: 45px;
  height: 45px;
  background-color: #fff;
  display: inline-block;
  border: 4px solid;
  border-color: transparent;
  border-radius: 50%;
  color: #cdd0da;
  font-weight: 600;
  text-align: center;
  line-height: 30px;
}

.step:first-child {
  line-height: 35px;
}

.step:nth-child(n+2) {
  margin: 0 0 0 100px;
  transform: translate(0, -4px);
}

.step:nth-child(n+2):before {
  width: 75px;
  height: 3px;
  display: block;
  background-color: #fff;
  transform: translate(-95px, 18px);
  content: '';
}

.step:after {
  width: 150px;
  display: block;
  transform: translate(-55px, 20px);
  color: #818698;
  content: attr(data-desc);
  font-weight: 400;
  font-size: 13px;
}

.step:first-child:after {
  transform: translate(-55px, 16px);
}

.step.active {
  border-color: #999;
  color: #999;
}

.step.active:before {
  background: linear-gradient(to right, #58bb58 0%, #999 100%);
}

.step.active:after {
  color: #999;
}

.step.done {
  background-color: #58bb58;
  border-color: #58bb58;
  color: #fff;
}

.step.done:before {
  background-color: #58bb58;
}

@media  screen and (max-width: 715px) {
  #steps {
    display: none;
  }
}

</style>