# SmartDirector - Project Page (website branch)

This branch hosts the project page for [SmartDirector](https://orange-3dv-team.github.io/SmartDirector/).

GitHub Pages 会从此分支的根目录部署 `index.html`。

---

## 目录结构

```
website/
├── index.html          # 项目主页
├── README.md           # 本文件
└── assets/             # 所有媒体资源（视频、图片）
    ├── logo.png        # 网页顶部 Logo
    ├── teaser/
    │   └── teaser_0.mp4
    ├── single_frame/
    │   ├── first_case2/    # first_frame2.png, first_video2_切镜.mp4
    │   ├── first_case3/    # first_frame3_v2.png, first_video3_v2.mp4
    │   ├── last_case3/     # last_frame3_v2.png, last_video3_v2.mp4
    │   ├── last_case5/     # last_frame5_v1.png, last_video5_v1.mp4
    │   ├── mid_case1/      # mid_frame1_v1_ref41.png, 0_[41]_18_ck3000_step4_blur6_seed253.mp4
    │   └── mid_case2/      # mid_frame2_v2_ref97.png, 3_[97]_30_ck3000_step4_blur6_seed411.mp4
    ├── multi_frame/
    │   ├── case1/          # NO1~7.jpeg, v2_狐狸甜点.mp4
    │   ├── case2/          # 小孩河马1~9.png/jpeg, v2_饼干碎屑.mp4
    │   ├── case3/          # 2D手绘1~7.jpeg/png, v2_星空隧道.mp4
    │   ├── case4/          # NO1~8.jpg/png, 虎鲸家书2_HR_step12.mp4
    │   ├── case5/          # single_shot_263_ref*.png, 263_HR.mp4
    │   └── case6/          # single_shot_172_ref*.png, 172_[25,74,99]_00_HR.mp4
    ├── pacing_control/
    │   ├── NO1.png, NO2.png, NO3.png
    │   ├── ACTION.mp4
    │   ├── DOCUMENTARY.mp4
    │   └── SUSPENSE.mp4
    ├── video_extend/
    │   ├── 两边生中间.mp4
    │   ├── 前生后.mp4
    │   └── 后生前.mp4
    └── SR/
        ├── case1/          # ori.mp4, Ours.mp4, SparkVSR.mp4
        └── case2/          # ori.mp4, Ours.mp4, SparkVSR.mp4
```

---

## 如何上传资源

本地 `video/` 目录的文件对应 `assets/` 目录（结构一致，只是文件夹名不同）。

```bash
# 1. 切到 website 分支
git checkout website

# 2. 将本地 video 文件夹内容复制到 assets（保持结构）
cp -r /path/to/video/* assets/

# 3. 单独放 logo
cp /path/to/logo.png assets/logo.png

# 4. 提交并推送
git add assets/
git commit -m "Add media assets"
git push origin website
```

> ⚠️ GitHub 单文件限制 100MB，单次 push 建议不超过 2GB。如果视频太大可以用 Git LFS。

---

## GitHub Pages 配置

在仓库 Settings → Pages 中设置：
- **Source**: Deploy from a branch
- **Branch**: `website` / `/ (root)`

部署后访问：https://orange-3dv-team.github.io/SmartDirector/
