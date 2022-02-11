<template>
  <div class="shopping-lists-wrapper">
    <div class="shopping-content">
      <p class="shopping-lists-title">購物籃</p>
      <ul class="shopping-lists">
        <li class="product">
          <img src="../assets/image/jeans-slim@2x.png" alt="" />
          <div class="product-content d-flex flex-column">
            <span class="title">破壞補丁修身牛仔褲</span>
            <div class="amount-control">
              <div class="minus">－</div>
              <span class="amount">1</span>
              <div class="plus">＋</div>
            </div>
            <div class="price">$3,999</div>
          </div>
        </li>
        <li class="product">
          <img src="../assets/image/jeans-straight@2x.png" alt="" />
          <div class="product-content d-flex flex-column">
            <span class="title">刷色直筒牛仔褲</span>
            <div class="amount-control">
              <div class="minus">－</div>
              <span class="amount">1</span>
              <div class="plus">＋</div>
            </div>
            <div class="price">$1,299</div>
          </div>
        </li>
      </ul>
      <div
        class="price-outline d-flex justify-content-between align-items-center"
      >
        運費
        <div class="delivery-fee">免費</div>
      </div>
      <div
        class="price-outline d-flex justify-content-between align-items-center"
      >
        小計
        <div class="total-amount">$5,298</div>
      </div>
    </div>
  </div>
</template>