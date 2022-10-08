<template>
  <el-table
    :data="tableData"
    style="width: 100%">
    <el-table-column
      prop="date"
      label="钟宏伟"
      width="180">
    </el-table-column>
    <el-table-column
      prop="name"
      label="男"
      width="180">
    </el-table-column>
    <el-table-column
      prop="address"
      label="202026702171">
    </el-table-column>
  </el-table>
</template>

<script>
  export default {
    data() {
      return {
        tableData: [ {
          date: 'QQ:3087591062',
          name: '邮箱：3087591062@qq.com',
          address: '手机号：15390722388'
        }]
      }
    }
  }
</script>
