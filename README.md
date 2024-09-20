## 以 github 仓库的方式部署到 cloudflare
可以将构建好的代码发布到 cloudflare, 现在以 github 仓库的方式来发布
先把整个工程上传到 github ：
https://github.com/qyzhizi/cloudflare_getStarted_react_vite_tsx_demo/tree/main
然后登录 cloudflare ，进入 worker 与 page 页面，选择 page 然后授权 cloudflare_getStarted_react_vite_tsx_demo 仓库
之后进行部署设置
架构可以选择 vue 或者不选
构建命令 ：npm run build
构建命令可以在 package.json 中找到
构建输出目录：dist

最终的网页地址： https://cloudflare-getstarted-react-vite-tsx-demo.pages.dev/

## React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

### Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
}
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list
