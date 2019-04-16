## 欢迎使用代码生成工具

一款从数据库逆向生成代码工具，开发该工具的初衷概念模型->逻辑模型->物理模型->生成代码，以释放双手为目的，各大模板也在陆续补充和优化。如有发现bug、建议和建议欢迎提交issue,谢谢！

支持win，macos欢迎[下载](https://github.com/eshun/pandora-doc/releases)

### 功能

- [x] 支持mysql库,其他数据库开发中
- [x] 支持生成JPA/JdbcTemplate/Mybatis代码
- [x] 支持生成vue element ui
- [x] 支持lombok
- [x] 支持swagger api
- [x] 支持模版编辑
- [ ] 一对多，多对多


### 模版编辑

工具提供可视化界面编辑模版，自定义模版。
```
{% raw %}{{packageName}}{% endraw %}包名
{% raw %}{{author}}{% endraw %}开发者
{% raw %}{{day}}{% endraw %}当期日期
{% raw %}{{className}}{% endraw %}类名

{% raw %}{{tableName}}{% endraw %}表名
{% raw %}{{tableInfo}}{% endraw %}表
{% raw %}{{pri}}{% endraw %}表第一个主键

{% raw %}{{columns}}{% endraw %}所有列
{% raw %}{{columnName}}{% endraw %}列名
{% raw %}{{oldColumnName}}{% endraw %}原列名
{% raw %}{{columnKey}}{% endraw %}是否主键
{% raw %}{{isNull}}{% endraw %}是否可为空
{% raw %}{{columnComment{% endraw %}列备注
{% raw %}{%if value%} ... {%endif%}{% endraw %}条件语句
{% raw %}{%for column in columns%}{{column.columnName}}{%endfor%}{% endraw %}循环语句
```

### 部分界面

![head](images/1.jpeg)

![head](images/2.png)

![head](images/3.png)

![head](images/4.png)
