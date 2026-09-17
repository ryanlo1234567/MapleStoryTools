<template>
  <n-layout-footer bordered class="site-footer">
    <n-space vertical size="small">
      <n-text depth="3" class="site-footer-line">
        本頁為原始專案的靜態重新發佈版本，所有功能皆在瀏覽器本機執行，不會上傳任何資料。
      </n-text>
      <n-text depth="3" class="site-footer-line">
        原始專案：<n-a :href="repoUrl" target="_blank" rel="noopener noreferrer">lintx/MapleStoryTools</n-a>
        ｜原作者：lintx
        ｜授權：MIT License
      </n-text>
      <n-text depth="3" class="site-footer-line">Copyright (c) 2019 lintx</n-text>
      <n-collapse>
        <n-collapse-item title="MIT License 全文" name="license">
          <n-text depth="3"><pre class="site-footer-license">{{ license }}</pre></n-text>
        </n-collapse-item>
      </n-collapse>
    </n-space>
  </n-layout-footer>
</template>

<script setup>
const repoUrl = "https://github.com/lintx/MapleStoryTools"
const license = `MIT License

Copyright (c) 2019 lintx

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.`
</script>

<style scoped>
.site-footer {
  padding: 20px 24px;
}

.site-footer-line {
  font-size: 12px;
  line-height: 1.8;
}

.site-footer-license {
  font-size: 11px;
  line-height: 1.6;
  white-space: pre-wrap;
  word-break: break-word;
  margin: 0;
  font-family: inherit;
}
</style>
