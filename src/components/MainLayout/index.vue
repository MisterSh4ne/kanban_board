<template>
  <div class="full-height">
    <div class="topnav">
      <div class="font-impact logo">BSRU Kanban</div>
      <div>
        <div>
          <b-avatar
            style="margin-right: 12px"
            size="lg"
            :src="image_profile"
          ></b-avatar>

          <b-dropdown id="fullname-btn" :text="fullname">
            <b-dropdown-item class="memu-item">
              <b-icon icon="gear"></b-icon> Account Setting
            </b-dropdown-item>
            <b-dropdown-item class="memu-item">
              <b-icon icon="box-arrow-right"></b-icon> Logout
            </b-dropdown-item>
          </b-dropdown>

        </div>
      </div>
    </div>
    <div class="content">
        <router-view></router-view>

    </div>
  </div>
</template>

<script>
export default {
    data() {
    return {
      fullname: "Anucha Srilachai",
      image_profile:
        "https://static01.nyt.com/newsgraphics/2020/11/12/fake-people/4b806cf591a8a76adfc88d19e90c8c634345bf3d/fallbacks/mobile-05.jpg",
    };
  },
};
</script>

<style>
.topnav {
  padding: 20px;
  display: flex;
  background-color: #43435e;
  justify-content: space-between;
}
.content {
  height: 92.5%;
}
.logo {
  color: white;
  font-size: 30px;
}




</style>