# 🌌 粒子生命模拟项目网站

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Active%20Development-brightgreen.svg)

**从简单规则中涌现复杂生命的可视化展示平台**

[在线演示](#-在线演示) • [项目特性](#-项目特性) • [技术架构](#-技术架构) • [快速开始](#-快速开始) • [贡献指南](#-贡献指南)

</div>

## 📋 项目简介

**粒子生命模拟项目网站**是一个基于现代Web技术构建的交互式展示平台，专门用于展示和演示粒子生命模拟的奇妙现象。通过简单的吸引和排斥规则，模拟原子般粒子间的相互作用，从而产生复杂的自组织类生命模式。

> **核心理念**：从简单性中涌现复杂性，探索人工生命的奥秘

### 🎯 项目背景
- **网站开发**：Deepseek / 玄曦雪
- **核心算法**：基于 [hunar4321/particle-life](https://github.com/hunar4321/particle-life)
- **灵感来源**：Jeffery Ventrella的Clusters项目
- **许可证**：MIT License

---

## ✨ 项目特性

### 🎨 现代化设计
| 特性 | 描述 | 状态 |
|------|------|------|
| 响应式设计 | 完美适配桌面和移动设备 | ✅ 完成 |
| 粒子背景 | 动态粒子动画和连接效果 | ✅ 完成 |
| 暗色主题 | 科学可视化风格的界面设计 | ✅ 完成 |
| 平滑交互 | 流畅的动画和过渡效果 | ✅ 完成 |

### 📚 内容展示
| 模块 | 功能 | 特点 |
|------|------|------|
| 在线演示 | 2D/3D粒子生命模拟链接 | 直接体验核心功能 |
| 代码展示 | 多语言实现代码对比 | JavaScript/C++/Python |
| 使用指南 | 详细的使用说明和编译指南 | 面向不同用户群体 |
| 版本生态 | 丰富的第三方移植版本 | 社区贡献展示 |

### 🔧 技术特色
- **现代前端栈**：HTML5 + TailwindCSS + 原生JavaScript
- **性能优化**：Canvas粒子动画，60fps流畅体验
- **代码高亮**：清晰的语法展示和代码对比
- **交互设计**：标签页切换、平滑滚动、移动端适配

---

## 🚀 在线演示

### 直接体验
<div align="center">

| 版本 | 演示链接 | 特性 | 状态 |
|------|----------|------|------|
| 🔵 2D模拟 | [https://hunar4321.github.io/particle-life/particle_life.html](https://hunar4321.github.io/particle-life/particle_life.html) | 基础粒子交互 | ✅ 在线 |
| 🟢 3D模拟 | [https://hunar4321.github.io/particle-life/particle_life_3d.html](https://hunar4321.github.io/particle-life/particle_life_3d.html) | 三维空间展示 | ✅ 在线 |

</div>

### 视频教程
📺 **完整教学视频**: [YouTube教程链接](https://youtu.be/0Kx4Y9TVMGg)
- 算法原理详解
- 参数调整技巧
- 有趣模式重现方法

---

## 🏗️ 技术架构

### 前端架构
```
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   展示层         │    │   交互层          │    │   数据层         │
│                 │    │                  │    │                 │
│ • HTML5结构     │◄──►│ • JavaScript     │◄──►│ • 静态配置      │
│ • TailwindCSS   │    │ • 事件处理        │    │ • 代码示例      │
│ • 响应式布局     │    │ • 动画控制        │    │ • 外部链接      │
└─────────────────┘    └──────────────────┘    └─────────────────┘
         │                        │                       │
         ▼                        ▼                       ▼
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   渲染层         │    │   服务层          │    │   集成层         │
│                 │    │                  │    │                 │
│ • Canvas动画    │    │ • CDN资源        │    │ • GitHub Pages  │
│ • 粒子效果       │    │ • 字体图标        │    │ • 外部演示链接   │
│ • 性能优化       │    │ • 缓存策略        │    │ • 跨域支持      │
└─────────────────┘    └──────────────────┘    └─────────────────┘
```

### 核心技术栈
| 技术 | 版本 | 用途 | 特点 |
|------|------|------|------|
| HTML5 | 标准 | 页面结构 | 语义化标签，现代API |
| TailwindCSS | 3.x | 样式框架 | 实用优先，响应式设计 |
| JavaScript | ES6+ | 交互逻辑 | 原生实现，无依赖 |
| Canvas API | 标准 | 粒子动画 | 高性能图形渲染 |
| Font Awesome | 4.7 | 图标库 | 丰富图标选择 |

### 核心算法参考

#### 粒子生命模拟原理
```javascript
// 简化的核心算法（来自原始项目）
rule = (atoms1, atoms2, g) => {
    for (let i = 0; i < atoms1.length; i++) {
        fx = 0; fy = 0;
        for (let j = 0; j < atoms2.length; j++) {
            a = atoms1[i]; b = atoms2[j];
            dx = a.x - b.x; dy = a.y - b.y;
            d = Math.sqrt(dx * dx + dy * dy);
            if (d > 0 && d < 80) {
                F = (g * 1) / d;
                fx += F * dx; fy += F * dy;
            }
        }
        a.vx = (a.vx + fx) * 0.5;
        a.vy = (a.vy + fy) * 0.5;
        a.x += a.vx; a.y += a.vy;
    }
};
```

#### 网站粒子背景实现
```javascript
class Particle {
    constructor() {
        this.x = Math.random() * canvas.width;
        this.y = Math.random() * canvas.height;
        this.size = Math.random() * 2 + 0.5;
        this.speedX = Math.random() * 0.5 - 0.25;
        this.speedY = Math.random() * 0.5 - 0.25;
    }
    
    update() {
        this.x += this.speedX;
        this.y += this.speedY;
        // 边界检测和反弹
        if (this.x < 0 || this.x > canvas.width) this.speedX *= -1;
        if (this.y < 0 || this.y > canvas.height) this.speedY *= -1;
    }
}
```

---

## 🛠️ 快速开始

### 环境要求
- **现代浏览器**：Chrome 90+, Firefox 88+, Safari 14+, Edge 90+
- **网络连接**：需要访问CDN资源（TailwindCSS、Font Awesome）
- **屏幕分辨率**：支持1024×768及以上分辨率
- **JavaScript**：需要启用JavaScript支持

### 本地部署

1. **克隆或下载项目**
```bash
# 直接下载HTML文件
wget https://raw.githubusercontent.com/your-repo/particle-life-website/main/index.html

# 或克隆整个项目
git clone https://github.com/your-repo/particle-life-website.git
cd particle-life-website
```

2. **本地运行**
```bash
# 使用Python简单服务器
python -m http.server 8000

# 或使用Node.js http-server
npx http-server

# 或直接浏览器打开
open index.html
```

3. **访问网站**
```
打开浏览器访问: http://localhost:8000
```

### 生产部署

#### GitHub Pages（推荐）
1. Fork本仓库
2. 在仓库设置中启用GitHub Pages
3. 选择main分支作为源
4. 访问 `https://your-username.github.io/repository-name`

#### 其他静态托管
- **Netlify**: 直接拖拽部署
- **Vercel**: 连接GitHub仓库自动部署
- **Cloudflare Pages**: 免费企业级托管

---

## 📖 使用指南

### 网站导航

#### 🏠 首页区域
- **英雄区块**：项目介绍和快速入口
- **动态背景**：Canvas粒子动画效果
- **行动号召**：直接跳转到演示或代码

#### 📖 内容区块
| 区块 | 内容 | 目标用户 |
|------|------|----------|
| 关于项目 | 项目背景和灵感来源 | 新用户 |
| 在线演示 | 2D/3D模拟链接 | 体验者 |
| 使用方法 | 详细使用指南 | 学习者 |
| 源代码 | 多语言代码展示 | 开发者 |
| 其他版本 | 社区移植版本 | 贡献者 |

#### 💻 代码浏览
- **标签页切换**：JavaScript、C++、Python代码对比
- **语法高亮**：清晰的代码展示
- **优化提示**：各版本的特性说明

### 功能操作

#### 移动端适配
```html
<!-- 响应式导航 -->
<nav class="fixed top-0 left-0 w-full bg-dark/80 backdrop-blur-md z-50">
    <!-- 桌面导航 -->
    <div class="hidden md:flex space-x-8">
        <!-- 导航项 -->
    </div>
    <!-- 移动端菜单切换 -->
    <button class="md:hidden text-2xl" id="menu-toggle">
        <i class="fa fa-bars"></i>
    </button>
</nav>
```

#### 交互特效
- **悬停效果**：卡片悬停动画和阴影
- **平滑滚动**：锚点链接平滑滚动
- **标签切换**：代码展示区域动态切换
- **粒子动画**：背景粒子动态效果

---

## 🌍 项目生态

### 多语言实现

| 语言 | 版本数 | 维护状态 | 特点 |
|------|--------|----------|------|
| C++ | 主版本 | ✅ 活跃 | 高性能，完整GUI |
| JavaScript | 2D/3D | ✅ 活跃 | 网页直接运行 |
| Python | 多个 | ✅ 活跃 | 易于学习修改 |
| Rust | 1个 | ✅ 活跃 | 内存安全 |
| Go | 3个 | ✅ 活跃 | 并发优化 |

### 社区移植版本

<div align="center">

| 平台/语言 | 图标 | 状态 | 特点 |
|-----------|------|------|------|
| Godot | 🎮 | ✅ 完成 | 游戏引擎集成 |
| Rust | 🦀 | ✅ 完成 | 系统级性能 |
| Go | � | ✅ 完成 | 高并发处理 |
| Lua | � | ✅ 完成 | 脚本语言版本 |
| Java | ☕ | ✅ 完成 | 跨平台运行 |
| C# Winforms | � | ✅ 完成 | Windows原生 |

</div>

---

## 🔬 科学背景

### 相关概念
- **粒子生命模拟**：基于简单规则的复杂系统
- **原始汤进化**：模拟生命起源环境
- **康威生命游戏**：经典的元胞自动机
- **自组织模式**：无序到有序的涌现现象

### 算法创新
与其他粒子生命项目相比，本实现的独特之处：
1. **无碰撞检测**：实现数千粒子实时模拟
2. **实时参数调整**：GUI控制便于探索新pattern
3. **代码简洁性**：核心算法不足百行
4. **教育友好**：适合初学者理解复杂系统

---

## 📋 开发计划

### 近期目标
- [ ] 添加参数保存/加载功能
- [ ] 支持更多粒子类型
- [ ] 优化算法性能（O(n²)问题）
- [ ] GPU加速计算

### 中期规划
- [ ] 屏幕自适应调整
- [ ] 更直观的UI控制
- [ ] 随机化按钮和元规则
- [ ] 进化算法集成

### 技术债务
- [ ] 改进边界检查机制
- [ ] 添加单元测试
- [ ] 性能分析和优化
- [ ] 代码文档完善

---

## 🤝 贡献指南

### 如何参与

#### 代码贡献
1. Fork本仓库
2. 创建功能分支：`git checkout -b feature/AmazingFeature`
3. 提交更改：`git commit -m 'Add AmazingFeature'`
4. 推送分支：`git push origin feature/AmazingFeature`
5. 创建Pull Request

#### 文档改进
- 修正拼写错误和语法问题
- 改进使用说明和示例
- 添加更多有趣模式的参数配置
- 翻译成其他语言

#### 新端口开发
欢迎使用其他编程语言或框架实现粒子生命模拟，请确保：
- 保持核心算法的一致性
- 提供清晰的编译/运行说明
- 添加适当的测试用例

### 开发规范
- 遵循各语言的代码风格指南
- 添加必要的注释和文档
- 确保向后兼容性
- 编写清晰的提交信息

---

## 📄 许可证

本项目基于 **MIT License** 开源。

**主要条款：**
- ✅ 允许商业使用
- ✅ 允许修改和分发
- ✅ 允许私有使用
- ✅ 只需保留版权声明
- ❌ 不提供责任担保

完整许可证文本请查看 [LICENSE](LICENSE) 文件。

### 引用要求
```
粒子生命模拟项目网站
版权所有 (c) 2025 Deepseek / 玄曦雪
基于 hunar4321/particle-life (MIT License)
```

---

## 🙏 致谢

### 核心贡献
- **hunar4321** - [原始粒子生命项目](https://github.com/hunar4321/particle-life)
- **Jeffery Ventrella** - Clusters项目灵感
- **开源社区** - 多语言移植和优化

### 技术依赖
| 项目 | 用途 | 许可证 |
|------|------|--------|
| TailwindCSS | CSS框架 | MIT |
| Font Awesome | 图标库 | MIT/SIL OFL 1.1 |
| Google Fonts | 网页字体 | Apache 2.0 |
| OpenFrameworks | C++图形框架 | MIT |

### 特别感谢
感谢所有为粒子生命模拟项目做出贡献的开发者，特别是那些创建了不同编程语言端口的贡献者，让这个项目能够在更多平台和环境中运行。

---

## 📞 支持与反馈

### 问题报告
如果您在使用过程中遇到问题：

1. **查看演示**：先确认在线演示是否正常工作
2. **检查控制台**：浏览器开发者工具查看错误信息
3. **搜索Issues**：在GitHub Issues中查找类似问题
4. **提交新Issue**：提供详细的问题描述和环境信息

### 交流社区
- **GitHub Discussions**：技术讨论和想法分享
- **YouTube评论区**：教程相关问题和反馈
- **相关论坛**：人工生命和复杂系统社区

---

<div align="center">

## 🎉 立即体验

**探索从简单规则中涌现的复杂生命模式**

[🚀 启动2D演示](https://hunar4321.github.io/particle-life/particle_life.html) • 
[🌐 访问3D版本](https://hunar4321.github.io/particle-life/particle_life_3d.html) • 
[📺 观看教程](https://youtu.be/0Kx4Y9TVMGg)

*见证简单规则如何创造出令人惊叹的复杂模式*

**网站开发者**: Deepseek / 玄曦雪  
**核心算法**: hunar4321  
**最后更新**: 2025年11月7日  

</div>
