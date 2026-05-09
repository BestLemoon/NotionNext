# Upstream config additions

This file records notable config entries added while syncing from upstream `tangly1024/NotionNext` to this fork.

## Root config

- `blog.config.js`
  - `API_BASE_URL`
  - `BEI_AN_GONGAN`
  - added `conf/performance.config`
  - added `conf/top-tag.config`
  - added `conf/techgrow.config`

## `conf` config files

- `conf/analytics.config.js`
  - `UMAMI_HOST`
  - `UMAMI_ID`
- `conf/code.config.js`
  - `CODE_COLLAPSE_MIN_LINES`
- `conf/comment.config.js`
  - `COMMENT_GISCUS_CATEGORY`
  - `COMMENT_GISCUS_STRICT`
- `conf/font.config.js`
  - `FONT_DISPLAY`
  - `FONT_PRELOAD`
  - `FONT_SUBSET`
- `conf/image.config.js`
  - `IMAGE_COMPRESS_QUALITY`
- `conf/post.config.js`
  - `LATEST_POST_COUNT`
- `conf/performance.config.js`
  - new file for preload, lazy loading, cache TTL, compression, image format, prefetch, and Web Vitals budget settings
- `conf/techgrow.config.js`
  - new file for TechGrow read-more / public-account diversion settings
- `conf/themeSwitch.manifest.js`
  - new file for theme switch metadata
- `conf/top-tag.config.js`
  - `TOP_TAG`

## Theme config

- `themes/heo/config.js`
  - `HEO_HERO_RECOMMEND_COVER_ENABLE`
- New theme config files added by upstream:
  - `themes/claude/config.js`
  - `themes/endspace/config.js`
  - `themes/fuwari/config.js`
- Other notable theme additions:
  - `themes/magzine/config.js`: `MAGZINE_HERO_SUB_POST_COUNT`
  - `themes/proxio/config.js`: many new landing-page section controls, including hero, blog, announcement, feature, career, testimonials, FAQ, about, brands, footer, CTA, and redirect settings

## Local config preserved

- `blog.config.js`
  - local `LINK` stays `https://blog.chillway.me`
  - existing local image, font, share, animation, widget, and route mapping config is retained
- `themes/heo/config.js`
  - local site creation date, notice links, hero text, category labels, hero cover, profile links, and social card setting are retained
- `public/favicon.ico`
  - local favicon is retained

