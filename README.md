# getx_fix

在 `getx` 的一些特定版本上，同步修复了一些问题。

> 注：由于 [getx](https://github.com/jonataslaw/getx) 缺失一些相应版本的 `tag`，如  `4.6.6`，所以代码取自 https://pub.dev/packages/get/versions 并上传

## ☕ 请我喝一杯咖啡

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/T6T4JKVRP) [![wechat](https://img.shields.io/static/v1?label=WeChat&message=微信收款码&color=brightgreen&style=for-the-badge&logo=WeChat)](https://cdn.jsdelivr.net/gh/FullStackAction/PicBed@resource20220417121922/image/202303181116760.jpeg)

微信技术交流群请看: [【微信群说明】](https://mp.weixin.qq.com/s/JBbMstn0qW6M71hh-BRKzw)

## 使用

在 `pubspec.yaml` 中的 `dependency_overrides` 下重写 `get` 依赖。

```yaml
dependencies:
  get: any

dependency_overrides:
  get:
    git:
      url: https://github.com/LinXunFeng/getx_fix.git
      ref: 4.6.6_fix
```

## 分支说明
### 4.6.6_fix

- 修复内存泄漏 ([getx/2626](https://github.com/jonataslaw/getx/pull/2626)、[getx/3141](https://github.com/jonataslaw/getx/pull/3141))
- 支持 `PopScope` ([getx/3049](https://github.com/jonataslaw/getx/pull/3049))

### 4.6.6
原 `4.6.6` 代码，仅同步
