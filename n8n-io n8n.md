# n8n - 面向技术团队的安全工作流自动化

n8n 是一个工作流自动化平台，赋予技术团队代码的灵活性和无代码的速度。通过 400 多个集成、原生 AI 功能和公平代码许可证，n8n 让您在保持对数据和部署的完全控制的同时，构建强大的自动化流程。

## 关键功能

- **需要时编写代码**：编写 JavaScript/Python，添加 npm 包，或使用可视化界面
- **原生 AI 平台**：基于 LangChain 使用您自己的数据和模型构建 AI 代理工作流
- **完全控制**：使用我们的公平代码许可证进行自托管或使用我们的 [云服务](https://app.n8n.cloud/login)
- **企业级准备**：高级权限、单点登录（SSO）和隔离部署
- **活跃社区**：400 多个集成和 900 多个现成的 [模板](https://n8n.io/workflows)

## 快速开始

通过 [npx](https://docs.n8n.io/hosting/installation/npm/)（需要 [Node.js](https://nodejs.org/en/)）立即尝试 n8n：

```
npx n8n
```

或使用 [Docker](https://docs.n8n.io/hosting/installation/docker/) 部署：

```
docker volume create n8n_data
docker run -it --rm --name n8n -p 5678:5678 -v n8n_data:/home/node/.n8n docker.n8n.io/n8nio/n8n
```

访问编辑器：http://localhost:5678

## 资源

- 📚 [文档](https://docs.n8n.io)
- 🔧 [400+ 集成](https://n8n.io/integrations)
- 💡 [示例工作流](https://n8n.io/workflows)
- 🤖 [AI & LangChain 指南](https://docs.n8n.io/langchain/)
- 👥 [社区论坛](https://community.n8n.io)
- 📖 [社区教程](https://community.n8n.io/c/tutorials/28)

## 支持

需要帮助吗？我们的社区论坛是获取支持和与其他用户联系的地方：
[community.n8n.io](https://community.n8n.io)

## 许可证

n8n 采用 [公平代码](https://faircode.io) 许可证，分发在 [可持续使用许可证](https://github.com/n8n-io/n8n/blob/master/LICENSE.md) 和 [n8n 企业许可证](https://github.com/n8n-io/n8n/blob/master/LICENSE_EE.md) 下。

- **源代码可见**：始终可见的源代码
- **可自托管**：可在任何地方部署
- **可扩展**：添加您自己的节点和功能

可通过 [电子邮件](mailto:license@n8n.io) 获取额外功能和支持的企业许可证。

有关许可证模型的更多信息，请参见 [文档](https://docs.n8n.io/reference/license/)。

## 贡献

发现了错误 🐛 或有功能想法 ✨？请查看我们的 [贡献指南](https://github.com/n8n-io/n8n/blob/master/CONTRIBUTING.md) 开始。

## 加入团队

想要塑造自动化的未来吗？查看我们的 [招聘信息](https://n8n.io/careers) 并加入我们的团队！

## n8n 的含义是什么？

**简短回答**：它意味着“nodemation”，发音为 n-eight-n。

**详细回答**：“我经常被问到这个问题（比我预期的要多），所以我决定最好在这里回答。寻找一个好的项目名称时，我很快意识到我能想到的所有好名字都已经被占用了。最后，我选择了 nodemation。'node-' 是指它使用 Node-View 和 Node.js，'-mation' 是指自动化，这是该项目旨在帮助的内容。然而，我不喜欢这个名字太长，也无法想象每次在 CLI 中写这么长的东西。于是我最终选择了 'n8n'。” - **Jan Oberhauser，n8n.io 创始人兼首席执行官**
