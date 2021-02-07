<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="info" class="shadow-lg">
      <b-navbar-brand href="#">
        <img
          src="@/assets/logo.png"
          class="d-inline-block align-top"
          alt="Kitten"
          style="width: 30px; height: 30px"
        />
        XX村图书馆
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#">图书</b-nav-item>
          <b-nav-item href="#">共享图书</b-nav-item>
          <b-nav-item href="#">借阅记录</b-nav-item>
          <b-nav-item href="#">积分商城</b-nav-item>
          <b-nav-item href="#">管理员</b-nav-item>
        </b-navbar-nav>

        <b-navbar-nav class="ml-auto">
          <b-nav-form>
            <b-form-input
              size="md"
              class="mr-sm-2"
              placeholder="搜索图书"
            ></b-form-input>
            <b-button size="md" class="my-2 my-sm-0" type="submit"
              >搜索</b-button
            >
          </b-nav-form>

          <b-nav-item right>
            <b-icon icon="cart4"></b-icon>
          </b-nav-item>
          <b-nav-item right>
            <b-icon icon="chat-dots"></b-icon>
            <b-badge pill variant="danger" style="font-size: 7px">99+</b-badge>
          </b-nav-item>

          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template #button-content>
              <em><b-icon icon="person-fill"></b-icon>User</em>
            </template>
            <b-dropdown-item href="#">Profile</b-dropdown-item>
            <b-dropdown-item href="#">Sign Out</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "NavBar",
};
</script>

<style>
</style>