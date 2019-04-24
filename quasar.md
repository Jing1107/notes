### 目录结构
.
├── src/
│   ├── assets/              # 动态资源（由webpack处理）
│   ├── statics/             # 纯静态资源（直接复制）
│   ├── components/          # 用于页面和布局的.vue组件
│   ├── css/                 # CSS/Stylus/Sass/...文件
|   |   ├── app.styl
|   │   └── themes/          # Quasar主题入口点供您调整
|   │       ├── common.variables.styl # 所有Quasar主题的常用Stylus变量
|   │       ├── variables.mat.styl    # Material Design主题的变量
|   │       └── variables.ios.styl    # iOS主题的变量
│   ├── layouts/             # 布局 .vue 文件
│   ├── pages/               # 页面 .vue 文件
│   ├── plugins/             # app插件 (app初始化代码)
│   ├── router/              # Vue路由器
|   |   ├── index.js         # Vue路由器定义
|   │   └── routes.js        # App路由器定义
│   ├── store/               # Vuex Store
|   |   ├── index.js         # Vuex Store 定义
|   │   ├── <folder>         # Vuex Store 模块...
|   │   └── <folder>         # Vuex Store 模块...
│   ├── App.vue              # APP的根Vue组件
│   └── index.template.html  # index.html模板
├── src-pwa/                 # PWA特定代码（如Service Worker）
├── src-cordova/             # Cordova生成的文件夹用于创建移动APP
├── src-electron/            # Electron特定代码（如"main"线程)
├── dist/                    # 生产版本代码，用于部署
│   ├── spa-mat/             # 使用MAT主题构建SPA应用生产代码
│   ├── spa-ios/             # 使用IOS主题构建SPA应用生产代码
│   ├── electron-mat/        # 使用MAT主题构建Electron应用生产代码
│   └── ....
├── quasar.conf.js           # Quasar App配置文件
├── .babelrc                 # babel配置
├── .editorconfig            # editor配置
├── .eslintignore            # ESlint忽略路径
├── .eslintrc.js             # ESlint配置
├── .postcssrc.js            # PostCSS配置
├── .stylintrc               # Stylus lint配置
├── .gitignore               # GIT忽略路径
├── package.json             # npm脚本和依赖项
└── README.md                # 您的网站/应用程序的自述文件


## common error
### Newline required at end of file but not found/ 需要在结尾再下行一行
### Trailing spaces not allowed /不允许尾随空间，把eslint检测关闭
## Expected indentation of 2 spaces but found 4