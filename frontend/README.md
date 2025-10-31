# Vue 3 + TypeScript + Vite

This template should help get you started developing with Vue 3 and TypeScript in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.

Learn more about the recommended Project Setup and IDE Support in the [Vue Docs TypeScript Guide](https://vuejs.org/guide/typescript/overview.html#project-setup).
 
 ## 目录结构说明

下面给出项目前端部分（`frontend/`）的主要目录树与说明，方便快速定位代码与资源：

```
frontend/
	index.html                 # 应用入口 HTML
	package.json               # 前端依赖与脚本
	README.md                  # 本文件
	tsconfig*.json             # TypeScript 配置
	vite.config.ts             # Vite 配置
	public/                    # 静态资源，直接原样拷贝到构建输出
	src/
		main.ts                  # 应用入口（挂载 Vue）
		App.vue                  # 根组件
		style.css                # 全局样式
		assets/                  # 图片、图标等静态资源（可由代码引用）
		components/              # 可复用组件
			HelloWorld.vue
			module/
				trainModel.vue       # 训练模型相关组件
				viewModel.vue        # 查看模型相关组件
			project/
				dataList.vue         # 数据列表组件
				taskList.vue         # 方案列表组件
				userList.vue         # 用户列表组件
		views/                   # 页面级别视图组件（路由视图）
			AccountSettings.vue
			DataDetail.vue
			ProjectDetail.vue
			ProjectManage.vue
			RecycleBin.vue
			TaskDetail.vue
			UserLogin.vue

```

说明（简要）：
- `src/components/`：放置可复用的小组件与模块化子组件。模块化子目录（如 `module/`、`project/`）用于按功能分组。
- `src/views/`：对应路由级页面，每个文件通常对应一个页面视图。
- `public/`：放置 favicon、robots、静态文件等，构建时直接复制到输出目录。
- `vite.config.ts` 与 `tsconfig*.json`：分别是构建与 TypeScript 的配置文件。

如果你需要我把这个目录树扩展为更详细的文档（例如每个组件/页面的职责、主要 props 或接口），告诉我想要的深度，我可以继续完善。
