<template>
  <form id="a-form">
    <div class="section delivery-info d-none">
      <h2 class="form-title">運送方式</h2>
      <div class="form-wrap mt-6">
        <div class="form-row d-flex">
          <input type="radio" name="delivery" value="standard" />
          <label for="">
            <div class="delivery-method standard">
              標準運送<span class="fee">免費</span>
            </div>
            <div class="days">約3~7個工作天</div>
          </label>
        </div>
      </div>
      <div class="form-wrap mt-6">
        <div class="form-row d-flex form-delivery">
          <input type="radio" name="delivery" value="DHL" />
          <label for="delivery">
            <div class="delivery-method dhl">
              DHL貨運<span class="fee">$500</span>
            </div>
            <div class="days">48小時內送達</div>
          </label>
        </div>
      </div>
    </div>
  </form>
</template>