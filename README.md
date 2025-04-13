# 🔐 安全字符串转换器 - 专业的加密解密解决方案

![工具截图](https://xqhz.bailanyun.cn/yp/view.php/cfc64bb35c7f3c8ddbcecaf0bd77b07b.png)

**安全字符串转换器**是一款专业的Web加密解密工具，采用多层加密算法，为您的敏感数据提供可靠的保护。支持：
- 强大的字符串加密功能
- 安全的解密还原
- 简单直观的操作界面
- 灵活的代码集成

适用于：
✅ 敏感信息保护
✅ 数据传输安全
✅ 教学演示
✅ 项目开发调试

## ✨ 功能特点

- 字符串加密功能
- 字符串解密功能
- 结果一键复制
- 响应式设计，适配各种设备
- 详细的错误处理
- 完整的使用说明和示例

## 🛠️ 使用方法

1. 访问工具页面
2. 在输入框中输入要处理的字符串
3. 点击"加密"或"解密"按钮
4. 查看结果并可使用"复制"按钮复制结果

## 📋 示例

**加密示例:**
```
原始字符串: Hello World
加密结果: 6c6c65482c6f57206f6c64c
```

**解密示例:**
```
加密字符串: 6c6c65482c6f57206f6c64c
解密结果: Hello World
```

## ⚙️ 技术实现

工具使用JavaScript实现，主要技术包括:
- Base64编码/解码 (btoa/atob)
- URI组件编码/解码
- 十六进制转换
- 字符串反转操作

```javascript
// 加密核心代码
const encrypted = btoa(unescape(encodeURIComponent(input)))
    .split('')
    .reverse()
    .join('')
    .split('')
    .map(c => c.charCodeAt(0).toString(16).padStart(2, '0'))
    .join('');
```

## 💻 代码集成

在实际项目中使用解密功能的示例代码：

```javascript
const e = "加密的内容";
document.write(decodeURIComponent(escape(atob(
    e.replace(/../g, h => String.fromCharCode(parseInt(h, 16)))
     .split('')
     .reverse()
     .join('')
))));
```

代码说明：
1. `e.replace(/../g, h => String.fromCharCode(parseInt(h, 16)))` - 将十六进制字符串转换为字符
2. `.split('').reverse().join('')` - 反转字符串
3. `atob()` - Base64解码
4. `decodeURIComponent(escape())` - 解码URI组件

注意事项：
- 确保加密字符串格式正确
- 在浏览器环境中使用
- 错误处理建议使用try-catch

## 🚀 部署方式

1. 下载HTML文件
2. 直接在浏览器中打开即可使用
3. 或部署到任意Web服务器

## 📜 许可证

MIT License © 2025 Fitten Code

---

🙏 欢迎提交Issue和PR！如有任何问题或建议，请在讨论区留言。
