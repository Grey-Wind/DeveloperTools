<script setup>
import IntroduceItem from './IntroduceItem.vue'
import SupportIcon from '../icons/IconSupport.vue'
import ImageConverter from './element/ImageConverter.vue'
import DocumentConverterIcon from '../icons/IconDocumentConverter.vue'
import CodeIcon from '../icons/IconCode.vue'
import ColorPaletteIcon from '../icons/IconColorPalette.vue'
</script>

<template>
  <ImageConverter />

  <IntroduceItem>
    <template #icon>
      <DocumentConverterIcon />
    </template>
    <template #heading>
      <RouterLink to="/convert/document">文档转换器</RouterLink>
    </template>
    <p>文档转换器可以快速将不同类型的文档转换成您所需要的格式。</p>
    <p>例如将Word文档或Excel表格转换为PDF。</p>
  </IntroduceItem>

  <IntroduceItem>
    <template #icon>
      <CodeIcon />
    </template>
    <template #heading>在线代码运行器</template>
    <p>一个类似于<a href="https://www.runoob.com/">菜鸟教程</a>的代码在线示例运行工具</p>
  </IntroduceItem>

  <IntroduceItem>
    <template #icon>
      <ColorPaletteIcon />
    </template>
    <template #heading>Community</template>

    Got stuck? Ask your question on
    <a href="https://chat.vuejs.org" target="_blank" rel="noopener">Vue Land</a>, our official
    Discord server, or
    <a href="https://stackoverflow.com/questions/tagged/vue.js" target="_blank" rel="noopener">StackOverflow</a>. You
    should also subscribe to
    <a href="https://news.vuejs.org" target="_blank" rel="noopener">our mailing list</a> and follow
    the official
    <a href="https://twitter.com/vuejs" target="_blank" rel="noopener">@vuejs</a>
    twitter account for latest news in the Vue world.
  </IntroduceItem>

  <IntroduceItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Support Vue</template>

    As an independent project, Vue relies on community backing for its sustainability. You can help
    us by
    <a href="https://vuejs.org/sponsor/" target="_blank" rel="noopener">becoming a sponsor</a>.
  </IntroduceItem>
</template>
