# Personal Website — Guangxiao Yang

## 文件结构

```
index.html              ← 主页
style.css               ← 样式
assets/
  humanoid_long_jump.mp4   ← 全尺寸人形跳远
  humanoid_high_jump.mp4   ← 全尺寸人形跳高
  humanoid_demo.mp4        ← 主 demo（2025）
```

## 1. 创建 GitHub 仓库

仓库名必须完全等于 `nuliguangxiaoyang-crypto.github.io`。

```
https://github.com/new
Repository name: nuliguangxiaoyang-crypto.github.io
Visibility: Public
```

## 2. 推送文件

```bash
cd /path/to/github-pages
git init
git remote add origin git@github.com:nuliguangxiaoyang-crypto/nuliguangxiaoyang-crypto.github.io.git
git add .
git commit -m "init personal website"
git push -u origin main
```

## 3. 启用 GitHub Pages

仓库 → Settings → Pages → Source: **Deploy from a branch** → Branch: `main / (root)` → Save

约 1 分钟后访问：`https://nuliguangxiaoyang-crypto.github.io`

## 4. 必须修改的内容（打开 index.html）

| 占位符 | 替换为 |
|--------|--------|
| `YOUR_EMAIL@example.com` | 你的真实邮箱（两处） |
| About 段落 | 你的真实背景和单位 |
| Demo 描述文字 | 对应视频的准确说明 |

## 5. 可选：添加头像

把照片命名为 `photo.jpg` 放入 `assets/`，然后取消 `index.html` 中这行注释：
```html
<!-- <img src="assets/photo.jpg" alt="Guangxiao Yang" class="avatar" /> -->
```

## 6. 在 OpenReview 填写 HomePage URL

```
https://nuliguangxiaoyang-crypto.github.io
```

## 注意：37MB 视频文件

`humanoid_demo.mp4` 为 37MB，GitHub 普通仓库支持单文件最大 100MB，可以正常推送。
但如果后续添加更多大文件建议改用 [Git LFS](https://git-lfs.com/)，或将视频上传到 B 站/YouTube 再嵌入 iframe。
