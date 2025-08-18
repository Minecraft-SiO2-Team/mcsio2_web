# 二氧化硅生存服务器官网

本项目为"二氧化硅生存服务器"官方主页，基于 HTML+CSS+JavaScript 实现，界面美观，内容丰富，适合 Minecraft 服务器展示与推广。

## 主要功能
- **首页**：展示服务器名、版本、特点、联系方式、服务器IP与QQ群号，实时显示在线玩家数。
- **规则页**：支持 Markdown 格式渲染，带有可折叠目录侧边栏，便于玩家查阅服务器规则。
- **管理组页**：展示管理团队成员信息与头像，结构清晰。
- **更新日志页**：展示服务器更新历史，支持 Markdown 格式，带有侧边栏导航。
- **访客统计**：使用不蒜子统计服务，实时显示今日访客数和总访客数。
- **响应式设计**：完美适配PC与移动端设备。
- **页脚统一**：展示版权信息、GitHub 项目地址和访客统计。

## 文件结构
```
mcsio2_web/
├── index.html          # 首页
├── rules.html          # 规则页面
├── team.html           # 管理组页面  
├── changelog.html      # 更新日志页面
├── style.css           # 全站样式
├── README.md           # 项目说明
├── CNAME              # 域名配置
├── images/            # 图片资源
│   └── bg.png         # 背景图片
├── js/                # JavaScript 文件
│   ├── status.js      # 服务器状态检测
│   ├── rules.js       # 规则页面逻辑
│   └── changelog.js   # 更新日志页面逻辑
├── docx/              # 文档文件
│   ├── rules.md       # 规则内容（Markdown格式）
│   └── changelog.md   # 更新日志内容（Markdown格式）
└── .github/           # GitHub 工作流
    └── workflows/
        └── release.yml # 自动部署配置
```

## 技术特性
- **前端框架**：纯 HTML+CSS+JavaScript，无依赖框架
- **Markdown 渲染**：使用 [marked.js](https://marked.js.org/) 进行 Markdown 解析
- **访客统计**：集成[不蒜子](https://busuanzi.cc/)统计服务
- **响应式布局**：适配各种屏幕尺寸
- **自动部署**：通过 GitHub Pages 自动部署

## 快速部署
1. **克隆本仓库**：
   ```bash
   git clone https://github.com/x1aoren/mcsio2_web.git
   cd mcsio2_web
   ```
2. **本地预览**：
   ```bash
   # Python 3
   python -m http.server 8080
   
   # Node.js 
   npx http-server -p 8080
   
   # 或使用 VSCode Live Server 插件
   ```
3. **访问网站**：浏览器打开 `http://localhost:8080`

> **注意：** 由于使用了 fetch API 加载 Markdown 文件，必须通过 HTTP 服务器访问，直接打开 HTML 文件会因跨域限制无法正常使用。

## 自定义配置
- **修改服务器信息**：编辑 `index.html` 中的服务器IP、QQ群等信息
- **更新规则内容**：编辑 `docx/rules.md` 文件
- **添加更新日志**：编辑 `docx/changelog.md` 文件
- **修改管理团队**：编辑 `team.html` 中的成员信息
- **自定义样式**：修改 `style.css` 文件

## 在线预览
- 官方网站：[https://x1aoren.github.io/mcsio2_web/](https://x1aoren.github.io/mcsio2_web/)

## 贡献与反馈
- 欢迎提交 Issue 和 Pull Request！
- GitHub 仓库：[https://github.com/x1aoren/mcsio2_web](https://github.com/x1aoren/mcsio2_web)
- 如有问题或建议，请创建 Issue 或联系项目维护者

## 版权声明
本项目采用 MIT 许可证，内容归"二氧化硅生存服务器"所有，仅供学习交流使用。 