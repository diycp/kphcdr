#说明
以下评测为个人片面了解后得出的结论，不代表项目的真实情况
##数据库类

### medoo
#### 官方说明
> The Lightest PHP database framework to accelerate development

#### github地址
[https://github.com/catfan/Medoo](https://github.com/catfan/Medoo)

#### 个人评价

**评测日期**：2016年04月11日

**文档分**：8分

**易学分**：8分

**易用分**：6分

**扩展性**：2分

**优点**

> 使用简单，上手快速，略微查看文档后即可上手使用。
> 可以在多种数据库中无缝切换，推荐在小型项目中使用

**缺点**
> 经过测试和使用，发现medoo针对于表前缀的支持非常差，包括不限于多表查询和field，作者更新速度不及时，对于合并请求的处理也比较懒惰。

**代码片段**

		return $this->get('goods',array(
				"[>]g" => ["g_id" => "id"],
				"[>]goods_category(c)" => ["c_id" => "id"],
		),array(
			'g.name','g.photo(gphoto)','goods.photo','c.name(cname)',
		),array(
			'AND'=>array('g.id' => $id,'c.is_use'=>0),
		    'ORDER'=>array('goods.sort ASC','goods.id DESC'),
			'LIMIT' =>1
		));








