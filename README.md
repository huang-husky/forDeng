# forDeng

一封给邓老师的信。单文件静态页面，无需构建。

- 信件正文经 PBKDF2 + AES-GCM 加密后内嵌于 `index.html`，源码中不含明文，密码即解密密钥。
- 字体：`text.ttf`（字魂125号-九州真书），通过 @font-face 本地加载。
- 背景音乐：`bg.flac`（无损）。播放器按 `bg.flac` → `bg.mp3` → `bg.ogg` 的顺序自动选择可用音源。
- 修改信件内容：编辑 `../letter contexts/forDeng/letter-content.html`，然后在该目录运行 `node update-letter.js <密码>`（明文与工具不在本目录，勿将其发布到公开仓库）。
- 正文以"落墨"效果逐字显现（非机械打字机）：字与字间隔带随机抖动，标点处停顿更长；点击信纸任意处可跳过动画直接显示全文。
