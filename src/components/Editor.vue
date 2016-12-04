<template>
	<div class="content">
        <div class="pagetitle">
        	<div class="pagenav">
	            <el-breadcrumb separator="/">
	                <el-breadcrumb-item :to="{ path: '/' }">后台首页</el-breadcrumb-item>
	                <el-breadcrumb-item>Editor 编辑器</el-breadcrumb-item>
	            </el-breadcrumb>
	        </div>
            <div class="pageactions">
                <!-- 页面操作这里添加 -->
            </div>
        </div>
        <div class="pagecontent">
             <h2>Editor 编辑器</h2>
            <htmleditor :content.sync="content" :height="500" :z-index="1000" :auto-height="true">
            </htmleditor>

        </div>
    </div>
</template>
<script type="text/javascript">

	export default {
		data () {
			return {
				content: ""	
			}
		}
	}
</script>

<style type="text/css" lang="less" scoped>

</style>