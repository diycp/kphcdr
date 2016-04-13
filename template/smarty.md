### smarty
#### 官方说明
> Smarty 3 template engine

#### github地址
[https://github.com/smarty-php/smarty](https://github.com/smarty-php/smarty)

#### 个人评价

**评测日期**：2016年04月11日

**文档分**：9分

**易学分**：7分

**易用分**：4分

**扩展性**：8分

**优点**

> 老东西了，用过PHP的人都听过这玩意

> 因为存在时间比较长，文档非常齐全

> 自定义函数的功能非常好用，扩展性非常棒

> 自带简单的调试功能

**缺点**

> 框架比较重，性能上有瓶颈

> 当年优秀的模板缓存，在今天略显格格不入

**代码片段**

    {section name=outer
    loop=$FirstName}
        {if $smarty.section.outer.index is odd by 2}
            {$smarty.section.outer.rownum} . {$FirstName[outer]} {$LastName[outer]}
        {else}
            {$smarty.section.outer.rownum} * {$FirstName[outer]} {$LastName[outer]}
        {/if}
        {sectionelse}
        none
    {/section}
