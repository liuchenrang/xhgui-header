# xhgui-header 中文版 精简依赖版
- 目标兼容php5 php7 php8
## 使用方式 
### 设置环境变量
- XHGUI_CONFIG_DEBUG 
  - 开启错误模式
- XHGUI_CONFIG_FILTER_PATH
  - 过滤某些路径,例如  111/11.html,222/22.html
- XHGUI_CONFIG_SHOULD_RUN
  - 是否开启
- XHGUI_CONFIG_EXTENSION
  - 使用的扩展
- XHGUI_CONFIG_SAVER_URL
  - 数据采集地址
- XHGUI_CONFIG_PERCENT
  - 采集百分比
### 添加appdend file

- append_file=src/main/header.php
如果要自定义保存器，在append_file之前 在append_file 一个文件，定义一个全局函数 _XhguiHeader_SimpleUrl($data)

## 使用注意事项

- 项目代码需要跑在php-fpm模式下