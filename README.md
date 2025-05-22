# the-blog

**现代全栈博客系统**，基于前后端分离架构，包含完整的内容管理、用户认证、评论互动和监控运维能力。

## 项目结构
```
blog-platform/
├── frontend/       # 前台子模块（Vite + Element Plus）
├── backend/        # 后台子模块（Flask + SQLAlchemy）
└── infra/          # 监控运维子模块（Prometheus + Grafana）
```

## 快速开始
```bash
# 克隆主仓库并初始化子模块
git clone --recurse-submodules https://github.com/Jack-samu/the-blog.git
cd the-blog

# 初始化所有子模块
git submodule update --init --recursive
```

## 子仓库(监控部分还没有实现)
| 模块       | 技术栈                          | 文档链接                         |
|------------|---------------------------------|----------------------------------|
| 前台       | Vite + Pinia + Element Plus    | [前端文档](./frontend/README.md) |
| 后台       | Flask + SQLAlchemy + JWT       | [后端文档](./backend/README.md)  |
| 监控运维   | Prometheus + Grafana + Docker  | [运维文档](./infra/README.md)    |

## 核心特性
- **全栈技术**：前后端分离 + RESTful API 设计
- **高性能**：异步任务队列 + Redis 缓存(待实现)
- **可观测性**：完整的监控告警体系
- **安全可靠**：JWT 认证 + 密码加密存储


