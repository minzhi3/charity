<template>
  <el-container>
    <el-header class="header">
      <Header/>
    </el-header>
    <el-container>
      <el-aside width="200px">
        <NavMenu/>
      </el-aside>
      <el-main>
        <div class="content">
          <div class="section">
            <router-view></router-view>
          </div>
        </div>
      </el-main>
    </el-container>
  </el-container>
</template>

<script>
import NavMenu from '@/components/NavMenu'
import Header from '@/components/Header'

export default {
  name: 'main',
  components: {
    NavMenu,
    Header
  },
  computed: {

  }
}

</script>

<style>
.header {
  background-color: #409EFF;
  color: #fff;
  line-height: 60px;
}
</style>