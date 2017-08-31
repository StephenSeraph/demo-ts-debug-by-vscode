### vscode下的ts开发调试配置demo

1. 终端里`tsc --init`生成`tsconfig.json`；将`"sourceMap": true,`取消注释，这将在编译时生成`.map`文件
2. 终端里`touch main.ts`创建`main.ts`，然后写点测试代码
3. vscode里`ctr+shift+p`调出面板，搜索`task`，生成`tasks.json`，不需要修改
4. vscode里生成`node`的`launch.json`，将`program`属性改为需要运行的js文件`${workspaceRoot}/main.js`
5. `ctrl+shift+b`编译，并且在后续的每次编辑之后、调试之前都要编译一下
6. `f5`调试
