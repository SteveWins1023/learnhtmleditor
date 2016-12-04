<template>
    <div id="app">
        <div id="wrapper">
            <div id="topnav">
                <router-link to="/">
                    <h2 class="admin_title">{{ adminTitle }}</h2>
                </router-link>
            </div>
            <div id="bodywrap">
                <div id="menulist">
                    <el-menu mode="vertical" theme="dark">
                        <el-menu-item-group title="Basic">
                            <router-link to="/editor">
                                <el-menu-item index="39"><i class="el-icon-edit"></i>Editor 编辑器</el-menu-item>
                            </router-link>
                        </el-menu-item-group>
                    </el-menu>
                </div>
                <router-view></router-view>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data () {
        return {
            adminTitle: 'YourAdmin'
        }
    },
    methods: {

    }
}
</script>
<style src="./main.less" lang="less"></style>









