TypeScript Yarn Workspaces Share Dependencies on Root Demo
=================================

使用`yarn`的workspaces功能管理多个package，并且在root共享一些dependency

在这种情况下，子workspace的package.json中不需要在dependency中添加需要的依赖，可以直接用。
（但是，感觉似乎有点不太好？要不放在peerDependencies里声明一下？）

如果想把某个dependency安装在根目录，需要加上`-W`参数：

```
yarn add lodash -W
```

运行

```
cd packages/workspaces-b
yarn run demo
```


