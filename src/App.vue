
<template>
  <div>
    <el-button>默认按钮</el-button>
  </div>
</template>

<script>
import { getListAPI } from '@/api'
export default {
  created () {
    this.getListFn()
  },
  methods: {
    async getListFn () {
      const res = await getListAPI()
      console.log(res)
    }
  }
}

</script>

<style lang="less" scoped>
</style>
