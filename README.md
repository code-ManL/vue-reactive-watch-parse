{
  "compilerOptions": {
    "outDir": "dist", // 输出的目录
    "sourceMap": true, // 采用sourcemap
    "target": "ESNext", // 目标语法
    "module": "esnext", // 模块格式
    "moduleResolution": "node", // 模块解析方式
    "strict": false, // 严格模式
    "resolveJsonModule": true, // 解析json模块
    "esModuleInterop": true, // 允许通过es6语法引入commonjs模块
    "jsx": "preserve", // jsx 不转义
    "lib": ["esnext", "dom"], // 支持的类库 esnext及dom
    "baseUrl": ".", // 以当前路径为基准进行查找
    "paths": {
      "@vue/*":["packages/*/src"] // 引入@vue 都去packages 下查找
    }
  },
  "include": [
    "packages/*/src",
    "packages/*/__tests__",
  ]
}