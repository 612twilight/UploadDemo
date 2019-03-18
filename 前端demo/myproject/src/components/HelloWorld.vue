<template>
  <div>
    <el-upload
      class="upload-demo"
      action="http://127.0.0.1:8888/uploadFile/"
      name="file"
      :multiple="false"
      :limit=1
      :show-file-list="false"
    >
      <div class="classBox fucBox" @click="addArticle">
        <i class="el-icon-plus" style="font-size: 70px;margin-left: 14px;margin-top: 20px"></i>
        <p style="margin-top: 40px;margin-left: 12px">文书新增</p>
      </div>
    </el-upload>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .fucBox{
    margin-left: 200px;
  }

  .classBox{
    height: 200px;
    width: 200px;
    float: left;
    cursor: pointer;
    margin-left: 200px;
  }
  .classBox:hover
  {
    background-color:grey;
  }
</style>
