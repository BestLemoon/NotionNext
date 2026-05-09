# 上游新增配置说明

这份文件记录本次从 `tangly1024/NotionNext` 同步到当前 fork 时吸收进来的主要新增配置项，方便后续按需调整。

## 根配置

- `blog.config.js`
  - `API_BASE_URL`：Notion API 请求地址，默认走 `https://www.notion.so/api/v3`，需要代理或自建接口时可以改。
  - `BEI_AN_GONGAN`：公安备案号配置，用于页脚或备案组件展示。
  - `conf/performance.config`：新增性能优化配置入口。
  - `conf/top-tag.config`：新增全局置顶标签配置入口。
  - `conf/techgrow.config`：新增 TechGrow 公众号导流/阅读全文插件配置入口。

## `conf` 配置文件

- `conf/analytics.config.js`
  - `UMAMI_HOST`：Umami 统计服务地址。
  - `UMAMI_ID`：Umami 网站统计 ID。
- `conf/code.config.js`
  - `CODE_COLLAPSE_MIN_LINES`：代码块超过多少行时启用折叠。
- `conf/comment.config.js`
  - `COMMENT_GISCUS_CATEGORY`：Giscus 评论使用的 GitHub Discussion 分类。
  - `COMMENT_GISCUS_STRICT`：Giscus 严格匹配模式开关。
- `conf/font.config.js`
  - `FONT_DISPLAY`：字体加载显示策略，例如 swap/block。
  - `FONT_PRELOAD`：是否预加载字体。
  - `FONT_SUBSET`：字体子集配置，用于减少字体资源体积。
- `conf/image.config.js`
  - `IMAGE_COMPRESS_QUALITY`：图片压缩质量。
- `conf/post.config.js`
  - `LATEST_POST_COUNT`：最新文章展示数量。
- `conf/performance.config.js`
  - 新文件：集中配置预加载、图片懒加载、缓存时间、压缩、WebP/AVIF、链接预取和 Web Vitals 性能预算。
- `conf/techgrow.config.js`
  - 新文件：配置 TechGrow 阅读更多/公众号导流能力，包括博客 ID、二维码、关键词、白名单和黄色名单等。
- `conf/themeSwitch.manifest.js`
  - 新文件：主题切换面板使用的主题元信息，例如主题名称、分组、预览图和推荐级别。
- `conf/top-tag.config.js`
  - `TOP_TAG`：全局置顶标签，通常用于把某个标签下的文章优先展示。

## 主题配置

- `themes/heo/config.js`
  - `HEO_HERO_RECOMMEND_COVER_ENABLE`：控制 Heo 首页英雄区右侧推荐文章是否显示遮罩图；本次保留了你的 `HERO_RECOMMEND_COVER`，并补入这个开关。
- `themes/claude/config.js`
  - 新文件：Claude 主题配置，覆盖菜单、目录、头像、页脚、README 缓存和贡献数据等。
- `themes/endspace/config.js`
  - 新文件：Endspace 主题配置，覆盖加载页、菜单、文章布局、列表封面、悬浮控件和暗色模式等。
- `themes/fuwari/config.js`
  - 新文件：Fuwari 主题配置，覆盖菜单、首页 Hero、侧边栏组件、主题色、联系卡片、文章页布局和动效等。
- `themes/magzine/config.js`
  - `MAGZINE_HERO_SUB_POST_COUNT`：Magzine 主题首页 Hero 区附属文章数量。
- `themes/proxio/config.js`
  - 新增大量落地页配置，覆盖 Hero、博客区、公告、特性、招聘、评价、FAQ、关于、品牌、页脚、CTA 和文章重定向等区域。

## 本地配置保留情况

- `blog.config.js`
  - 保留本地 `LINK: https://blog.chillwaytech.com`。
  - 保留已有图片、字体、分享、动画、挂件和路由映射等个性配置。
- `themes/heo/config.js`
  - 保留建站日期、通知链接、首页 Hero 文案、分类标签、右侧推荐图、个人资料链接和社交卡片开关。
- `public/favicon.ico`
  - 保留本地 favicon。

