# 俄罗斯文学的流动画廊

保留已确认预览版的界面、图片和交互，用于新建 GitHub 仓库与 Cloudflare Workers 网站。

## 上传
解压 ZIP，将文件夹里面的全部文件和子文件夹拖入 GitHub 上传区域；不要上传 ZIP 本身。仓库根目录应直接看到 package.json、wrangler.jsonc、src、public、scripts。完成后点击 Commit changes。

## Cloudflare Workers
- Project name: literature-gallery
- Build command: npm run build
- Deploy command: npx wrangler deploy
- 根目录：默认仓库根目录

更改项目名时请同步修改 wrangler.jsonc 的 name。

## 本地预览
需要 Node.js 20 或更高版本。运行 npm run dev，打开 http://localhost:4173/。

src 为源码，public 为图片和字体，scripts 为构建与预览脚本。dist 在构建时自动生成，因此本包不重复包含。
中文采用随包思源黑体；Franie 仅在设备安装该字体时使用，否则使用备用字体。本包不包含商业 Franie 字体。
