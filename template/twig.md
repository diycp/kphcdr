### twig
#### 官方说明
> Twig, the flexible, fast, and secure template language for PHP

#### github地址
[https://github.com/twigphp/Twig](https://github.com/twigphp/Twig)

#### 个人评价

**评测日期**：2016年04月11日

**文档分**：5分

**易学分**：4分

**易用分**：9分

**扩展性**：6分

**优点**

> 这是一个把PHP带入一个新纪元的模板引擎
> 模板继承和block，使用起来爽翻
> 框架优雅，类js的外表，让前端工程师也能用起来

**缺点**

> 学习成本略高
> 使用composer加载后，较难扩展

**代码片段**

	{% for a in data %}
    <tr>
        <td>{{ a.id }}</td>
        <td>{{ a.name }}</td>
        <td>{{ a.cname }}</td>
        <td>{{ a.is_use==0 ? '可用' : '不可用' }}</td>
        <td>
            <a href="/article/infoarticle/id/{{ a.id}}" class="label label-info" data-original-title="">编辑</a>
            <a data-url="/article/delarticle/id/{{ a.id}}" href="javascript:;" class="label label-danger btn-del" data-original-title="">删除</a>
        </td>
    </tr>
    {% endfor %}
