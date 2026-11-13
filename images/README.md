# 图片使用指南

## 目录结构

```
public/
  └── images/
      ├── posts/        # 博客文章中的图片
      └── README.md     # 本文件
```

## 如何在文章中使用图片

### 1. 上传图片

将图片文件放到 `public/images/posts/` 目录下。

例如：

- `public/images/posts/react-原理图.png`
- `public/images/posts/vapor-mode-diagram.jpg`

### 2. 在 Markdown 文章中引用

在你的文章（如 `src/content/posts/React的原理.md`）中使用以下格式：

```markdown
![图片描述](/images/posts/react-原理图.png)
```

**注意**：

- 路径以 `/` 开头（相对于网站根目录）
- 不需要写 `public`，因为 `public` 目录的内容会被直接复制到网站根目录

### 3. 示例

```markdown
## React 渲染流程

下面是 React 的渲染流程图：

![React 渲染流程图](/images/posts/react-render-flow.png)

这张图展示了...
```

## 图片命名建议

- 使用有意义的文件名
- 使用小写字母和连字符
- 避免使用空格和特殊字符
- 例如：`react-fiber-architecture.png`

## 图片格式建议

- **照片/截图**：使用 `.jpg` 或 `.webp`（更小的文件大小）
- **图表/示意图**：使用 `.png`（透明背景）
- **图标**：使用 `.svg`（矢量图，可缩放）

## 优化建议

1. **压缩图片**：使用工具（如 TinyPNG）压缩图片以加快加载速度
2. **合理尺寸**：文章图片宽度建议 800-1200px
3. **添加描述**：为图片添加有意义的 alt 文本，有利于 SEO 和无障碍访问
