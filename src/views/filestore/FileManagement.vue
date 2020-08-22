<template>
  <div class="file-management-container">
    <el-card>
      <el-upload class="upload-demo"
                 drag
                 :action="uoloadURL"
                 multiple>
        <i class="el-icon-upload" />
        <div class="el-upload__text">将文件拖到此处，或<em>点击上传</em></div>

      </el-upload>
    </el-card>

  </div>
</template>

<script>
export default {
  data () {
    return {
      uoloadURL: 'http://localhost:9000/api/file/upload'
    }
  }

}
</script>

<style scoped>
</style>
