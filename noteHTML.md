// <meta name="robots" content="noindex">
### 上述示例中的漫游器元标记可指示大多数搜索引擎不要在搜索结果中显示相应网页。name 属性的值 (robots) 
### 指定此指令适用于所有抓取工具。要使此指令仅适用于某一具体抓取工具，请用该抓取工具的名称替换 name 属性的 robots 值。
### 具体的抓取工具也称为用户代理（抓取工具使用其用户代理请求网页）。Google 的标准网页抓取工具的用户代理名称为 Googlebot。
### 如果只是要禁止 Googlebot 抓取您的网页，请按如下所示更新标记：
#<meta name="googlebot" content="noindex" />
