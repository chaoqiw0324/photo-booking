# 摄影约拍网页

## 本地预览
直接双击 `index.html` 在浏览器中打开即可。

## 部署到 GitHub Pages

```bash
# 1. 在 GitHub 上新建一个仓库（比如叫 photo-booking）

# 2. 在本地初始化并推送
cd photo-booking
git init
git add .
git commit -m "init"
git branch -M main
git remote add origin https://github.com/你的用户名/photo-booking.git
git push -u origin main

# 3. 开启 GitHub Pages
#    进入仓库 → Settings → Pages → Source 选 "main" 分支 → Save
#    几分钟后访问：https://你的用户名.github.io/photo-booking/
```

## 修改内容

打开 `index.html`，找到顶部的 `DATA` 对象：

- **改工作室信息**：修改 `studioName`、`subtitle`、`contacts`
- **增减器材**：在 `equipment` 数组中添加/删除条目
- **更新库存**：修改 `films` 中对应相纸的 `stock` 数字（设为 0 = 显示缺货，仍然展示）
- **替换客片**：将图片放在同目录下的 `photos/` 文件夹，`samples` 中填 `"photos/xxx.jpg"`

修改后 `git add . && git commit -m "update" && git push` 即可自动更新网站。
