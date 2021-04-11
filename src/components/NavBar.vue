<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="dark">
      <b-navbar-brand href="#">TTOG</b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#">線上遊戲</b-nav-item>
          <b-nav-item href="#">手機遊戲</b-nav-item>
          <b-nav-item href="#">網頁遊戲</b-nav-item>
          <b-nav-item href="#">Steam專區</b-nav-item>
          <b-nav-item href="#">點數卡</b-nav-item>
        </b-navbar-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-form class="mx-1">
            <b-form-input
              size="sm"
              class="mr-sm-2"
              placeholder="Search"
            ></b-form-input>
            <b-button size="sm" class="my-2 mr-2 my-sm-1" type="submit">
              <b-icon icon="search"></b-icon>搜尋
            </b-button>
          </b-nav-form>
          <b-button id="cart-tooltip" size="sm" class="my-2 my-sm-1">
            <b-icon icon="cart4"></b-icon>
          </b-button>
          <b-nav-item-dropdown class="ml-2" text="會員中心" right>
            <b-dropdown-item href="#">個人資料</b-dropdown-item>
            <b-dropdown-item href="#">交易中商品</b-dropdown-item>
            <b-dropdown-item href="#">待出售商品</b-dropdown-item>
            <b-dropdown-item href="#">競價出售列表</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <b-tooltip target="cart-tooltip" triggers="hover" variant="light">
      <p class="card-text">最近加入商品</p>
      <b-card no-body>
        <b-row no-gutters>
          <b-col class="mx-1">
            <b-card-img
              src="https://picsum.photos/50/50/?image=20"
              alt="Image"
            ></b-card-img>
          </b-col>
          <b-col>
            <b-card-text> 商品1 </b-card-text>
          </b-col>
          <b-col>
            <b-card-text> $10 </b-card-text>
          </b-col>
        </b-row>
      </b-card>
      <b-card no-body>
        <b-row no-gutters>
          <b-col class="mx-1">
            <b-card-img
              src="https://picsum.photos/50/50/?image=20"
              alt="Image"
            ></b-card-img>
          </b-col>
          <b-col>
            <b-card-text> 商品2 </b-card-text>
          </b-col>
          <b-col>
            <b-card-text> $20 </b-card-text>
          </b-col>
        </b-row>
      </b-card>
    </b-tooltip>
  </div>
</template>
