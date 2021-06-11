<template>
  <div class="row">
    <div class="col-4">
      <div class="list-group">
        <router-link to="/newpage/a" class="list-group-item list-group-item-action">
          元件 A
        </router-link>
      </div>
      <div class="list-group">
        <router-link to="/newpage/b" class="list-group-item list-group-item-action">
          元件 B
        </router-link>
      </div>
      <div class="list-group">
        <router-link to="/newpage/namedview/ab" class="list-group-item list-group-item-action">
          命名視圖 AB
        </router-link>
      </div>
      <div class="list-group">
        <router-link to="/newpage/namedview/ca" class="list-group-item list-group-item-action">
          命名視圖 CA
        </router-link>
      </div>
      <div class="list-group">
        <router-link to="/newpage/dynamicRouter/51f9c4fb635a92aa" class="list-group-item list-group-item-action">
          動態路由
        </router-link>
      </div>
      <div class="list-group">
        <router-link to="/newpage/dynamicRouterByProps/51f9c4fb635a92aa" class="list-group-item list-group-item-action">
          動態路由 Props
        </router-link>
      </div>
      <div class="list-group">
        <router-link to="/newpage/routerNavigation" class="list-group-item list-group-item-action">
          路由導覽
        </router-link>
      </div>
    </div>
    <div class="col-8">
      <router-view></router-view>
    </div>
  </div>
</template>
