# editor
文字编辑器插件
import makedownplugin from '@/plugin/makedown'
Vue.use(makedownplugin)

全局注册了以后，可以在任何一个页面上引用组件
<template>
    <div>
        <markdown @getData="getdata">
          <!--这是插槽-->
        </markdown>
    </div>
</template>

@getData有两个参数，传递了编辑器的内容，和选中文本。得到了选中文本，就可以对插件进行拓展。
