# 蒋涛祝你立冬快乐 🎐

一封落在初雪里的信：点击信封 → 火漆揭开、白光一闪 → 满屏 3D 文字与雪花迎面飘来，配一段冬日 BGM。

**在线地址**：https://bird-liu.github.io/jiangtao-lidong/

![首屏](preview-intro.png)

## 效果

- 首屏：深蓝夜色 + 漫天小雪，中间一封带火漆的信，标题「蒋涛祝你立冬快乐」
- 点击后：信封翻开、白光闪屏，3D 雪花 / 饺子 / 红手套 / 爱心 / 祝福文字从远处扑面而来
- 背景音乐 22 秒循环；右下角可「↻ 再看一次」；支持回车/空格拆信、`prefers-reduced-motion`
- 纯静态、无构建、无第三方依赖，全部资源本地化

## 本地预览

直接双击 `index.html`，或起一个静态服务：

```bash
python -m http.server 8080
# 打开 http://localhost:8080
```

## 自定义

| 想改什么 | 改哪里 |
| --- | --- |
| 祝福语（第一行即开场） | `index.html` 中 `const LETTER = [...]` |
| 信封大字 | `<p class="env-title" id="tEnvTitle">` |
| 背景音乐 | 替换 `assets/bgm.m4a` |
| 配色 | `:root` 的 `--night` / `--plum` / `--ember` |

## 部署

仓库已开启 GitHub Pages（`main` 分支根目录），推送到 `main` 后会自动发布，约 1 分钟生效。

## 说明

页面复刻自 `5b5b.top/3374`（立冬 · 3D 飘雪信封模板），仅作个人祝福页使用；原模板的插画、动效与音乐版权归原作者/原站所有。
