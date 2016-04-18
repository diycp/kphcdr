### Seaslog
#### 官方说明
> An effective,fast,stable log extension for PHP

#### github地址
[https://github.com/Neeke/SeasLog](hhttps://github.com/Neeke/SeasLog)

#### 个人评价

**评测日期**：2015年12月25日

**文档分**：8分

**易学分**：9分

**易用分**：5分

**扩展性**：1分

**优点**

> 作为PHP扩展形式加载，性能刚刚的

> 一次安装，终身使用，无需配置，上手就用

> 使用简单，文档精美，优雅又高效

**缺点**

> 基于C语言开发，扩展性基本为0

> 门槛较高，需要对熟悉Linux操作和PHP扩展安装 

**代码片段**

		SeasLog::log(SEASLOG_ERROR,'this is a error test by ::log');

		SeasLog::debug('this is a {userName} debug',array('{userName}' => 'neeke'));
		
		SeasLog::info('this is a info log');
		
		SeasLog::notice('this is a notice log');
		
		SeasLog::warning('your {website} was down,please {action} it ASAP!',array('{website}' => 'github.com','{action}' => 'rboot'));
		
		SeasLog::error('a error log');
		
		SeasLog::critical('some thing was critical');
		
		SeasLog::alert('yes this is a {messageName}',array('{messageName}' => 'alertMSG'));
		
		SeasLog::emergency('Just now, the house next door was completely burnt out! {note}',array('{note}' => 'it`s a joke'));

