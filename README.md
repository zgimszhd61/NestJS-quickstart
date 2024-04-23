# NestJS-quickstart
 - https://github.com/nestjs

NestJS 是一个用于构建高效、可扩展的 Node.js 服务器端应用程序的框架。它使用现代 JavaScript，内置 TypeScript 支持，并结合了面向对象编程、函数式编程和函数响应式编程的元素。下面是一个简单的 NestJS Quickstart 指南，让你快速开始一个基本的项目。

### 步骤 1: 安装 NestJS CLI

首先，你需要安装 NestJS 的命令行工具。打开终端并运行以下命令：

```bash
npm i -g @nestjs/cli
```

### 步骤 2: 创建新项目

使用 CLI 创建一个新项目：

```bash
nest new project-name
```

替换 `project-name` 为你想要的项目名称。这将创建一个新目录，包含所有必要的文件和依赖。

### 步骤 3: 进入项目目录

切换到项目目录中：

```bash
cd project-name
```

### 步骤 4: 运行开发服务器

使用以下命令启动你的开发服务器：

```bash
npm run start:dev
```

这将启动一个热重载服务器，任何代码改动都会自动重启服务器。

### 步骤 5: 创建一个简单的 Controller

在 NestJS 中，你可以使用装饰器来定义路由。打开你的项目，在 `src` 目录下找到 `app.controller.ts` 文件，并修改它来添加一个新的路由：

```typescript
import { Controller, Get } from '@nestjs/common';

@Controller('hello')
export class AppController {
  @Get()
  getHello(): string {
    return 'Hello World!';
  }
}
```

### 步骤 6: 测试你的应用

打开浏览器并访问 `http://localhost:3000/hello`，你应该能看到返回的 "Hello World!"。

### 总结

这个快速开始指南展示了如何使用 NestJS 创建一个基本的项目，并包括了一个简单的控制器示例。NestJS 提供了很多高级特性和模块，例如中间件、过滤器、守卫等，你可以继续探索这些功能来扩展你的应用。

