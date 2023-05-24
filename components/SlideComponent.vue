<script setup>
onMounted(function(){

const boxes = document.querySelectorAll('.content__box');

window.addEventListener('scroll', checkBoxes);

checkBoxes(); // shows initial box(es) 

function checkBoxes() {
  const triggerBottom = (window.innerHeight / 5 * 4);
  
  boxes.forEach(box => {
    const boxTop = box.getBoundingClientRect().top;
    
    if(boxTop < triggerBottom) {
      box.classList.add('show');
    } else {
      box.classList.remove('show');
    }
  })
}
})
</script>

<template>
  <h2>Что я могу?</h2>
  <div class="content__container">
    <div class="content__box">
      <div class="content__box--item">Проконсультировать и ответить на все вопросы по татуировке.</div>
      <img class="content__box--img" src="/img/t4.jpg" alt="">
    </div>
    <div class="content__box">
      <img class="content__box--img" src="/img/t3.jpg" alt="">
      <div class="content__box--item content__box--right">Разработать эскиз, учитывая все пожелания.</div>
    </div>
    <div class="content__box">
      <div class="content__box--item">Качественно и безопасно нанести рисунок.</div>
      <img class="content__box--img" src="/img/t2.jpg" alt="">
    </div>
    <div class="content__box">
      <img class="content__box--img" src="/img/t5.jpg" alt="">
      <div class="content__box--item content__box--right">Перекрыть старую татуировку или шрам.</div>
    </div>
    <div class="content__box">
      <div class="content__box--item">Откорректировать татуировку, которая уже есть, но не полностью устраивает.</div>
      <img class="content__box--img" src="/img/t8.jpg" alt="">
    </div>
    <div class="content__box">
      <img class="content__box--img" src="/img/t9.jpg" alt="">
      <div class="content__box--item content__box--right">Рассказать про уход и правильное заживление новой тату.</div>
    </div>
    <div class="content__box">
      <div class="content__box--item">Вкусняшки, чай, сериал или фильм, wi-fi и классная атмосфера, жду тебя!</div>
      <img class="content__box--img" src="/img/t10.jpg" alt="">
    </div>
  </div>
</template>

<style lang="sass" scoped>
.content__container
  margin: 0
  overflow-x: hidden
.content__box
  transform: translateX(400%)
  transition: transform 0.7s ease
  &:nth-of-type(even)
    transform: translateX(-400%)
  &--right
    text-align: right
.content__box.show
  transform: translateX(0)
</style>