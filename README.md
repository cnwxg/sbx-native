# Sbx Native

本仓库提供不同运行环境的 sing-box native 启动器，用于部署 VMess Ws + Argo、VLESS Reality、Hysteria2、TUIC、AnyTLS、SOCKS5 等代理，只有主进程，没有子进程。

请选择对应环境查看说明：

| 环境 | 说明文档 | 入口文件 |
| --- | --- | --- |
| Node.js | [NODE.md](NODE.md) | [nodejs/index.js](nodejs/index.js) |
| Python | [PYTHON.md](PYTHON.md) | [python/app.py](python/app.py) |

## 目录结构

```text
.
├── nodejs/
│   ├── index.js
│   └── package.json
├── python/
│   ├── app.py
│   └── requirements.txt
├── NODE.md
├── PYTHON.md
└── README.md
```

## 简要说明

- Node.js 版本使用 `koffi` 加载 `.so` 动态库。
- Python 版本使用 `ctypes` 加载 `.so` 动态库。
- 两个版本均应部署在 Linux `amd64` 或 `arm64` 环境运行。

详细安装、启动、环境变量和协议说明请查看对应环境文档。
