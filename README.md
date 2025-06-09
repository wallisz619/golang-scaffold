## 项目目录结构

```bash
.
├── app
│   └── http
│       └── middlewares
│           ├── logger.go           # 日志中间件
│           └── recovery.go         # 恐慌恢复中间件
├── bootstrap
│   ├── database.go                 # 数据库初始化
│   ├── logger.go                   # 日志系统初始化
│   └── route.go                    # 路由注册
├── config
│   ├── app.go                      # 应用级配置
│   ├── config.go                   # 配置加载逻辑
│   ├── database.go                 # 数据库相关配置
│   └── log.go                      # 日志相关配置
├── go.mod                          # Go Module 文件
├── go.sum                          # Go Module 校验文件
├── main.go                         # 应用主入口
├── pkg
│   ├── app
│   │   └── app.go                  # 应用工具类
│   ├── config
│   │   └── config.go               # 配置处理封装
│   ├── database
│   │   └── database.go             # 数据库封装操作
│   ├── helpers
│   │   └── helpers.go              # 通用辅助函数
│   └── logger
│       └── logger.go               # 日志封装
├── routes
│   └── api.go                      # 路由定义
├── storage
│   └── logs
│       └── logs.log                # 应用运行日志
└── tmp
    ├── air.log                     # Air 工具热重载日志
    └── main                        # 临时文件/缓存