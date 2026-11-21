# 春雪云仓库 · 公共更新源

本仓库只存放春雪云仓库 Windows 便携版安装包和 `latest.json`，不放源码。

## 文件

- `wms-windows-portable.zip`：Windows x64 便携包
- `latest.json`：更新清单，客户端通过 `releases/latest/download/latest.json` 读取

## 更新清单格式

```json
{
  "version": "1.3.1",
  "notes": "更新说明",
  "url": "https://github.com/fangcun11/chunxue-wms-releases/releases/download/latest/wms-windows-portable.zip",
  "sha256": "64 位十六进制 SHA-256",
  "size": 65000000,
  "publishedAt": "2026-11-21T00:00:00.000Z"
}
```

客户端会校验 SHA-256，下载后下次启动时替换 `app/` 和 `public/`，保留 `data/`。
