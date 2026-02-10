# 词汇卡片生成器 (Vocabulary Card Generator)

一个简单易用的单词卡片生成工具，可生成支持翻转和发音功能的交互式HTML卡片页面。

## 功能特性

- 📝 **简单输入**：支持多种格式的单词列表输入
- 🔄 **翻转效果**：点击卡片即可查看背面的详细解释
- 🔊 **发音功能**：支持单词发音，多种TTS方案自动切换
- 📱 **响应式设计**：适配各种屏幕尺寸
- 💾 **自动保存**：每次生成带时间戳的独立HTML文件，不会覆盖
- 🎨 **美观设计**：清晰的字体和优雅的布局

## 使用方法

### 方式一：本地使用

1. 将单词列表发送给Claude，格式如下：

```
单词1 | 解释1
单词2 | 解释2
单词3 | 解释3
```

2. 系统会自动生成HTML文件
3. 在浏览器中打开即可使用

### 方式二：在线使用

访问 [GitHub Pages](https://[your-username].github.io/vocabulary-card-generator/) 使用在线版本。

## 输入格式

支持两种分隔格式：

```
格式1: 单词 | 解释
apple | 苹果，一种常见的水果

格式2: 单词, 解释
banana | 香蕉，热带水果
```

## 示例

```
apple | 苹果，一种常见的水果
banana | 香蕉，热带水果，黄色弯曲
orange | 橙子，柑橘类水果，富含维生素C
```

## 发音功能

- **首选方案**：Web Speech API（浏览器内置）
- **备用方案**：HTML5 Audio
- **第三方案**：在线TTS服务

系统会自动检测并使用最佳可用方案。

## 浏览器兼容性

| 浏览器 | 发音功能 | 翻转效果 |
|--------|----------|----------|
| Chrome | ✅ | ✅ |
| Edge | ✅ | ✅ |
| Firefox | ⚠️ | ✅ |
| Safari | ⚠️ | ✅ |

推荐使用 Chrome 或 Edge 以获得最佳体验。

## 项目结构

```
vocabulary-card-generator/
├── SKILL.md                # Claude Skill 配置文件
├── README.md               # 项目说明文档
└── *.html                  # 生成的单词卡片文件
```

## 技术栈

- HTML5
- CSS3 (3D Transforms)
- JavaScript (ES6+)
- Web Speech API

## 许可证

MIT License

## 贡献

欢迎提交 Issue 和 Pull Request！

---

由 [Claude Code](https://claude.com/claude-code) 生成
