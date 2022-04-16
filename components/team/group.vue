<template>
    <div>
        <div class="app">
  <div class="cardList">
    <button class="cardList__btn btn btn--left">
      <div class="icon">
        <svg>
          <use xlink:href="#arrow-left"></use>
        </svg>
      </div>
    </button>

    <div class="cards__wrapper">
      <div class="card current--card">
        <div class="card__image">
          <img src="img/person1.png" alt="" />
        </div>
      </div>

      <div class="card next--card">
        <div class="card__image">
          <img src="img/person2.png" alt="" />
        </div>
      </div>

      <div class="card previous--card">
        <div class="card__image">
          <img src="img/person3.png" alt="" />
        </div>
      </div>
    </div>

    <button class="cardList__btn btn btn--right">
      <div class="icon">
        <svg>
          <use xlink:href="#arrow-right"></use>
        </svg>
      </div>
    </button>
  </div>

  <div class="infoList">
    <div class="info__wrapper">
      <div class="info current--info">
        <h1 class="text name">Gilang Muh Iqbal</h1>
        <h4 class="text location">Front-End Users</h4>
        <p class="text description">Student Fullstack Developer Batch 6</p>
      </div>

      <div class="info next--info">
        <h1 class="text name">Muhammad Nur Fauzan</h1>
        <h4 class="text location">Front-End Users</h4>
        <p class="text description">Student Fullstack Developer Batch 6</p>
      </div>

      <div class="info previous--info">
        <h1 class="text name">Aufa</h1>
        <h4 class="text location">Back-End</h4>
        <p class="text description">Student Fullstack Developer Batch 6</p>
      </div>
    </div>
  </div>


  <div class="app__bg">
    <div class="app__bg__image current--image">
      
    </div>
    <div class="app__bg__image next--image">
      
    </div>
    <div class="app__bg__image previous--image">
      
    </div>
  </div>
</div>

<svg class="icons" style="display: none;">
  <symbol id="arrow-left" xmlns='http://www.w3.org/2000/svg' viewBox='0 0 512 512'>
    <polyline points='328 112 184 256 328 400'
           style='fill:none;stroke:#00CC8E;stroke-linecap:round;stroke-linejoin:round;stroke-width:48px' />
  </symbol>
  <symbol id="arrow-right" xmlns='http://www.w3.org/2000/svg' viewBox='0 0 512 512'>
    <polyline points='184 112 328 256 184 400'
           style='fill:none;stroke:#00CC8E;stroke-linecap:round;stroke-linejoin:round;stroke-width:48px' />
  </symbol>
</svg>
    </div>
</template>
