## nodejs和npm关系
#### node.js是javascript的一种运行环境，是对Google V8引擎进行的封装。是一个服务器端的javascript的解释器。
#### 其实npm是nodejs的包管理器（package manager）。我们在Node.js上开发时，会用到很多别人已经写好的javascript代码，如果每当我们需要别人的代码时，都根据名字搜索一下，下载源码，解压，再使用，会非常麻烦。于是就出现了包管理器npm。大家把自己写好的源码上传到npm官网上，如果要用某个或某些个，直接通过npm安装就可以了，不用管那个源码在哪里。并且如果我们要使用模块A，而模块A又依赖模块B，模块B又依赖模块C和D，此时npm会根据依赖关系，把所有依赖的包都下载下来并且管理起来。试想如果这些工作全靠我们自己去完成会多么麻烦！

### npm 是 node package manager 的缩写， 是用来管理用node开发出来的库，在安装vue cli时，需要全局安装，也就是所谓的-g， npm默认为将它安装在/user/local/lib/node——modules，第一个slash就是表示根目录，通俗的讲就是这个vue cli会available to 任何当前登陆系统，都可以无需安装直接使用。但是根目录的访问是要授权的，所以用sudo就可以工作，这时会要求提供密码。
